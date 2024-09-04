`##` Make a project

```javascript
npm create vite@latest tic-tac-toe -- --template react
```

`##` Install Tailwind css dependencies

```javascript
npm install -D tailwindcss postcss autoprefixer
```

`##` Initial Tailwind css

```javascript
npx tailwindcss init -p
```

`##` at tailwind.config

```javascript
content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
```

`##` Clean index.css and add below declarations

```javascript
@tailwind base;
@tailwind components;
@tailwind utilities;
```

`##` Add animation using className, at index.css

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

- [How To Handle form In react form code](https://github.com/Learn-with-Sumit/rnext/blob/2.10/src/task/AddTaskModal.jsx)
- [How To Handle form In react parent code](https://github.com/Learn-with-Sumit/rnext/blob/2.10/src/task/TaskBoard.jsx)

`##` Basic Add and edit by same form in an array

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

```javascript
function handleDeleteTask(taskId) {
  const tasksAfterDelete = tasks.filter((task) => task.id !== taskId);
  setTasks(tasksAfterDelete);
}
```

`##` Basic Delete all items

```javascript
function handleDeleteAllClick() {
  tasks.length = 0;
  setTasks([...tasks]);
}
```

`##` Basic Toggle

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
`##` How to  implement sort
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
      cover: book 
    }]
 //Parent's code
  const handleSort =(sortOption) => {
    let sortedBooks = [...books];
    switch (sortOption) {
      case 'name_asc':
        sortedBooks.sort((a, b) => a.title.localeCompare(b.title));
        break;
      case 'name_desc':
        sortedBooks.sort((a, b) => b.title.localeCompare(a.title));
        break;
      case 'year_asc':
        sortedBooks.sort((a, b) => {
          const yearA = new Date(a.publicationDate).getFullYear();
          const yearB = new Date(b.publicationDate).getFullYear();
          return yearA - yearB;
        });
        break;
      case 'year_desc':
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
  }
//child'd code 
/* eslint-disable react/prop-types */
const Sort = ({onSortChange}) => {
  const handleChange = (event) => {
    onSortChange(event.target.value);
    console.log(event.target.value)
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
```javascript
function getAllMovies() {
    return data;// Here data is the array and we can import and call the function in other components
}

export { getAllMovies };
```
`##` How to filter data by a function
```javascript
function getFavoriteMovies() {
    return data.filter(movie => movie.isFavorite); // Here data is the array and we can import and call the function in other components
}

export { getFavoriteMovies };
```