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
`##` set Prettier
```javascript
how to enable prettier format on save in vs code
ChatGPT said:
ChatGPT
To enable Prettier to format your code automatically on save in Visual Studio Code (VS Code), follow these steps:

1. Install the Prettier Extension
Open VS Code.
Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window, or press Ctrl+Shift+X.
In the search bar, type Prettier - Code Formatter and click Install on the extension by Prettier.
2. Configure VS Code to Use Prettier by Default
Open the settings by clicking on the gear icon in the bottom left corner and selecting Settings, or press Ctrl+,.
In the search bar at the top of the settings window, type "format on save".
Check the box for Editor: Format On Save. This will ensure that the code is formatted whenever you save the file.
3. Set Prettier as the Default Formatter
In the settings window, search for "default formatter".
Under Editor: Default Formatter, select esbenp.prettier-vscode from the dropdown list. This sets Prettier as the default formatter.
4. Configure Prettier (Optional)
You can customize Prettier's behavior by creating a .prettierrc configuration file in your project. For example:

json
Copy code
{
  "semi": false,
  "singleQuote": true,
  "tabWidth": 2,
  "trailingComma": "es5"
}
5. Enable Format on Save for Specific Languages (Optional)
If you want to enable Format on Save for specific languages only, you can do so in the settings:

Search for "editor.formatOnSave".
Click Edit in settings.json.
Add settings for specific languages. For example:
json
Copy code
"[javascript]": {
  "editor.formatOnSave": true
},
"[typescript]": {
  "editor.formatOnSave": true
}
6. Save and Restart VS Code
Save your settings and restart VS Code to ensure that all changes take effect.

Now, whenever you save a file, Prettier will automatically format your code according to the rules defined in your configuration.

You said:
how to enable prettier to change class to className on save
ChatGPT said:
ChatGPT
To enable Prettier to automatically change class to className when saving your files in Visual Studio Code, you'll need to use a combination of Prettier and a tool like eslint-plugin-react that enforces React-specific rules, such as using className instead of class.

Here’s how you can set it up:

1. Install Required Packages
First, make sure you have the necessary packages installed in your project:

bash
Copy code
npm install --save-dev eslint eslint-plugin-react prettier eslint-config-prettier eslint-plugin-prettier
2. Create or Update .eslintrc Configuration
Next, create or update your .eslintrc configuration file to include the React plugin and Prettier:

json
Copy code
{
  "env": {
    "browser": true,
    "es2021": true
  },
  "extends": [
    "eslint:recommended",
    "plugin:react/recommended",
    "plugin:prettier/recommended"
  ],
  "parserOptions": {
    "ecmaFeatures": {
      "jsx": true
    },
    "ecmaVersion": "latest",
    "sourceType": "module"
  },
  "plugins": ["react", "prettier"],
  "rules": {
    "prettier/prettier": "error",
    "react/jsx-uses-react": "error",
    "react/jsx-uses-vars": "error",
    "react/no-unknown-property": ["error", { "ignore": ["class"] }]
  },
  "settings": {
    "react": {
      "version": "detect"
    }
  }
}
3. Create or Update .prettierrc Configuration
Ensure you have a .prettierrc file to configure Prettier as needed. This file might include settings such as:

json
Copy code
{
  "semi": false,
  "singleQuote": true,
  "tabWidth": 2,
  "trailingComma": "es5"
}
4. Update VS Code Settings
If you haven't already set up Prettier to format on save, follow the steps outlined in the previous section to enable Format on Save and set Prettier as the default formatter.

5. ESLint Integration with Prettier
Ensure that ESLint is integrated with Prettier so that when you save your files, ESLint checks for class and automatically changes it to className:

Install the ESLint VS Code extension if you haven’t already.

Configure ESLint to fix issues on save. In your VS Code settings (settings.json), add:

json
Copy code
"editor.codeActionsOnSave": {
  "source.fixAll.eslint": true
}
6. Restart VS Code
Finally, save your settings and restart VS Code to ensure everything is applied correctly.

How It Works
When you save a file, Prettier formats the code according to the rules defined in .prettierrc.
ESLint, with the eslint-plugin-react plugin, checks for React-specific issues like using class instead of className and corrects them.
The VS Code setting "source.fixAll.eslint": true ensures that these fixes are applied automatically on save.
With this setup, any time you use class in your JSX, ESLint will automatically change it to className when you save the file.
```