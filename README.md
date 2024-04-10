# react_project_install_steps

## Food Delivery (Project Name)

### Command to Run Project
    1. npx parcel index.html // To run a project
    2. npx jest // To testing a project
    2. npx jest --init // To initialize jest

### To installation of food delivery project in react js there are some steps to follow
    1. Initialize our project folder > "git init" and push on github
        1. echo "# repo_name" >> README.md
        2. git init
        3. git add README.md
        4. git commit -m "first commit"
        5. git branch -M main
        6. git remote add origin https://github.com/rajratnmore/repo_name.git
        7. git push -u origin main
    2. npm init
    3. npm install -D parcel
    4. npm install react
    5. npm install react-dom
    6. npm install react-router-dom
    7. npx parcel build index.html

### To install redux in react project
    1. npm install @reduxjs/toolkit
    2. npm install react-redux
    
### To install tailwindcss in react project
    1. npm install -D tailwindcss
    2. npx tailwindcss init
    3. npm install postcss autoprefixer --save-dev
    4. create file named "postcss.config.js" with the following content into it
            
            module.exports = {
                plugins: [
                require('tailwindcss'),
                require('autoprefixer'),
                ],
            };

    5. Have to following content into file named "index.css"
            
            /* src/styles/tailwind.css */
            @import 'tailwindcss/base';
            @import 'tailwindcss/components';
            @import 'tailwindcss/utilities';

            /* Your custom styles here */

    6. create file named ".postcssrc" with the following content into it
            
            {
                "plugins": {
                    "tailwindcss": {}
                }
            }

    7. Have to following content into file named "tailwind.config.js"
            
            /** @type {import('tailwindcss').Config} */
            module.exports = {
            content: [
                "./src/**/*.{js,jsx,ts,tsx}",
            ],
            theme: {
                extend: {},
                container: {
                center: true,
                padding: '2rem',
                }
            },
            plugins: [],
            }


### To install fontawesome in react project
    1. npm install @fontawesome/free-solid-svg-icons
    2. npm install @fontawesome/react-fontawesome

### Redux Toolkit 
    - Install @reduxjs/toolkit and @react-redux 
        npm install @reduxjs/toolkit
        npm install react-redux
    - Build our store
    - Connect our store to our app
    - Create Slice (cart slice)
    - dispatch (action)
    - Selector

### To install react testing library
    1. npm install -D @testing-library/react
    2. npm install -D jest
    3. npm install --save-dev babel-jest @babel/core @babel/preset-env (To install jest along with babel)
    4. Configure Babel to target your current version of Node by creating a babel.config.js file
       in the root of your project:
        eg. babel.config.js (file name)
            module.exports = {
                presets: [['@babel/preset-env', {targets: {node: 'current'}}]],
            };
    5. Configure Parcel Config file to disable default babel transpilation.
       Create '.parcelrc' file in your root directory and put below code inside this file.
        eg: .parcelrc (file name)
            {
                "extends": "@parcel/config-default",
                "transformers": {
                    "*.{js,mjs,jsx,cjs,ts,tsx}": [
                    "@parcel/transformer-js",
                    "@parcel/transformer-react-refresh-wrap"
                    ]
                }
            }
    6. npx jest // To testing a project
    7. npx jest --init // To initialize jest
    8. If you're using Jest 28 or later, jest-environment-jsdom package now must be installed separately.
        npm install --save-dev jest-environment-jsdom
    9. Install @babel/preset-react - to make JSX work in test cases.
        run this command: npm install --save-dev @babel/preset-react
 
        Go inside 'babel.config.js' file and modify this file from this
            module.exports = {
                presets: [['@babel/preset-env', {targets: {node: 'current'}}]],                
            };

            to this
            module.exports = {
                presets: [
                    ['@babel/preset-env', {targets: {node: 'current'}}],
                    ['@babel/preset-react', {runtime: "automatic"}]
                ],  
            };
    10. npm install -D @testing-library/jest-dom
    
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
    


                

                
