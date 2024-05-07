# react_project_install_steps

## webpage design color sites
    1. https://htmlcolorcodes.com/color-picker/
    2. https://tailwindcolor.com/

## Food Delivery (Project Name)

### install some extensions in vs code to auto tailwindcss classes and css classes suggestions
    1. tailwind css intellisense
    2. intellisense for css class names in HTML
    3. Prettier - Code formatter

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

    OR YOU CAN INSTALL REACT PORJECT THROUGH THE COMMAND
        1.  npx create-react-app 'project_name'
        2.  npm install -D react-router-dom

### To install redux in react project

    - Install @reduxjs/toolkit and @react-redux
        1. npm install -D @reduxjs/toolkit
        2. npm install -D react-redux
    
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


### To host react project on firebase
    1. npm install firebase
        2. create 'firebase.js' inside utils folder and paste code which has been given by firebase site just below
            above 'npm install firebase' command
            and also copy two line code in 'firebase.js' file in netflixGPT project only: (Remember below two line put in 'firebase.js' file only in NetflixGPT project.
                1. import { getAuth } from "firebase/auth"; // put this top of firebase.js file
                2. export const auth = getAuth(); // Put this at last line into firebase.js file
            
        3. npm install -g firebase-tools  (To run this command first open your cmd in run as administator mode )
        4. firebase login
        5. firebase init
            1. Are you ready to proceed? (Y/n): Y
            2. (*) Hosting: Configure files for Firebase Hosting and (optionally) set up GitHub Action deploys
            3.  Please select an option: (Use arrow keys)
                > Use an existing project
            4. Select a default Firebase project for this directory:
                > netflixgpt-openai-00 (NetflixGPT)
            5. What do you want to use as your public directory? (public): build
            6. Configure as a single-page app (rewrite all urls to /index.html)? (y/N): No
            7. Set up automatic builds and deploys with GitHub? (y/N): No
        6. npm run build
        7. firebase deploy
        And now you are ready to go your hosted site
    


                

                
