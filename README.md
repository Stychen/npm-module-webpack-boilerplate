# npm-module-webpack-boilerplate
A boilerplate for making npm modules, bundled with webpack and written in ES6.

## Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Clone the repo](#clone-the-repo)
  - [Customize package.json](#customize-packagejson)
  - [Customize the README.md file](#customize-the-readmemd-file)
  - [Build your module](#build-your-module)
  - [Test your module](#test-your-module)

## Features

* ES6 with Babel
* Bundle with Webpack
* Run tests and tdd with karma in ES6

## Getting Started

### Clone the repo

```
git clone git@github.com:Stychen/npm-module-webpack-boilerplate.git <your-new-repo-name>
cd <your-repo-name>
```

### Update package.json

Open up `package.json` and update to your liking.
Important: 
Change `module_name_here` in `package.json` to your module_name.
Also in `webpack.config.js`, change `module_name_here`.



### Build your module

Your module's entry path is at `src\index.js` and the output path is at `lib\<module_name>.min.js`. This can be edited at `webpack.config.js`.

1. For production

  ```sh
  npm run build
  ```

  This will run webpack to bundle minified versions of your library in `./lib` with sourcemaps.


2. For development

  ```sh
  npm start
  ```

  This will run the `webpack` build in watch mode.
  
### Test your module

1. For testing
    ```sh
    npm run test
    ```
    This will run tests in `./test` that are named `**_test.js` (ie: `sample_test.js`). 
   
2. For test driven development
    ```sh
    npm run tdd
    ```
    This will run karma in tdd mode