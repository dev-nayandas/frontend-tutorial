[Make a project](#make-project)<br>
[Tailwind Installation](#tailwind-install)<br>
[Tailwind Initialize](#initialize-tailwind-css)<br>
[Tailwind Config](#tailwind-css-config)<br>
[index.css config](#index-css-config)<br>
[Animation Addition at tailwind](#add-animation-at-tailwind)<br>
[Basic Form Handle](#form-handle)<br>
[Basic add and edit by same form](#basic-add-and-edit-by-same-form)<br>
[Basic delete an item](#basic-delete-item)<br>
[Basic delete all item](#basic-delete-all)<br>
[Basic Toggle](#basic-toggle)<br>
[Basic Search ](#basic-search)<br>
[Sort Implementations](#sort-implementations)<br>
[Export Data By a function](#export-data-by-function)<br>
[Filter data By a function](#filter-data-by-function)<br>
[Image url generation by a function and how to use it](#image-url-generator-function)<br>
[Make a Rating Component to dynamic rating](#rating-component)<br>
[How to open a modal with data](#modal-with-data)<br>
[Stop Propagation](#stop-propagation)<br>
[How to use context api](#context-api)<br>


`##` Make a project
## make-project

```javascript
npm create vite@latest tic-tac-toe -- --template react
```

`##` Install Tailwind css dependencies
## tailwind-install


```javascript
npm install -D tailwindcss postcss autoprefixer
```

`##` Initial Tailwind css
## initialize-tailwind-css


```javascript
npx tailwindcss init -p
```

`##` at tailwind.config
## tailwind-css-config


```javascript
content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
```

`##` Clean index.css and add below declarations
## index-css-config


```javascript
@tailwind base;
@tailwind components;
@tailwind utilities;
```

`##` Add animation using className, at index.css
## add-animation-at-tailwind


```javascript
@tailwind base;
@tailwind components;
@tailwind utilities;


@layer components {
    .animate-updown {
        animation-name: animate-updownAnim;
        animation-duration: 2s;
        animation-iteration-count: infinite;
        animation-direction: alternate-reverse;
    }

    @keyframes animate-updownAnim {
        from {
            transform: translateY(-20px);
        }
        to {
            transform: translateY(20px);
        }
    }
}
```

`##` Basic React Form Handle
## form-handle


- [How To Handle form In react form code](https://github.com/Learn-with-Sumit/rnext/blob/2.10/src/task/AddTaskModal.jsx)
- [How To Handle form In react parent code](https://github.com/Learn-with-Sumit/rnext/blob/2.10/src/task/TaskBoard.jsx)

`##` Basic Add and edit by same form in an array
## basic-add-and-edit-by-same-form


- [Form's details](https://github.com/Learn-with-Sumit/rnext/blob/2.10/src/task/AddTaskModal.jsx)
- [Parents details](https://github.com/Learn-with-Sumit/rnext/blob/2.10/src/task/TaskBoard.jsx)
- [Edit details](https://github.com/Learn-with-Sumit/rnext/blob/2.10/src/task/TaskList.jsx)

```javascript
function handleAddEditTask(newTask, isAdd) {
  if (isAdd) {
    setTasks([...tasks, newTask]);
  } else {
    setTasks(
      tasks.map((task) => {
        if (task.id === newTask.id) {
          return newTask;
        }
        return task;
      })
    );
  }

  handleCloseClick();
}

function handleEditTask(task) {
  setTaskToUpdate(task);
  setShowAddModal(true);
}
```

`##` Basic Delete item
## basic-delete-item

```javascript
function handleDeleteTask(taskId) {
  const tasksAfterDelete = tasks.filter((task) => task.id !== taskId);
  setTasks(tasksAfterDelete);
}
```

`##` Basic Delete all items
## basic-delete-all


```javascript
function handleDeleteAllClick() {
  tasks.length = 0;
  setTasks([...tasks]);
}
```

`##` Basic Toggle
## basic-toggle

```javascript
function handleFavorite(taskId) {
  // This portion of the commented code is not fully perfect. Here
  // we are not doing the deep cloning of the tasks array. The tasks array has
  // objects inside, while using the spread operator, it will only make the shallow copy.
  // But we need to do the deep copy.

  // We are not removing this commented code as it was part of the recording.
  // But the same code is now made better and written below.
  /*
        const taskIndex = tasks.findIndex((task) => task.id === taskId);
        const newTasks = [...tasks];
        newTasks[taskIndex].isFavorite = !newTasks[taskIndex].isFavorite;
        setTasks(newTasks);
        */

  // The better way of managing updates in the object within an array as a
  // state in react.
  setTasks(
    tasks.map((task) => {
      if (task.id === taskId) {
        return { ...task, isFavorite: !task.isFavorite };
      } else {
        return task;
      }
    })
  );
}
```

`##` Basic Search Implementation
## basic-search

```Javascript
 // search component
  const [searchTerm, setSearchTerm] = useState("")
  const handleClick = (e) =>{
    e.preventDefault()
    onSearch(searchTerm)// SearchTerm will come as props
  }
 //input and button's code
    <input
        type="search"
        id="search-dropdown"
        className="z-20 block w-full bg-gray-800 px-4 py-2 pr-10 focus:outline-none"
        placeholder="Search Task"
        value={searchTerm}
        onChange={(e) => setSearchTerm(e.target.value)}
        required
    />
    <button
        onClick={handleClick}
        type="submit"
        className="absolute right-2 top-0 h-full rounded-e-lg text-white md:right-4"
    >
        Search
        <span className="sr-only">Search</span>
    </button>

     //Parent's code
        const handleSearch = (searchTerm) => {
            console.log(searchTerm);
            const filteredTasks = tasks.filter(task => task.title.toLowerCase().includes(searchTerm.toLowerCase()));
            setTasks([...filteredTasks]);
  };
```

`##` How to implement sort
## sort-implementations

```javascript
//The array
const defaultData = [
  {
    id: crypto.randomUUID().toString(),
    title: "The Silent Patient",
    author: "Alex Michaelides",
    publicationDate: "2019-02-05",
    price: "20",
    rating: "4.5",
    isFavorite: false,
    cover: book,
  },
];
//Parent's code
const handleSort = (sortOption) => {
  let sortedBooks = [...books];
  switch (sortOption) {
    case "name_asc":
      sortedBooks.sort((a, b) => a.title.localeCompare(b.title));
      break;
    case "name_desc":
      sortedBooks.sort((a, b) => b.title.localeCompare(a.title));
      break;
    case "year_asc":
      sortedBooks.sort((a, b) => {
        const yearA = new Date(a.publicationDate).getFullYear();
        const yearB = new Date(b.publicationDate).getFullYear();
        return yearA - yearB;
      });
      break;
    case "year_desc":
      sortedBooks.sort((a, b) => {
        const yearA = new Date(a.publicationDate).getFullYear();
        const yearB = new Date(b.publicationDate).getFullYear();
        return yearB - yearA;
      });
      break;
    default:
      // No sorting
      break;
  }

  setBooks(sortedBooks);
};
//child'd code
/* eslint-disable react/prop-types */
const Sort = ({ onSortChange }) => {
  const handleChange = (event) => {
    onSortChange(event.target.value);
    console.log(event.target.value);
  };

  return (
    <div className="flex items-stretch space-x-3">
      <select
        className="cursor-pointer rounded-md border px-4 py-2 text-center text-gray-600"
        name="sortBy"
        id="sortBy"
        onChange={handleChange}
      >
        <option value="">Sort</option>
        <option value="name_asc">Name (A-Z)</option>
        <option value="name_desc">Name (Z-A)</option>
        <option value="year_asc">Publication Year (Oldest)</option>
        <option value="year_desc">Publication Year (Newest)</option>
      </select>
    </div>
  );
};

export default Sort;
```

`##` How to export data by a function
## export-data-by-function
```javascript
function getAllMovies() {
  return data; // Here data is the array and we can import and call the function in other components
}

export { getAllMovies };
```

`##` How to filter data by a function
## filter-data-by-function

```javascript
function getFavoriteMovies() {
  return data.filter((movie) => movie.isFavorite); // Here data is the array and we can import and call the function in other components
}

export { getFavoriteMovies };
```

`##` How to make image url generating function for react vite projects
## image-url-generator-function

```javascript
///make a folder called utils and create a file called cine-utility.js
const getImageUrl = (name) => {
  return new URL(`../assets/movie-covers/${name}`, import.meta.url).href;
};
export { getImageUrl };

/// how to use this function
/// eslint-disable react/prop-types , one thing to be remembered that is cover title name and cover image name should be same
import Rating from "./Rating";
import tag from "./assets/tag.svg";
import { getImageUrl } from "./utils/cine-utility";

const MovieCard = ({ movie }) => {
  console.log(movie);
  return (
    <figure className="p-4 border border-black/10 shadow-sm dark:border-white/10 rounded-xl">
      <img
        className="w-full object-cover"
        src={getImageUrl(movie?.cover)}
        alt=""
      />
    </figure>
  );
};

export default MovieCard;
```

`##` How to make Rating components
## rating-component

```javascript
///component
/* eslint-disable react/prop-types */
import star from "./assets/star.svg";
const Rating = ({ value }) => {
  const stars = Array(value).fill(star);
  return (
    <>
      {stars.map((star, index) => (
        <img key={index} src={star} width="14" height="14" alt="" />
      ))}
    </>
  );
};
export default Rating;


///use of the rating component, jus pass the value to the rating component which is a number
<div className="flex items-center space-x-1 mb-5">
  <Rating value={movie?.rating} />
</div>;
```

`##` How to open modal with data 
## modal-with-data
```javascript

///Card codes
import { useState } from "react";
import MovieDetails from "./MovieDetails";


const MovieCard = ({ movie }) => {
  const [showModal, setShowModal] = useState(false);
  const [selectedMovie, setSelectedMovie] = useState(null);

  const handleCloseMovieDetails = () => {
    setSelectedMovie(null);
    setShowModal(false);
  };
  const handleModalClick = (movie) => {

    setSelectedMovie(movie);
    setShowModal(true);
  };

  return (
    <>
      {showModal && (
        <MovieDetails movie={selectedMovie} onClose={handleCloseMovieDetails} />
      )}
      <figure className="p-4 border border-black/10 shadow-sm dark:border-white/10 rounded-xl">
        <a  onClick={() =>handleModalClick(movie)} href="#">
        {/* Other codes */}
        </a>
      </figure>
    </>
  );
};

export default MovieCard;




///Modal codes
import { getImageUrl } from "./utils/cine-utility";

const MovieDetails = ({movie, onClose}) => {

  return (
    <div className="fixed top-0 left-0 w-screen h-screen z-50 bg-black/60 backdrop-blur-sm">
      <div className="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 w-full max-w-[420px] sm:max-w-[600px] lg:max-w-[984px] p-4 max-h-[90vh] overflow-auto">
        <div className="bg-white shadow-md dark:bg-[#12141D] rounded-2xl sm:grid sm:grid-cols-[2fr_1fr] overflow-hidden">
          <div className="p-5 lg:p-11">
            <div className="grid lg:grid-cols-2 gap-2">
              <a
                onClick={onClose}
                className="border border-[#74766F] rounded-lg py-2 px-5 flex items-center justify-center gap-2 text-[#6F6F6F] dark:text-gray-200 font-semibold text-sm"
                href="#"
              >
                Cancel
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  );
};

export default MovieDetails;
```
`##`  How to stop propagation
## stop-propagation
```javascript
/* eslint-disable react/prop-types */
import { useState } from "react";
import MovieDetails from "./MovieDetails";
import Rating from "./Rating";
import tag from "./assets/tag.svg";
import { getImageUrl } from "./utils/cine-utility";

const MovieCard = ({ movie }) => {
  const [showModal, setShowModal] = useState(false);
  const [selectedMovie, setSelectedMovie] = useState(null);

  const handleCloseMovieDetails = () => {
    setSelectedMovie(null);
    setShowModal(false);
  };
  const handleModalClick = (movie) => {
    setSelectedMovie(movie);
    setShowModal(true);
  };

  const handleAddToCart = (e, movie) => {
    e.stopPropagation();
    console.log(movie)
  }

  return (
    <>
      {showModal && (
        <MovieDetails movie={selectedMovie} onClose={handleCloseMovieDetails} />
      )}
      <figure className="p-4 border border-black/10 shadow-sm dark:border-white/10 rounded-xl">
        <a onClick={() => handleModalClick( movie)} href="#">
          <img
            className="w-full object-cover"
            src={getImageUrl(movie?.cover)}
            alt=""
          />
          <figcaption className="pt-4">
            <h3 className="text-xl mb-1">{movie?.title}</h3>
            <p className="text-[#575A6E] text-sm mb-2">{movie?.genre}</p>
            <div className="flex items-center space-x-1 mb-5">
              <Rating value={movie?.rating} />
            </div>
            <a
              className="bg-primary rounded-lg py-2 px-5 flex items-center justify-center gap-2 text-[#171923] font-semibold text-sm"
              href="#"
              onClick={(e) => handleAddToCart(e, movie)}
            >
              <img src={tag} alt="" />
              <span>$100 | Add to Cart</span>
            </a>
          </figcaption>
        </a>
      </figure>
    </>
  );
};

export default MovieCard;
```
`##`  How to use context api
## context-api

```javascript

// make a folder at src folder called context and a index.js file it it  like below
/* eslint-disable react-hooks/rules-of-hooks */
import { createContext } from "react";


const MovieContext = createContext();


export {MovieContext};




// provide data  necessary   child
  /* eslint-disable no-unused-vars */
import { useState } from "react";
import { MovieContext } from "./context";

function App() {

  const [cartData, setCartData] = useState([])
  return (
    <>
    <MovieContext.Provider value={{cartData, setCartData}}>
      <NavBar />
      <main>
        <div className="container grid lg:grid-cols-[218px_1fr] gap-[3.5rem]">
          <SideBar />
          <MovieList />
        </div>
      </main>
      <Footer />
      </MovieContext.Provider>
    </>
  );
}

export default App;



// use the data where necessary example I have used it at MovieCard like below
/* eslint-disable react/prop-types */
import { useContext, useState } from "react";
import MovieDetails from "./MovieDetails";
import Rating from "./Rating";
import tag from "./assets/tag.svg";
import { getImageUrl } from "./utils/cine-utility";
import { MovieContext } from "./context";

const MovieCard = ({ movie }) => {
  const [showModal, setShowModal] = useState(false);
  const [selectedMovie, setSelectedMovie] = useState(null);
  const { cartData, setCartData } = useContext(MovieContext);

  const handleCloseMovieDetails = () => {
    setSelectedMovie(null);
    setShowModal(false);
  };
  const handleModalClick = (movie) => {
    setSelectedMovie(movie);
    setShowModal(true);
  };

  const handleAddToCart = (e, movie) => {
    e.stopPropagation();
    const found = cartData.find((item) => item.id === movie.id);
    
    if (found) {
      alert("Movie already in cart!");
      return;
    } else {
      setCartData([...cartData, movie]);
    }
  };

  return (
    <>
      {showModal && (
        <MovieDetails movie={selectedMovie} onClose={handleCloseMovieDetails} />
      )}
      <figure className="p-4 border border-black/10 shadow-sm dark:border-white/10 rounded-xl">
        <a onClick={() => handleModalClick(movie)} href="#">
          <img
            className="w-full object-cover"
            src={getImageUrl(movie?.cover)}
            alt=""
          />
          <figcaption className="pt-4">
            <h3 className="text-xl mb-1">{movie?.title}</h3>
            <p className="text-[#575A6E] text-sm mb-2">{movie?.genre}</p>
            <div className="flex items-center space-x-1 mb-5">
              <Rating value={movie?.rating} />
            </div>
            <a
              className="bg-primary rounded-lg py-2 px-5 flex items-center justify-center gap-2 text-[#171923] font-semibold text-sm"
              href="#"
              onClick={(e) => handleAddToCart(e, movie)}
            >
              <img src={tag} alt="" />
              <span>$100 | Add to Cart</span>
            </a>
          </figcaption>
        </a>
      </figure>
    </>
  );
};

export default MovieCard;

```
