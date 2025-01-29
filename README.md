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
[How to implement dark theme](#dark-theme)<br>
[How to implement useReducer ](#use-reducer)<br>
[How to implement React Toastify ](#react-toastify)<br>
[Open Weather Link ](#open-weather-map)<br>
[How to set and use .env ](#env-setting)<br>
[How to create and use custom hook and how to use context api with React composition pattern ](#custom-hook)<br>
[How to make utility function for formatted date](#formatted-date)<br>
[How to show icon by a function](#dynamic-icon)<br>
[How to add and remove something from local storage by ,custom hook, context api and provider](#local-storage-provider-context)<br>
[Send Value to a hook ](#send-value-to-provider)<br>
[How to use useDebounce hook ](#how-to-use-debounce)<br>
[React Router Dom ](#react-router-dom)<br>
[React Hook Form ](#react-hook-form)<br>
[Fetching Data with axios ](#axios-data-fetching)<br>
[Data Fetching With Axios and TansStackQuery ](#tans-stack-query-fetching-with-axios)<br>
[Suspense and Error Boundaries](#react-suspense)<br>
[React Lazy Load](#lazy-load)<br>
[Framer Motion](#framer-motion)<br>
[Firebase Authentication](#firebase)<br>
[React Infinite Scroll](#infinite-scroll)<br>
[React Styled Component](#styled-component)<br>
[React Virtualized](#react-virtualized)<br>
[React Portal](#react-portal)<br>
[React Redux](#react-redux)<br>
[Tailwind Custom Class add](#tailwind-custom-class)<br>
[Private Route](#private-route)<br>
[Store User Data By API Call](#store-data-by-api-call)<br>
[JWT Implementation](#jwt-implementation)<br>
[Use Reducer Advanced](#useReducer-advanced)<br>
[Multipart Image Upload](#multipart-image-upload)<br>
[How to make reuseable components](#reuseable-components)<br>
[Get Difference from now utility function](#get-difference-from-now)<br>
[Check the avatar of mine or others](#check-isme-avatar)<br>
[New User Registration](#new-user-registration)<br>
[Implement Like with api call](#implement-like-with-api)<br>
[Implement Comments with api call](#implement-comments-with-api)<br>
[Implement Delete with api call](#implement-delete-with-api)<br>
[Implement Create with api call](#implement-create-with-api)<br>
[Next Js Installation](#nextjs-installation)<br>
[Next Js Basic Setup in Installation Time](#nextjs-basic-setup)<br>
[How to make custom link so that it become a cline component](#custom-link)<br>
[How to make custom Programmatically navigate](#programmatically-naviagte)<br>
[How to set meta data](#set-meta-data)<br>
[How to get active link](#get-active-link)<br>
[How to get search params](#get-search-params)<br>
[Add Loading at Next js](#add-loading-at-nextjs)<br>
[How to add Route group](#add-route-group)<br>
[How to add more than one RootLayout](#add-more-than-one-root-layout)<br>
[How to add dynamic routes](#dynamic-routes)<br>
[How to get ReadMe files content](#readme-file-content)<br>
[How to filter for pathname](#filter-for-pathname)<br>
[DocuCraft full Resource](#docucraft-full-Resource)<br>
[Implement Search In advanced way](#implement-search-advanced-way)<br>
[Error handling at real life project](#error-handling-at-real-project)<br>
[Parallel Routes ](#parallel-routes)<br>
[Unmatched and intercepting routes ](#unmatched-and-intercepting-routes)<br>
[Parallel, unmatched and Intercepting Routes combination](#parallel-and-intercepting-routes-combination)<br>
[Route Handlers(CRUD)](#route-handlers)<br>
[Route Handlers(Search Params, cookies, caching , Redirecting)](#search-params-cookies-caching-redirecting)<br>
[Middleware](#middleware)<br>
[Next Js Not Found Page](#next-js-not-found-page)<br>
[Internalization](#internalization)<br>
[Basic Setup of photo feed](#basic-photo-feed)<br>
[Api creation in next js](#api-creation-in-next-js)<br>
[Internalization Implementation in photo feed](#internalization-at-photo-feed)<br>
[Full code of photo feed](#full-code-of-photo-feed)<br>
[How to import data Dynamically](#import-data-dynamically)<br>
[Data fetching, caching, and revalidating techniques in Next.js](#fetching-catching-revalidation)<br>
[Server Action - Introduction & Example with MongoDB Database](#server-action-with-mongodb)<br>
[Data Fetching Patterns and Best Practices - Sequential & Parallel Data Fetching & Progressive Rendering ](#sequential-parallel-progressive-rendering)<br>
[Full Next Weather Dashboard ](#weather-dashboard)<br>
[Data fetching in the server with fetch ](#data-fetching-in-server)<br>
[Data fetching in the server with fetch at route handler ](#data-fetching-in-server-route-handler)<br>
[Another way to prevent caching ](#another-way-to-prevent-caching)<br>
[We can Revalidate the fetching ](#revalidating-fetching)<br>
[Revalidation all fetch requests in a page and its child ](#revalidating-fetching-for-a-page-and-child)<br>
[De-Duplication ](#de-duplication)<br>
[Caching and Revalidation with Axios](#axios-caching-revalidation)<br>
[Static Dynamic Hybrid ISR Rendering](#static-dynamic-hybrid-isr-rendering)<br>
[RSC Rendering](#rsc-rendering)<br>
[Composition Pattern rendering ](#composition-pattern)<br>
[Cache fetching time to get data to the child to performance ](#catch-fetching-time-to-get-data)<br>
[Use environment variables at server ](#env-at-server)<br>
[Use environment variables at client ](#env-at-client)<br>
[Font Optimization](#font-optimization)<br>
[Meta Data ](#meta-data)<br>
[MongoDB Database Reference ](#mongodb-database)<br>

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
  setTasks([...tasksAfterDelete]);
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

`##` How to stop propagation

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
    console.log(movie);
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

`##` How to use context api

## context-api

```javascript

// make a folder at src folder called context and a index.js file it it  like below
/* eslint-disable react-hooks/rules-of-hooks */
import { createContext } from "react";


const MovieContext = createContext();


export {MovieContext};




// provide data to necessary   child
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

`##` how to implement dark theme

## dark-theme

```javascript
// create a a theme context at context folder's index.js file like below
/* eslint-disable react-hooks/rules-of-hooks */
import { createContext } from "react";


const MovieContext = createContext();
const ThemeContext = createContext();


export {MovieContext, ThemeContext};



// Wrap the pages by context provider like below
import { useState } from "react";
import { MovieContext, ThemeContext } from "./context";
import Page from "./Page";

function App() {
  const [cartData, setCartData] = useState([]);
  const [darkMode, setDarkMode] = useState(true);
  return (
    <>
      <ThemeContext.Provider value={{ darkMode, setDarkMode }}>
        <MovieContext.Provider value={{ cartData, setCartData }}>
          <Page />
        </MovieContext.Provider>
      </ThemeContext.Provider>
    </>
  );
}

export default App;


// config tailwind like below
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  darkMode: "class",// We have to add this
  theme: {
		extend: {
			container: {
				center: true,
				padding: "1.25rem",
			},
			colors: {
				primary: '#00D991',
				dark: "#171923",
				light: "#fff",
				body: "#1D1E28"
			},
		},
	},
  plugins: [],
}


// Add dynamic classes to the pages parent div like below
import { useContext } from "react";
import Footer from "./Footer";
import MovieList from "./MovieList";
import NavBar from "./NavBar";
import SideBar from "./SideBar";
import { ThemeContext } from "./context";

const Page = () => {
  const { darkMode } = useContext(ThemeContext);

  return (
    <div className={`h-full w-full ${darkMode ? "dark" : ""}`}> {/*add classes here*/}
      <NavBar />
      <main>
        <div className="container grid lg:grid-cols-[218px_1fr] gap-[3.5rem]">
          <SideBar />
          <MovieList />
        </div>
      </main>
      <Footer />
    </div>
  );
};

export default Page;
```

`##` how to use useReducer

## use-reducer

```javascript
// make a folder called reducer at src and make a file with reducer name example CartReducer.js
// and write the logic with switch case
/* eslint-disable no-unreachable */
const initialState = {
    cartData: [],
}

const cartReducer = (state, action) => {
    switch (action.type){
        case 'ADD_TO_CART':
            return {
                cartData: [...state.cartData, action.payload],
            }
        break;
        case 'REMOVE_FROM_CART':
            return {
                ...state,
                cartData: state.cartData.filter(item => item.id!== action.payload.id)
            }
        break;

        default:
            return state;
    }
}

export {initialState, cartReducer}



// then import  the initialState and cartReducer at parent level
import { useReducer, useState } from "react";
import { MovieContext, ThemeContext } from "./context";
import Page from "./Page";
import { cartReducer, initialState } from "./reducers/CartReducer";

function App() {
  const [darkMode, setDarkMode] = useState(true);
  const [state, dispatch] = useReducer(cartReducer, initialState)
  return (
    <>
      <ThemeContext.Provider value={{ darkMode, setDarkMode }}>
        <MovieContext.Provider value={{ state, dispatch }}>
          <Page />
        </MovieContext.Provider>
      </ThemeContext.Provider>
    </>
  );
}

export default App;


//then use it in different file for add items , delete items , read items and update items
// we can add like this
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
  const { state, dispatch } = useContext(MovieContext);

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
    const found = state.cartData.find((item) => item.id === movie.id);

    if (found) {
      console.log("Movie already in cart!");
      return;
    } else {

     dispatch({
       type: "ADD_TO_CART",
       payload: {
            ...movie
       }
     })
      setShowModal(false);
    }
  };

  return (
    <>
      {showModal && (
        <MovieDetails movie={selectedMovie} onClose={handleCloseMovieDetails} onAddCart={handleAddToCart}/>
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



// We can delete like this
/* eslint-disable react/prop-types */
import { useContext } from "react";
import { MovieContext } from "./context";
import deleteIcon from "../src/assets/delete.svg";
import checkoutIcon from "../src/assets/icons/checkout.svg";
import { getImageUrl } from "./utils/cine-utility";

const ShopingCard = ({ onClose }) => {
  const { state, dispatch } = useContext(MovieContext);
  const handleDeleteCartItem = (cartItem) => {
    dispatch({
      type : 'REMOVE_FROM_CART',

      payload: {...cartItem}
    })
  };

  return (
    <div className="fixed top-0 left-0 w-screen h-screen z-50 bg-black/60 backdrop-blur-sm">
      <div className="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 w-full max-w-[420px] sm:max-w-[600px] lg:max-w-[790px] p-4 max-h-[90vh] overflow-auto">
        <div className="bg-white shadow-md dark:bg-[#12141D] rounded-2xl overflow-hidden p-5 md:p-9">
          <h2 className="text-2xl lg:text-[30px] mb-10 font-bold">
            Your Carts
          </h2>
          <div className="space-y-8 lg:space-y-12 max-h-[450px] overflow-auto mb-10 lg:mb-14">
            {state.cartData.map((cartItm) => (
              <div
                key={cartItm.key}
                className="grid grid-cols-[1fr_auto] gap-4"
              >
                <div className="flex items-center gap-4">
                  <img
                    className="rounded overflow-hidden"
                    src={getImageUrl(cartItm?.cover)}
                    alt=""
                    width={"50px"}
                    height={"50px"}
                  />
                  <div>
                    <h3 className="text-base md:text-xl font-bold">
                      {cartItm?.title}
                    </h3>
                    <p className="max-md:text-xs text-[#575A6E]">
                      {cartItm?.genre}
                    </p>
                    <span className="max-md:text-xs">${cartItm?.price}</span>
                  </div>
                </div>
                <div className="flex justify-between gap-4 items-center">
                  <button
                    onClick={() => handleDeleteCartItem(cartItm)}
                    className="bg-[#D42967] rounded-md p-2 md:px-4 inline-flex items-center space-x-2 text-white"
                  >
                    <img className="w-5 h-5" src={deleteIcon} alt="" />
                    <span className="max-md:hidden">Remove</span>
                  </button>
                </div>
              </div>
            ))}

            {state.cartData.length === 0 && (
              <p className="text-center text-sm text-[#575A6E]">
                No items in your cart. Please add some item
              </p>
            )}
          </div>
          <div className="flex items-center justify-end gap-2">
            {state.cartData.length > 0 && (
              <a
                className="rounded-md p-2 md:px-4 inline-flex items-center space-x-2 bg-primary text-[#171923] text-sm"
                href="#"
              >
                <img src={checkoutIcon} width="24" height="24" alt="" />
                <span>Checkout</span>
              </a>
            )}
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
  );
};

export default ShopingCard;
```

`##` how to use react toastify

## react-toastify

```javascript
//install the package and css at parent level like this
npm install --save react-toastify

// Import the ToastContainer and css  and keep near the parent like this
import { useReducer, useState } from "react";
import { MovieContext, ThemeContext } from "./context";
import Page from "./Page";
import { cartReducer, initialState } from "./reducers/CartReducer";
import { ToastContainer } from "react-toastify";
import 'react-toastify/dist/ReactToastify.css';

function App() {
  const [darkMode, setDarkMode] = useState(true);
  const [state, dispatch] = useReducer(cartReducer, initialState)
  return (
    <>
      <ThemeContext.Provider value={{ darkMode, setDarkMode }}>
        <MovieContext.Provider value={{ state, dispatch }}>
          <Page />
          <ToastContainer/>
        </MovieContext.Provider>
      </ThemeContext.Provider>
    </>
  );
}

export default App;

// Now use it where necessary
// first we need to import the toast
import { toast } from "react-toastify";

const MovieCard = ({ movie }) => {


  const handleAddToCart = (e, movie) => {
    e.stopPropagation();
    const found = state.cartData.find((item) => item.id === movie.id);

    if (found) {

      toast.error(`The movie ${movie?.title} Already in the cart`, {
        position: "bottom-right",
        autoClose: 5000,
        hideProgressBar: false,
        closeOnClick: true,
        pauseOnHover: true,
        draggable: true,
        progress: undefined,
      });
      return;
    } else {

     dispatch({
       type: "ADD_TO_CART",
       payload: {
            ...movie
       }
     })
      setShowModal(false);
      // toast.success(`Added the movie ${movie?.title} successfully`);
      toast.success(`Added the movie ${movie?.title} successfully`, {
        position: "bottom-right",
        autoClose: 5000,
        hideProgressBar: false,
        closeOnClick: true,
        pauseOnHover: true,
        draggable: true,
        progress: undefined,
      });

    }
  };

  return (
    <>
      {/* other code */}
    </>
  );
};

export default MovieCard;
```

`##` Open weather link

## open-weather-map

- [Open weather](https://openweathermap.org/current)

`##` How to set .env variables and import

## env-setting

```javascript
//create a new Environment file called .env at root file where package.json exists
// take necessary parameters here like bellow

VITE_WEATHERE_API_KEY = d2944e3de3b546d31c0f9d21c14d4afb

// client side env must start with VITE_

// Ignore .env at gitIgnore like below
node_modules
dist
dist-ssr
*.local
.env

//Import necessary parameters here like bellow where necessary
 const response = await fetch(`https://api.openweathermap.org/data/2.5/weather?lat=${latitude}&lon=${longitude}&appid=${import.meta.env.VITE_WEATHERE_API_KEY}&units=metric`)

```

`##` How to create a custom hook and how to use it with context api composition pattern

## custom-hook

```javascript
 // create a  folder at src called uesWeather or any other name start with the word use
 // a example of  custom hook given below
 import { useEffect } from "react";
import { useState } from "react";


const useWeather = () => {
    const [weatherData, setWeatherData] = useState({
        location: "",
        climate: "",
        temperature: "",
        maxTemperature: "",
        minTemperature: "",
        humidity: "",
        cloudPercentage: "",
        wind: "",
        time: "",
        latitude: "",
        longitude: "",
    });
    const[loading, setLoading] = useState({
        state: false,
        message: "",
    })
    const [error, setError] = useState(null);

    const featchWeatherData = async (latitude, longitude) => {
        try {
            setLoading({
                state: true,
                message: "Fetching weather data..."
            })

            const response = await fetch(`https://api.openweathermap.org/data/2.5/weather?lat=${latitude}&lon=${longitude}&appid=${import.meta.env.VITE_WEATHERE_API_KEY}&units={metric}`)
            if(!response.ok) {
                const errorMessage = `Fetching weather data failed: ${response.status}`;
                throw new Error(errorMessage)
            }

            const data = await response.json();

            const updateWeatherData = {
                ...weatherData,
                location: data?.name,
                climate: data?.weather[0]?.description,
                temperature: data?.main?.temp,
                maxTemperature: data?.main?.temp_max,
                minTemperature: data.main.temp_min,
                humidity: data?.main?.humidity,
                cloudPercentage: data?.clouds?.all,
                wind: data?.wind?.speed,
                time: data?.dt,
                latitude: latitude,
                longitude: longitude,
            }

            setWeatherData(updateWeatherData);


        } catch (e) {
            setError(e.message);

        }finally{
            setLoading({
                state: false,
                message: ""
            })

        }
    }

    useEffect(() => {
        setLoading({
            loading: true,
            message: "Fetching weather data..."
        })
        navigator.geolocation.getCurrentPosition((position) =>{
            featchWeatherData(position.coords.latitude, position.coords.longitude)
        })

    }, [])

    return {weatherData, loading, error}
}

export default useWeather;

// then create a new file at hooks folder and create a new file called index.js to export multiple hook from one file. like this:
import useWeather from "./useWeather";

export {useWeather}

//use anywhere like below (simple pattern)
import { useWeather } from "./hooks";

const WeatherBoard = () => {
  const {weatherData, loading, error} = useWeather()
  console.log(weatherData, loading, error)
  return (
    <main>
      {/*other code */}
    </main>
  );
};

export default WeatherBoard;

// use by context api with React composition pattern
// steps for composition pattern
// step 1: create folder at src called context inside this create a file called index.js, and create a context one and export it like below
import { createContext } from "react";

const WeatherContext = createContext("")

export { WeatherContext }

// step 2: create a folder at src called provider an create a file called WeatherProvider.jsx , file name will be as per file type
// make a provider like below
import { WeatherContext } from "../context";
import { useWeather } from "../hooks";

const WeatherProvider = ({children}) => {
    const {weatherData, loading, error} = useWeather()
  return (
    <WeatherContext.Provider value={{weatherData, loading, error}}>
      {children}
    </WeatherContext.Provider>
  );
};

export default WeatherProvider;

//Then make a file called index.js at Provider folder
// call and export the WeatherProvider like below
import WeatherProvider from "./WeatherProvider";

export { WeatherProvider}

// step 3: Wrap all necessary child with this provider like below
import Header from "./Header";
import WeatherBoard from "./WeatherBoard";
import bodyBg from "../src/assets/body-bg.png";
import { WeatherProvider } from "./provider";

const App = () => {
  return (
    <WeatherProvider>
      <div
        className="bg-body font-[Roboto] text-light bg-no-repeat bg-cover h-screen grid place-items-center"
        style={{ backgroundImage: `url(${bodyBg})` }}
      >
        <Header />
        <WeatherBoard />
      </div>
    </WeatherProvider>
  );
};

export default App;

// step 4: Then use this data where necessary like below:
// look how conditionally rendered
import { useContext } from "react";
import { WeatherContext } from "./context";

const WeatherBoard = () => {
  const {weatherData} = useContext(WeatherContext)
  console.log(weatherData)
  return (
    <main>
        <section className="">
        <div className="container">
          <div className="grid bg-black/20 rounded-xl backdrop-blur-md border-2 lg:border-[3px] border-white/[14%] px-4 lg:px-14 py-6 lg:py-10 min-h-[520px] max-w-[1058px] mx-auto">
            <div className="grid md:grid-cols-2 gap-10 md:gap-6">
              {loading.state? (
                <p>{loading.message}</p>
              ) : (
                <>
                  <AddToFavourite />
                  <WeatherHeading weatherData={weatherData} />
                  <WeatherCondition />
                </>
              )}
            </div>
          </div>
        </div>
      </section>
    </main>
  );
};

export default WeatherBoard;

```

`##` How to make utility function for formatted date

## formatted-date

```javascript
// create a  folder at src called utils then make a file called date-utils.js and make  the function like below
// data may come like this  :  1726417186
// after use te function output will be like: 10:19 PM- Sunday, September 15, 2024
const getFormattedDate = (value, type, isMS) => {
  if (!type) return;

  if (!isMS) {
    value = value * 1000;
  }

  const date = new Date(value);

  let options;

  if (type === "date") {
    options = {
      weekday: "long",
      year: "numeric",
      month: "long",
      day: "numeric",
    };
  } else if (type === "time") {
    options = {
      hour: "numeric",
      minute: "numeric",
    };
  }
  return new Intl.DateTimeFormat("en-us", options).format(date);
};

export { getFormattedDate };

//How to use this  utility function for formatted date
/* eslint-disable react/prop-types */
/* eslint-disable no-unused-vars */

import { getFormattedDate } from "./utils/date-utils";

const WeatherHeading = () => {
  const { weatherData, loading } = useContext(WeatherContext);
  const { climate, location, temperature, time } = weatherData;
  return (
    <div>
      {/* Other codes  */}
      <p className="text-sm lg:text-lg">
        {getFormattedDate(time, "time", false)}-{" "}
        {getFormattedDate(time, "date", false)}
      </p>
    </div>
  );
};

export default WeatherHeading;
```

`##` How to show dynamic icon by an function

## dynamic-icon

```javascript

//import icon in the component where necessary and make and use  a function like below
/* eslint-disable react/prop-types */
/* eslint-disable no-unused-vars */
import Pin from "./assets/pin.svg"
import cloud from "./assets/cloud.svg"
import { useContext } from "react";
import { WeatherContext } from "./context";
import { getFormattedDate } from "./utils/date-utils";
import CloudIcon from "./assets/cloud.svg";
import HazeIcon from "./assets/haze.svg";
import RainIcon from "./assets/rainy.svg";
import ThunderIcon from "./assets/thunder.svg";
import SunnyIcon from "./assets/icons/sunny.svg";
import SnowIcon from "./assets/icons/snow.svg";
const WeatherHeading = () => {
  const { weatherData, loading } = useContext(WeatherContext);
  const { climate, location, temperature, time } = weatherData;

  function getWeatherIcon(climate) {
    switch (climate) {
        case "Rain":
            return RainIcon;
        case "Clouds":
            return CloudIcon;
        case "Clear":
            return SunnyIcon;
        case "Snow":
            return SnowIcon;
        case "Thunder":
            return ThunderIcon;
        case "Fog":
            return HazeIcon;
        case "Haze":
            return HazeIcon;
        case "Mist":
            return HazeIcon;

        default:
            return SunnyIcon;
    }
}
  return (
    <div>
      <div className="max-md:flex items-center justify-between md:-mt-10">
        <img src={getWeatherIcon(climate)} alt="cloud" />
        {/* other code*/}
  );
};

export default WeatherHeading;

```

`##` How to add and remove something from local storage by ,custom hook, context api and provider

## local-storage-provider-context

```javascript
//create a folder at src called hooks, and make a file called useLocalStorage.js and code like below
import { useEffect, useState } from "react"

const useLocalStorage = (storageKey, defaultValue) => {
    const [value, setValue] = useState(
        JSON.parse(localStorage.getItem(storageKey)) ?? defaultValue);

        useEffect(() => {
            localStorage.setItem(storageKey, JSON.stringify(value));
        }, [value, storageKey]);

    return [value, setValue];
}

export default useLocalStorage;





//then create a file called index.js and code like below
import useWeather from "./useWeather";
import useLocalStorage from "./useLocalStorage";

export {useWeather, useLocalStorage}





//then create a folder at src called context and make a file called index.js and make a context like below
import { createContext } from "react";

const WeatherContext = createContext("")
const FavouriteContext = createContext("")

export { WeatherContext, FavouriteContext }





//then create a folder at src called Provider and make a file called FavouriteProvider.jsx and make a Provider  like below
//We can extend the features like add and remove by the Provider
import { WeatherContext } from "../context";
import { useWeather } from "../hooks";
import { FavouriteContext } from "../context";
import { useLocalStorage } from "../hooks";

const FavouriteProvider = ({children}) => {
    const [ favourites, setFavourites] = useLocalStorage("favourites", [])

    const addToFavorites = (latitude, longitude, location) => {
            setFavourites(
                [...favourites,
                {latitude: latitude, longitude: longitude, location: location}
                ])
    }

    const removeFromFavorites = (location)  => {
        const restFavorites = favourites.filter((fav) =>{
            return fav.location !== location;
        })
        setFavourites(restFavorites);
    }
  return (
    <FavouriteContext.Provider value={{favourites, addToFavorites, removeFromFavorites}}>
        {children}
    </FavouriteContext.Provider>
  );
};

export default FavouriteProvider;





//then create  a file at Provider folder called index.js and export the Provider like below
import WeatherProvider from "./WeatherProvider";
import FavouriteProvider from "./FavouriteProvider";

export { WeatherProvider, FavouriteProvider}





// then wrap the Component at higher level with the Provider like below
import Header from "./Header";
import WeatherBoard from "./WeatherBoard";
import bodyBg from "../src/assets/body-bg.png";
import { FavouriteProvider, WeatherProvider } from "./provider";

const App = () => {
  return (
    <WeatherProvider>
      <FavouriteProvider>
        <div
          className="bg-body font-[Roboto] text-light bg-no-repeat bg-cover h-screen grid place-items-center"
          style={{ backgroundImage: `url(${bodyBg})` }}
        >
          <Header />
          <WeatherBoard />
        </div>
      </FavouriteProvider>
    </WeatherProvider>
  );
};

export default App;





//now we can add and remove item by the Provider like below. Here we used to add and remove location at localStorage
import { useContext, useEffect, useState } from "react";
import { FavouriteContext, WeatherContext } from "./context";
import HeartIcon from "./assets/heart.svg"
import RedHeartIcon from "./assets/heart-red.svg"

const AddToFavourite = () => {
  const {favourites, addToFavorites, removeFromFavorites} = useContext(FavouriteContext);
  const {weatherData} = useContext(WeatherContext)
  const {latitude, longitude, location} = weatherData;
  const [isFavourite, toggleFavourite] = useState(false)


  useEffect(() => {
    const found  = favourites.find((fav) => fav.location === location);
      toggleFavourite(found);

  } , [])

  const handleFavourites = () => {
    const found  = favourites.find((fav) => fav.location === location);

    if(!found){
      addToFavorites(latitude, longitude, location);
    } else {
      removeFromFavorites(location)
    }
    toggleFavourite(!isFavourite);
  }

  return (
    <div className="md:col-span-2">
      <div className="flex items-center justify-end space-x-6">
        <button onClick={handleFavourites} className="text-sm md:text-base inline-flex items-center space-x-2 px-3 py-1.5 rounded-md bg-[#C5C5C54D]">
          <span>Add to Favourite</span>
          <img src={isFavourite ? RedHeartIcon : HeartIcon} alt="" />
        </button>
      </div>
    </div>
  );
};

export default AddToFavourite;
```

`##` How to send value to a hook

## send-value-to-provider

```javascript
// First we need to make a provider for location like below
/* eslint-disable react/prop-types */
import { useState } from "react";
import { LocationContext } from "../context";

const LocationProvider = ({children}) => {
    const [selectedLocation, setSelectedLocation] = useState({
      location: "",
      latitude: 0,
      longitude: 0,
    });
  return (
    <LocationContext.Provider value={{selectedLocation, setSelectedLocation }}>
      {children}
    </LocationContext.Provider>
  );
};

export default LocationProvider;



// Then we have to wrap other component like below with the location context, we already know how to make a context . That's why we have not show it here
import Header from "./Header";
import WeatherBoard from "./WeatherBoard";
import bodyBg from "../src/assets/body-bg.png";
import {FavouriteProvider, LocationProvider, WeatherProvider} from "./provider";

const App = () => {
  return (
    <LocationProvider>
      <WeatherProvider>
        <FavouriteProvider>
          <div
            className="bg-body font-[Roboto] text-light bg-no-repeat bg-cover h-screen grid place-items-center"
            style={{ backgroundImage: `url(${bodyBg})` }}
          >
            <Header />
            <WeatherBoard />
          </div>
        </FavouriteProvider>
      </WeatherProvider>
    </LocationProvider>
  );
};

export default App;



//Then we need to modify the hook
import { useContext, useEffect } from "react";
import { useState } from "react";
import { LocationContext } from "../context";


const useWeather = () => {
    const [weatherData, setWeatherData] = useState({
        location: "",
        climate: "",
        temperature: "",
        maxTemperature: "",
        minTemperature: "",
        humidity: "",
        cloudPercentage: "",
        wind: "",
        time: "",
        latitude: "",
        longitude: "",
    });
    const[loading, setLoading] = useState({
        state: false,
        message: "",
    })
    const {selectedLocation} = useContext(LocationContext) //here we get the location by context

    const [error, setError] = useState(null);

    const fetchWeatherData = async (latitude, longitude) => {
        try {
            setLoading({
                state: true,
                message: "Fetching weather data..."
            })

            const response = await fetch(`https://api.openweathermap.org/data/2.5/weather?lat=${latitude}&lon=${longitude}&appid=${import.meta.env.VITE_WEATHERE_API_KEY}&units=metric`)
            if(!response.ok) {
                const errorMessage = `Fetching weather data failed: ${response.status}`;
                throw new Error(errorMessage)
            }

            const data = await response.json();

            const updateWeatherData = {
                ...weatherData,
                location: data?.name,
                climate: data?.weather[0]?.description,
                temperature: data?.main?.temp,
                maxTemperature: data?.main?.temp_max,
                minTemperature: data.main.temp_min,
                humidity: data?.main?.humidity,
                cloudPercentage: data?.clouds?.all,
                wind: data?.wind?.speed,
                time: data?.dt,
                latitude: latitude,
                longitude: longitude,
            }

            setWeatherData(updateWeatherData);


        } catch (e) {
            setError(e.message);

        }finally{
            setLoading({
                state: false,
                message: ""
            })
        }
    }

    useEffect(() => {
        setLoading({
            loading: true,
            message: "Fetching weather data..."
        })

        //here we added a condition to fetch weather data
        if(selectedLocation.longitude && selectedLocation.latitude) {
            fetchWeatherData(selectedLocation?.latitude, selectedLocation?.longitude)
        } else {
            navigator.geolocation.getCurrentPosition((position) =>{
                fetchWeatherData(position.coords.latitude, position.coords.longitude)
            })
        }
        return
    }, [selectedLocation.longitude, selectedLocation.latitude]) //here we render again if the longitude an latitude has changed

    return {weatherData, loading, error}
}

export default useWeather;
```

`##` How to use useDebounce

## how-to-use-debounce

```javascript
//make a file at hooks folder called "useDebounce"
// make a debounce function like bellow
import { useState, useEffect } from 'react';

function useDebounce(value, delay) {
  const [debouncedValue, setDebouncedValue] = useState(value);

  useEffect(() => {
    const handler = setTimeout(() => {
      setDebouncedValue(value);
    }, delay);

    return () => {
      clearTimeout(handler);
    };
  }, [value, delay]);

  return debouncedValue;
}

export default useDebounce;




// then we can use it where necessary like bellow
import React, { useState, useEffect } from 'react';
import useDebounce from './useDebounce';

function SearchComponent() {
  const [searchTerm, setSearchTerm] = useState('');
  const debouncedSearchTerm = useDebounce(searchTerm, 500); // 500ms delay

  useEffect(() => {
    if (debouncedSearchTerm) {
      // Call your API or perform the desired action
      console.log('Searching for:', debouncedSearchTerm);
    }
  }, [debouncedSearchTerm]);

  return (
    <input
      type="text"
      placeholder="Search..."
      value={searchTerm}
      onChange={(e) => setSearchTerm(e.target.value)}
    />
  );
}

export default SearchComponent;
```

`##` React Router Dom

## react-router-dom

- [React Router Dom](https://github.com/Learn-with-Sumit/rnext/tree/5.1/src)

`##` React Hook Form

## react-hook-form

- [React Hook Form](https://github.com/Learn-with-Sumit/rnext/tree/5.4)

`##` Fetching Data With Axios

## axios-data-fetching

- [Data Fetching With Axios](https://github.com/Learn-with-Sumit/rnext/tree/5.2/src)

`##` State management with TansStackQuery and Fetching Data With Axios

## tans-stack-query-fetching-with-axios

- [Data Fetching With Axios and TansStackQuery](https://github.com/Learn-with-Sumit/rnext/tree/5.3)

`##` Suspense and Error Boundaries

## react-suspense

- [Suspense and Error Boundaries](https://github.com/Learn-with-Sumit/rnext/tree/5.5)

`##` React Lazy Load

## lazy-load

- [React Lazy Load](https://github.com/Learn-with-Sumit/rnext/tree/5.6)

`##` Framer Motion

## framer-motion

- [Framer Motion](https://github.com/Learn-with-Sumit/rnext/tree/5.7)

`##` Firebase Authentication

## firebase

- [Firebase Authentication](https://github.com/Learn-with-Sumit/rnext/tree/5.8)

`##` React Infinite Scroll

## infinite-scroll

- [React Infinite Scroll](https://github.com/Learn-with-Sumit/rnext/tree/5.9)

`##` React Styled Component

## styled-component

- [React Styled Component](https://github.com/Learn-with-Sumit/rnext/tree/5.11)

`##` React Virtualized

## react-virtualized

- [React Virtualized](https://github.com/Learn-with-Sumit/rnext/tree/5.12)

`##` React Portal

## react-portal

- [React Portal](https://github.com/Learn-with-Sumit/rnext/tree/5.13)

`##` React Redux

## react-redux

- [React Redux](https://github.com/Learn-with-Sumit/rnext/tree/5.14)

`##` Tailwind Custom Class

## tailwind-custom-class

- [Tailwind Custom Class index.css](https://github.com/Learn-with-Sumit/rnext/blob/5.15/src/index.css)
- [Tailwind Custom Class tailwind.config](https://github.com/Learn-with-Sumit/rnext/blob/5.15/tailwind.config.js)

`##` Private Route

## private-route

- [PrivateRoutes at routes folder](https://github.com/Learn-with-Sumit/rnext/blob/5.17/src/routes/PrivateRoutes.jsx)
- [Wrap Routes which are private](https://github.com/Learn-with-Sumit/rnext/blob/5.17/src/App.jsx)
- [Make auth empty at Logout component](https://github.com/Learn-with-Sumit/rnext/blob/5.17/src/components/auth/Logout.jsx)

`##` Store user info at state by api call

## store-data-by-api-call

- [Store User Data By API Call](https://github.com/Learn-with-Sumit/rnext/blob/5.18/src/components/auth/LoginForm.jsx)

`##` JWT Implementation

## jwt-implementation

- [Create a wrapper of axios api folder](https://github.com/Learn-with-Sumit/rnext/blob/5.18/src/api/index.js)
- [Create a useAxios Hook](https://github.com/Learn-with-Sumit/rnext/blob/5.18/src/hooks/useAxios.js)
- [Example of use: Make a call using this api from useAxios to get profile](https://github.com/Learn-with-Sumit/rnext/blob/5.18/src/pages/ProfilePage.jsx)

`##` Use Reducer Advanced

## useReducer-advanced

- [Actions In Another file](https://github.com/Learn-with-Sumit/rnext/blob/5.19/src/actions/index.js)
- [Create the Reducer](https://github.com/Learn-with-Sumit/rnext/blob/5.19/src/reducers/ProfileReducer.js)
- [Make a context](https://github.com/Learn-with-Sumit/rnext/blob/5.19/src/context/index.js)
- [Make a provider](https://github.com/Learn-with-Sumit/rnext/blob/5.19/src/providers/ProfileProvider.jsx)
- [Make a hook](https://github.com/Learn-with-Sumit/rnext/blob/5.19/src/hooks/useProfile.js)
- [Use it where need](https://github.com/Learn-with-Sumit/rnext/blob/5.19/src/pages/ProfilePage.jsx)
- [Another use case at Change Bio ](https://github.com/Learn-with-Sumit/rnext/blob/5.19/src/components/profile/Bio.jsx)

`##` Use Reducer Advanced

## multipart-image-upload

- [Multipart Image Upload ](https://github.com/Learn-with-Sumit/rnext/blob/5.19/src/components/profile/ProfileImage.jsx)

`##` How to make reuseable components

## reuseable-components

- [Reuseable components in For Profile ](https://github.com/Learn-with-Sumit/rnext/blob/5.20/src/components/profile/MyPosts.jsx)
- [Reuseable components in For Home ](https://github.com/Learn-with-Sumit/rnext/blob/5.21/src/pages/HomePage.jsx)

`##` Get Difference from now utility function

## get-difference-from-now

- [Get Difference from now utility function ](https://github.com/Learn-with-Sumit/rnext/blob/5.20/src/utils/index.js)

`##` Check the avatar of mine or others

## check-isme-avatar

- [Check the avatar of mine or others ](https://github.com/Learn-with-Sumit/rnext/blob/5.20/src/hooks/useAvatar.js)

`##` New User Registration

## new-user-registration

- [New User Registration](https://github.com/Learn-with-Sumit/rnext/blob/5.22/src/components/auth/RegistrationForm.jsx)

`##` Implement Like with api call

## implement-like-with-api

- [Implement Link with api call](https://github.com/Learn-with-Sumit/rnext/blob/5.23/src/components/posts/PostAction.jsx)

`##` Implement Comments with api call

## implement-comments-with-api

- [Implement Comments with api call](https://github.com/Learn-with-Sumit/rnext/blob/5.23/src/components/posts/PostComments.jsx)

`##` Implement Comments with api call

## implement-delete-with-api

- [Implement Delete with api call](https://github.com/Learn-with-Sumit/rnext/blob/5.24/src/components/posts/PostHeader.jsx)

`##` Implement create with api call

## implement-create-with-api

- [Implement create with api call](https://github.com/Learn-with-Sumit/rnext/blob/5.24/src/components/posts/PostEntry.jsx)

`##` Next js Installation

## nextjs-installation

```javascript
npx create-next-app@latest
```

`##` Next js Basic Setup in Installation time

## nextjs-basic-setup

- [Next js Basic Setup in Installation time](https://prnt.sc/Ga4NfPbGUk4a)

`##` How to make custom link so that it become a client component

## custom-link

- [Component Part](https://github.com/Learn-with-Sumit/rnext/blob/7.6/app/components/CustomLink.js)
- [Uses Part](https://github.com/Learn-with-Sumit/rnext/blob/7.6/app/layout.js)

`##` How to make custom Programmatically navigate

## programmatically-naviagte

- [Component Part](https://github.com/Learn-with-Sumit/rnext/blob/7.6/app/components/Button.js)
- [Uses Part](https://github.com/Learn-with-Sumit/rnext/blob/7.6/app/dashboard/settings/page.js)

`##` How to set meta data

## set-meta-data

- [Set Meta Data like this](https://github.com/Learn-with-Sumit/rnext/blob/7.6/app/dashboard/analytics/page.js)

`##` How to get active link

## get-active-link

- [How to get active link](https://github.com/Learn-with-Sumit/rnext/blob/7.6/app/components/CustomLink.js)

`##` How to get search params

## get-search-params

- [How to get search params](https://github.com/Learn-with-Sumit/rnext/blob/7.6/app/components/SortProducts.js)
- [Uses](https://github.com/Learn-with-Sumit/rnext/blob/7.6/app/dashboard/settings/page.js)

`##` Add loading at nextjs

## add-loading-at-nextjs

- [Add loading at nextjs](https://github.com/Learn-with-Sumit/rnext/tree/7.7/app/heavy)
- [Custom Loading state to part](https://github.com/Learn-with-Sumit/rnext/blob/7.7/app/heavy/page.js)

`##` Show Error In Next js

## show-errors-at-nextjs

Error Comments must be a client component

- [Add a error page at Component Boundary](https://github.com/Learn-with-Sumit/rnext/blob/7.8/app/dashboard/error.js)
- [Now it can catch server component and Client Component error](https://github.com/Learn-with-Sumit/rnext/blob/7.8/app/dashboard/analytics/page.js)

`##` Route Group

## add-route-group

- [How to add a route group](<https://github.com/Learn-with-Sumit/rnext/tree/7.9/app/(dashboard)>)

`##` How to add More than one RootLayout

## add-more-than-one-root-layout

```javascript
In Next.js, you can use more than one Root Layouts by taking advantage of Route Groups and the layout.js file. Each layout.js file defines a layout for a specific segment or section of your application. By strategically organizing your app directory, you can create and apply multiple layouts for different parts of your app.

app/
├── (admin)/
│   ├── layout.js         // Layout for the "admin" section
│   ├── dashboard/
│   │   └── page.js       // /dashboard
│   ├── settings/
│       └── page.js       // /settings
├── (marketing)/
│   ├── layout.js         // Layout for the "marketing" section
│   ├── home/
│   │   └── page.js       // /home
│   ├── about/
│       └── page.js       // /about
├── layout.js             // Global Root Layout
└── page.js               // Home page (root URL /)

```

`##` How to add dynamic routes

## dynamic-routes

- [How to add dynamic routes -main page](https://github.com/Learn-with-Sumit/rnext/blob/7.10/app/blogs/page.js)
- [How to add dynamic routes -child page](https://github.com/Learn-with-Sumit/rnext/blob/7.10/app/blogs/%5Bid%5D/page.js)

`##` How to get ReadMe files content

## readme-file-content

- [How to get ReadMe files content](https://github.com/Learn-with-Sumit/rnext/blob/7.11/docucraft/lib/doc.js)

`##` How to filter for pathname

## filter-for-pathname

- [How to filter for pathname](https://github.com/Learn-with-Sumit/rnext/blob/7.12/docucraft/components/Sidebar.jsx)

`##` DocuCraft full Resource

## docucraft-full-Resource

- [DocuCraft full Resource](https://github.com/Learn-with-Sumit/rnext/tree/7.13/docucraft)

`##` Implement Search In advanced way

## implement-search-advanced-way

Here need to check how onClick is implemented for Link specially in closeSearchResults function at Search Component (Most Important)

- [Implement Search In advanced way-Search Component](https://github.com/Learn-with-Sumit/rnext/blob/7.13/docucraft/components/Search.jsx)
- [Implement Search In advanced way-Search Result Component](https://github.com/Learn-with-Sumit/rnext/blob/7.13/docucraft/components/SearchResult.jsx)

`##` Error handling at real life project

## error-handling-at-real-project

- [Error handling at real life project](https://github.com/Learn-with-Sumit/rnext/blob/7.13/docucraft/app/layout.js)

`##` Parallel Routes

## parallel-routes

- [Parallel Routes](https://github.com/Learn-with-Sumit/rnext/tree/8.2)

`##` Unmatched and intercepting routes

## unmatched-and-intercepting-routes

- [Unmatched and intercepting routes](https://github.com/Learn-with-Sumit/rnext/tree/8.3)

`##` Parallel, unmatched and Intercepting Routes combination

## parallel-and-intercepting-routes-combination

- [Parallel, unmatched and Intercepting Routes combination](https://github.com/Learn-with-Sumit/rnext/tree/8.4)

`##` Route Handlers(CRUD)

## route-handlers

- [ Route Handlers(CRUD)](https://github.com/Learn-with-Sumit/rnext/tree/8.5)

`##` Route Handlers(Search Params, cookies, caching , Redirecting)

## search-params-cookies-caching-redirecting

- [ Route Handlers(Search Params, cookies, caching, Redirecting)](https://github.com/Learn-with-Sumit/rnext/tree/8.6)

`##` Middleware

## middleware

- [ Middleware](https://github.com/Learn-with-Sumit/rnext/tree/8.7)

`##` Next Js Not Found Page

## next-js-not-found-page

- [ Next Js Not Found Page](https://github.com/Learn-with-Sumit/rnext/tree/8.8)

`##` Internalization

## internalization

- [ Internalization](https://github.com/Learn-with-Sumit/rnext/tree/8.9)

`##` Basic Setup of photo feed

## basic-photo-feed

- [ Basic Setup of photo feed](https://github.com/Learn-with-Sumit/rnext/tree/8.10)

`##` Api creation in next js

## api-creation-in-next-js

- [ Api creation in next js](https://github.com/Learn-with-Sumit/rnext/tree/8.11)

`##` Internalization Implementation in photo feed

## internalization-at-photo-feed

- [ Internalization Implementation in photo feed](https://github.com/Learn-with-Sumit/rnext/tree/8.12)

`##` Full code of photo feed

## full-code-of-photo-feed

- [ Full code of photo feed](https://github.com/Learn-with-Sumit/rnext/tree/8.14)

`##` How to import data Dynamically

## import-data-dynamically

- [How to import data Dynamically](https://github.com/Learn-with-Sumit/rnext/blob/8.14/photofeed/app/%5Blang%5D/disctionaries.js)

`##` Data fetching, caching, and revalidating techniques in Next.js

## fetching-catching-revalidation

- [Data fetching, caching, and revalidating techniques in Next.js](https://github.com/Learn-with-Sumit/rnext/tree/9.1)
- [ Data Fetching - on the server & client with third-party libraries & route handlers](https://github.com/Learn-with-Sumit/rnext/tree/9.2)

`##` Server Action - Introduction & Example with MongoDB Database

## server-action-with-mongodb

- [ Server Action - Introduction & Example with MongoDB Database](https://github.com/Learn-with-Sumit/rnext/tree/9.3)
- [More Server Action - Introduction & Example with MongoDB Database](https://github.com/Learn-with-Sumit/rnext/tree/9.4)

`##` Data Fetching Patterns and Best Practices - Sequential & Parallel Data Fetching & Progressive Rendering

## sequential-parallel-progressive-rendering

- [Data Fetching Patterns and Best Practices - Sequential & Parallel Data Fetching & Progressive Rendering ](https://github.com/Learn-with-Sumit/rnext/tree/9.5)

`##` Full Next Weather Dashboard

## weather-dashboard

- [Full Next Weather Dashboard](https://github.com/Learn-with-Sumit/rnext/tree/9.12)

`##` Data fetching in the server with fetch

## data-fetching-in-server

- [Data fetching in the server with fetch](https://github.com/Learn-with-Sumit/rnext/tree/9.1)

```javascript
// Good to know know:
// get Request in Next is by default cached.
// To prevent it we need to use cookies like bellow
import getJoke from "@/utils/getJoke";
import RandJoke from "./components/RandomJoke";
import { cookies } from "next/headers";

export default async function Home() {
  const theme = cookies().get("theme");
  const joke = await getJoke();

  return (
    <main className="flex min-h-screen flex-col items-center justify-center p-24 gap-5">
      <h1 className="text-xl">{joke.value}</h1>
      <RandJoke />
    </main>
  );
}
```

`##` Data fetching in the server with fetch at route handler

## data-fetching-in-server-route-handler

- [Data fetching in the server with fetch at route handler](https://github.com/Learn-with-Sumit/rnext/blob/9.1/app/api/posts/route.js)

```javascript
// Good to know know:
// get Request in Next is by default cached.
// To prevent cached  we need to use export const dynamic = "force-dynamic"; like bellow
import getJoke from "@/utils/getJoke";

export const dynamic = "force-dynamic";

export async function GET(request) {
  const posts = await getJoke();

  return Response.json(posts);
}
```

`##` Another way to prevent caching

## another-way-to-prevent-caching

- [Another way to prevent caching](https://github.com/Learn-with-Sumit/rnext/tree/9.1)

```javascript
// Another way to prevent caching
// we have to use cache: 'no-store' like this:

export default async function getJoke() {
  const res = await fetch("https://api.chucknorris.io/jokes/random", {
    cache: "no-store",
  });

  if (!res.ok) {
    throw new Error("Fetch error...");
  }

  return res.json();
}
```

`##` We can Revalidate the fetching

## revalidating-fetching

- [We can Revalidate the fetching](https://github.com/Learn-with-Sumit/rnext/tree/9.1)

```javascript
// We can Revalidate the fetching like this (It is recommended to revalidate for each fetch call)

export default async function getJoke() {
  const res = await fetch("https://api.chucknorris.io/jokes/random", {
    next: {
      revalidate: 10, // 10 seconds
    },
  });

  if (!res.ok) {
    throw new Error("Fetch error...");
  }

  return res.json();
}
```

`##` Revalidation all fetch requests in a page and its child

## revalidating-fetching-for-a-page-and-child

- [Revalidation all fetch requests in a page and its child](https://github.com/Learn-with-Sumit/rnext/tree/9.1)

```javascript
// We can Revalidate the for a page like this
//Good to no if we use revalidation the page render as static
// We no need to revalidate at individual fetch requests like this

export default async function getJoke() {
    const res = await fetch("https://api.chucknorris.io/jokes/random");

    if (!res.ok) {
        throw new Error("Fetch error...");
    }

    return res.json();
}

// We need to revalidate at page like this
import getJoke from "@/utils/getJoke";
import RandJoke from "./components/RandomJoke";

export const revalidate = 10;

export default async function Home() {
    const joke = await getJoke();

    return (
        <main className="flex min-h-screen flex-col items-center justify-center p-24 gap-5">
            <h1 className="text-xl">{joke.value}</h1>
            <RandJoke />
        </main>
    );
}

```

`##` De-Duplication

## de-duplication

- [De-Duplication](https://github.com/Learn-with-Sumit/rnext/tree/9.1)

```javascript
// De Duplication
// Not need to pass props thought both are hitting same api
// here  <RandJoke /> hitting same api  const joke = await getJoke();
import getJoke from "@/utils/getJoke";
import RandJoke from "./components/RandomJoke";

export const revalidate = 10;

export default async function Home() {
  const joke = await getJoke();

  return (
    <main className="flex min-h-screen flex-col items-center justify-center p-24 gap-5">
      <h1 className="text-xl">{joke.value}</h1>
      <RandJoke /> // it is
    </main>
  );
}
```

`##` Caching and Revalidation with Axios

## axios-caching-revalidation

- [Caching and Revalidation with Axios](https://github.com/Learn-with-Sumit/rnext/tree/9.2)

```javascript
  // Manually use cache
 import axios from "axios";
import { cache } from "react";

const getJoke = cache(async () => {
    return axios.get("https://api.chucknorris.io/jokes/random");
});

export default getJoke;


//For Revalidation
import getJoke from "@/utils/getJoke";
import RandJoke from "./components/RandomJoke";

export const revalidate = 10;

export default async function Home() {
    const joke = await getJoke();

    return (
        <main className="flex min-h-screen flex-col items-center justify-center p-24 gap-5">
            <h1 className="text-xl">{joke.value}</h1>
            <RandJoke />
        </main>
    );
}
```

`##` Static Dynamic Hybrid ISR Rendering

## static-dynamic-hybrid-isr-rendering

- [Static Dynamic Hybrid ISR Rendering](https://github.com/Learn-with-Sumit/rnext/tree/10.1)

`##` RSC Rendering

## rsc-rendering

SSG rendering happens in page level,
RSC rendering happens in component level,
In Client Component we can keep Child components as children or send as props but can not import child components,
But we can import client components in server component.

- [RSC Rendering](https://github.com/Learn-with-Sumit/rnext/tree/10.2)

`##` Composition Pattern rendering

## composition-pattern

- [Composition Pattern rendering ](https://github.com/Learn-with-Sumit/rnext/tree/10.3)

`##` Cache fetching time to get data to the child to performance

## catch-fetching-time-to-get-data

```javascript
import connectMongo from "@/dbConnect/connectMongo";
import User from "@/models/User";
import { cache } from "react";

export const getUserByEmail = cache(async (email) => {
  console.log("I am pulling from database");
  try {
    await connectMongo();

    // get users
    const user = await User.findOne({
      email,
    });

    return user;
  } catch (err) {
    console.log(err);
  }
});

//Now if we use the component it will get data from parents
import NewUserForm from "./components/users/NewUserForm";
import User from "./components/users/User";
import UserList from "./components/users/UserList";

export default async function Home() {
  return (
    <div className="py-8">
      <h1 className="text-gray-800">USER REGISTRATION</h1>
      <NewUserForm />
      <User />
      <UserList />
      <User />
      <User />
    </div>
  );
}
```

- [Composition Pattern rendering ](https://github.com/Learn-with-Sumit/rnext/tree/10.3)

`##` Use environment variables at server

## env-at-server

```javascript
DB_HOST = localhost;
DB_USER = myuser;
DB_PASS = mypassword;
```

`##` Use environment variables at client

## env-at-client

```javascript
NEXT_PUBLIC_ANALYTICS_ID=abcdefghijk
```
`##` Font Optimization

## font-optimization
- [Font Optimization](https://github.com/Learn-with-Sumit/rnext/tree/10.5)

`##` Meta Data

## meta-data
- [Meta data ](https://github.com/Learn-with-Sumit/rnext/tree/10.6)

`##` MongoDB Database Reference

## mongodb-database
```javascript
//Steps required to work with MongoDB
// 1.Download the MongoDB 
// 2.Download the MongoDB Compass which is graphical user interface which helps us to manage MongoDB Database easily
// 3.Open MongoDB Compass create database and create collection as per requirements
// 4.Upload json file or create 
// 5. Install mongoose for make model and scheme for crud operation. It is a data modeling tool
// 6.At .env keep the mongodb database url like bellow

MONGO_URI=mongodb://127.0.0.1:27017/Momentous

// 7.Make a folder at root folder called services and make a file in it called mongo.js and make a function to connect to database like bellow
import mongoose from "mongoose";

export async function dbConnect() {
    try{
        const conn = await mongoose.connect(process.env.MONGO_URI);
        console.log("Connected");
        return conn;
    } catch(err){
        console.log(err);
    }
}

//8. Import the function at the top root layout like bellow
import { Inter } from "next/font/google";
import "./globals.css";
import Navbar from "@/components/Navbar";
import { dbConnect } from "@/services/mongo";

const inter = Inter({ subsets: ["latin"] });

export const metadata = {
  title: "Momentous",
  description: "An Event Booking Application",
};

export default async function RootLayout({ children }) {
  await dbConnect();
  return (
    <html lang="en">
      <body className={inter.className}>
        <Navbar />
        <main className="py-8">
          {children}
        </main>
      </body>
    </html>
  );
}
//9. Have to check is it connected or not. If connected we can see "Connected" string though I have consoled it
//10. Then make a folder at root level and make a file in it for model exp: moments-model.js like bellow

import mongoose, {Schema} from "mongoose";

const schema = new Schema({
  name: {
    required: true,
    type: String
  },
  details: {
    required: true,
    type: String
  },
  location: {
    required: true,
    type: String
  },
  imageUrl: {
    required: true,
    type: String
  },
  interested_ids: {
    required: false,
    type: Array
  },
  going_ids: {
    required: false,
    type: Array
  },
  swgs: {
    required: false,
    type: Array
  }
});

export const momentsModel = mongoose.models.moments ?? mongoose.model("moments", schema);

//11. Then a make folder at root called db and make a file called called queries.js and make queries like bellow
import { momentsModel } from "@/models/moments-model";
import { replaceMongoIdInArray, replaceMongoIdInObject } from "@/utils/data-util";

async function getAllMoments() {
    const allMoments = await momentsModel.find().lean();
    return replaceMongoIdInArray(allMoments);
}

async function getMomentById(momentId) {
    const moment = await momentsModel.findById(momentId).lean();
    return replaceMongoIdInObject(event);
}

export {
    getAllMoments,
    getMomentById
}

// 12. Then check it by calling anywhere like bellow:
import { getAllMoments } from "@/db/queries"
import EventCard from "./EventCard"

const EventList = async () => {
  const allMoments =  await getAllMoments();
  console.log(allMoments);
  
  return (
    <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mt-8">
      <EventCard />
    </div>
  )
}

export default EventList


// 14. We can process mongoDb default _id to make it simple "id" by a utility function. For that make file a utility folder called data-util and process like bellow 
import { eventModel } from "@/models/event-models"
import { replaceMongoIdInArray, replaceMongoIdInObject } from "@/utils/data-util";

async function getAllEvents() {
    const allEvents = await eventModel.find().lean();
    return replaceMongoIdInArray(allEvents);
}

async function getEventById(eventId) {
    const event = await eventModel.findById(eventId).lean();
    return replaceMongoIdInObject(event);
}

export {
    getAllEvents,
    getEventById
}

// 15. Then use this utility function like shown at step 11
```
- [MongoDB Database Reference](https://github.com/Learn-with-Sumit/rnext/tree/10.11)
