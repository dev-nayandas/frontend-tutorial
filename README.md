`##` Make a project
```javascript 
npm create vite@latest tic-tac-toe -- --template react
```
`##` Install Tailwind css dependencies
```javascript
npm install -D tailwind css postcss autoprefixer
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
`##` Clean index.css and below declarations
```javascript
@tailwind base;
@tailwind components;
@tailwind utilities;
```
