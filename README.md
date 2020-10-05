# UI-Seed
A simple seed project with SASS and BrowserSync

### Uses NPM

Make sure you have latest stable NodeJS and NPM installed.

### Directory Structure and Setup

#### Project Structure

```unicode
.
├── LICENSE - License file
├── README.md - You're reading it right now
├── app - Directory where SourceCode resides.
│   ├── assets - Directory for your assets such as fonts, images etc
│   │   └── temp - Can be any directory though, or any sublevel.
│   │       └── test.img
│   ├── index.html - Basic HTML broilerplate.
│   ├── scripts - No need of this directory name,
│   │   └── main.js -  all it cares about is file to have .js extension
│   ├── styles - no need of this directory name,
│   │   ├── main.scss - It can be .scss
│   │   └── test.css - Or .css
│   └── tests -  this directory consists of tests, tests and specs directories doesn't get minified.
│       └── yourFile.test.js - technically those files can be anywhere as long as they end with .test.js
├── ava.config.js - AVA configuration for testing.
├── babel.config.js - Babel transpilation configuration, consists of plugins used.
├── gulpfile.babel.js - Gulpfile, consist definitions for all the tasks for this project.
├── package-lock.json
├── package.json - NPM instructions and dependecies.
└── test-helpers - Required Helpers for AVA.
    ├── _testHelperBabel.js - Babel required for imports and stuff
    └── _testHelperENV.js - BrowserENV for using JSDOM in testing
```


#### Getting Started

install Node dependencies

`npm i` - Installs the dependencies

Developement

`npm run develop` - Opens Browser Sync live server and watches for file changes, reloads/updates view.

`npm run build` - Generates user deployable code inside `dist` directory.

`npm run build:prod` - Generates Minified build inside `dist` directory.

`npm run test` - Runs AVA test for all the `.test.js` files

