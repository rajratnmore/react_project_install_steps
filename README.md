# react_project_install_steps

# food delivery

## To installation of food delivery project in react js there are some steps to follow
    1. Initialize our project folder > "git init" and push on github
    2. npm init
    3. npm install -D parcel
    4. npm install react
    5. npm install react-dom
    6. npm install react-router-dom
    7. npx parcel build index.html

## To install tailwindcss in react project
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


## To install fortawesome in react project
    1. npm install @fontawesome/free-solid-svg-icons
    2. npm install @fontawesome/react-fontawesome


                

                
