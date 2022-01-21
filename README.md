//// install Tailwind Css 

====> install tailwind CLI 
commend >>>
1.First create npm project file to commend
$ npm init -y

2.install tailwindcss to commend
$npm i -D tailwindcss

3. config file create
$npx tailwindcss init

/////////////create 2 file and into create to file 

1. src/tailwind.Css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
2.output/tailwind.css
    auto create vanilla css

//////////////ignore error vscode to create a file>

    .vscode/settings.json
      wright code>
        {
            "css.validate": false,
            "tailwindCSS.emmetCompletions": true
        }

/////////////package.json setup to wright code

        {
        "name": "tailwind-first",
        "version": "1.0.0",
        "description": "",
        "main": "index.js",
        "scripts": {
            "build": "tailwindcss -i ./src/input.css -o ./output/style.css -w"
        },
        "keywords": [],
        "author": "",
        "license": "ISC",
        "devDependencies": {
            "tailwindcss": "^3.0.15"
        }
    }

///////////// tailwind.config.js file settings

        module.exports = {
    content: [
        "./components/**/*.{html,js}",
        "./pages/**/*.{html,js}",
        "./index.html",
    ],
    theme: {
        extend: {},
    },
        plugins: [],
    };

///////////// auto css transfer output/output.css file
 command>>>>
 $npm run build