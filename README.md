# npm-module-webpack-boilerplate
A boilerplate for making npm modules, bundled with webpack and written in ES6.

## Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Clone the repo](#clone-the-repo)
  - [Update package.json](#update-packagejson)
  - [Build your module](#build-your-module)
  - [Test your module](#test-your-module)
  - [Upload your npm module](#upload-your-npm-module)

## Features

* ES6 with Babel
* Bundle with Webpack
* Run tests and tdd with karma in ES6

## Getting Started

### Clone the repo

```
git clone git@github.com:Stychen/npm-module-webpack-boilerplate.git <your-new-repo-name>
cd <your-repo-name>
npm install
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
    
### Upload your npm module

After your done with development of your npm module. You can upload your module in npmjs.com
https://docs.npmjs.com/getting-started/publishing-npm-packages