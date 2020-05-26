# Vue, Firebase Portfolio JS Boilerplate

<img src="http://vuejs.org/images/logo.png" height="50"> <img src="https://camo.githubusercontent.com/66747a6e05a799aec9c6e04a3e721ca567748e8b/68747470733a2f2f662e636c6f75642e6769746875622e636f6d2f6173736574732f313336353838312f313931383337332f32653035373166612d376462632d313165332d383436352d3839356632393164343366652e706e67" height="50">

[![Known Vulnerabilities](https://snyk.io/test/github/icebob/vue-express-mongo-boilerplate/badge.svg)](https://snyk.io/test/github/icebob/vue-express-mongo-boilerplate)
![Node 6](https://img.shields.io/badge/node-6.x.x-green.svg)
![VueJS 2](https://img.shields.io/badge/vuejs-2.3.x-green.svg)
![Webpack 2](https://img.shields.io/badge/webpack-2.6.x-green.svg)

This is a front-end webapp boilerplate project with VueJS + Firebase. It is NOT an out-of-box project.
I made it in order to create an up-to-date starter repo which contains all important fields for a portfolio gallery website. So when neccessary I can create a new webapp and only need to upload a new Json to Firebase.

### [Live Demo](https://asherccohen.co.uk/)

## Features

**Client-side**

- [x] **[VueJS 2.x](https://github.com/vuejs/vue)**
- [x] [Vuex](https://github.com/vuejs/vuex)
- [x] [Vue-router](https://github.com/vuejs/vue-router)
- [x] **[Webpack 2](https://github.com/webpack/webpack)**
- [x] [SCSS](http://sass-lang.com/)
- [x] [PostCSS](https://github.com/postcss/postcss) with precss and autoprefixer
- [x] [Babel](https://babeljs.io/).

## Build Setup

```bash
# install dependencies
npm install

# serve with hot reload at localhost:3333
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

Before start, you have to install production dependencies with npm: `npm install`

## Obtaining API keys for social signup/login

![Firebase Logo](data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiA/PjxzdmcgYmFzZVByb2ZpbGU9InRpbnkiIGhlaWdodD0iNTEycHgiIGlkPSJMYXllcl8xIiB2ZXJzaW9uPSIxLjIiIHZpZXdCb3g9IjAgMCA1MTIgNTEyIiB3aWR0aD0iNTEycHgiIHhtbDpzcGFjZT0icHJlc2VydmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiPjxnPjxwYXRoIGQ9Ik0yOTcuMDM2LDIwNS41NzhsLTM2LjMzNCwzMy44MDlsLTMzLjcxNi02OC4wMDVsMTcuNDQ2LTM5LjEwOGM0LjQxNi03Ljg0LDExLjYyMS03Ljg1NSwxNi4wMzcsMCAgIEwyOTcuMDM2LDIwNS41Nzh6IiBmaWxsPSIjRkZBMDAwIi8+PHBvbHlnb24gZmlsbD0iI0Y1N0YxNyIgcG9pbnRzPSIyNjAuNzAyLDIzOS4zODYgMTI0LjkyNCwzNjUuNjk3IDIyNi45ODYsMTcxLjM4MSAgIi8+PHBhdGggZD0iTTMzNi43NzYsMTUzLjkwMWM2LjQ5MS02LjIzOSwxMy4yMDItNC4xMTEsMTQuOTEyLDQuNzI5bDM1LjM0MiwyMDUuMzc1TDI2OS44NzMsNDM0LjIyICAgYy00LjEsMi4yNjQtMTQuOTU3LDMuMjQ2LTE0Ljk1NywzLjI0NnMtOS45MS0xLjE4NS0xMy42ODctMy4yODFMMTI0LjkyLDM2NS42OUwzMzYuNzc2LDE1My45MDF6IiBmaWxsPSIjRkZDQTI4Ii8+PHBhdGggZD0iTTIyNi45ODYsMTcxLjM4MUwxMjQuOTI0LDM2NS42OTdsNDUuNDYtMjgzLjk5OGMxLjY3NC04Ljg0Nyw2LjcxLTkuNjk5LDExLjIwMy0xLjg5TDIyNi45ODYsMTcxLjM4MXoiIGZpbGw9IiNGRkEwMDAiLz48L2c+PC9zdmc+)

These are the instructions for Firebase:

- Visit [Firebase Console](https://firebase.google.com/)
- Click on the **Go to console** button
- Click on the **Create Project** button
- Enter _Project Name_, then click on **Create** button
- Then click on _Database_ in the sidebar
- Click on **Import JSON** and select your JSON file from ./src/api/app.json
- Next, under _Settings_ in the sidebar
- Click on **Add to a web app** button
- Copy and paste the _script_ keys into `./src/api/firebase-conf.js` file

## License

This repo is available under the [MIT license](https://tldrlegal.com/license/mit-license).

## Contact

Copyright (C) 2016 Snake

[![@asherccohen](https://img.shields.io/badge/github-asherccohen-green.svg)](https://github.com/asherccohen) [![@asherccohen](https://img.shields.io/badge/twitter-iSnake_-blue.svg)](https://twitter.com/iSnake_)
