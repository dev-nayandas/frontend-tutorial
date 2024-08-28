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

`##` Basic Delete Delete all items 
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
        setTasks(tasks.map((task) => {
            if (task.id === taskId) {
                return {...task, isFavorite: !task.isFavorite};
            } else {
                return task;
            }
        }))
    }

```

