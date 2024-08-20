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
