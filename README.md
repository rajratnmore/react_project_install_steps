# react_project_install_steps

## food delivery

### To install of food delivery project in React js there are some steps to follow
    1. Initialize our project folder > "git init" and push on GitHub
    2. npm init
    3. npm install -D parcel
    4. npm install react
    5. npm install react-dom
    6. npm install react-router-dom
    7. npx parcel build index.html

### To install redux in react project
    1. npm install @reduxjs/toolkit
    2. npm install @react-redux


### To install tailwindcss in the react project
    1. npm install -D tailwindcss
    2. npx tailwindcss init
    3. npm install postcss autoprefixer --save-dev
    4. create a file named "postcss.config.js" with the following content in it
            
            module.exports = {
                plugins: [
                require('tailwindcss'),
                require('autoprefixer'),
                ],
            };

    5. Have to follow content into a file named "index.css"
            
            /* src/styles/tailwind.css */
            @import 'tailwindcss/base';
            @import 'tailwindcss/components';
            @import 'tailwindcss/utilities';

            /* Your custom styles here */

    6. create a file named ".postcssrc" with the following content in it
            
            {
                "plugins": {
                    "tailwindcss": {}
                }
            }

    7. Have to follow content into a file named "tailwind.config.js"
            
            /** @type {import('tailwindcss').Config} */
            module.exports = {
            content: ["./src/**/*.{js,jsx,ts,tsx}"],
            theme: {
                extend: {},
                container: {
                center: true,
                padding: '2rem',
                }
            },
            plugins: [],
            }


### To install font awesome in react project
    1. npm install @fontawesome/free-solid-svg-icons
    2. npm install @fontawesome/react-fontawesome

### To create a new repository on the command line
    1. echo "# repo_name" >> README.md
    2. git init
    3. git add README.md
    4. git commit -m "first commit"
    5. git branch -M main
    6. git remote add origin https://github.com/rajratnmore/repo_name.git
    7. git push -u origin main

### To push an existing repository from the command line
    1. git remote add origin https://github.com/rajratnmore/repo_name.git
    2. git branch -M main
    3. git push -u origin main
    

                

                
