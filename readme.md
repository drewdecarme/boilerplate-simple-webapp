# Simple Webapp Boilerplate

## Table of Contents
1. [Why a Boilerplate](#why-a-boilerplate)
2. [Features](#features)
3. [Getting Started](#getting-started)

## Why a Boilerplate
I wanted the ability to be able to start any simple web application project right of the gate and not continually build the asset pipeline from scratch all of the time. I used a Yeoman scaffold as the initial starter and then started to build and take away on top of it for the things that I like to have in my projects.

Projects such as these are normally simple websites, proof of concepts, quick jQuery components, or styling exercises where I don't need a massive asset pipeline.

### Styling
I typically use sass for all of my projects, but I like to set it up in a way where I can port my configurations from project to project. The configuration in this project typically works for this and angular projects (ReactJS is a different situation in that I really don't use the C in CSS via [Babel Plugin React CSS Modules](https://github.com/gajus/babel-plugin-react-css-modules)).

I like to start off with some base builds, define their details as partials and then include them all of the way up the styles file structure. The only sass file that isn't a partial is the main.scss file. That way I know exactly what I'm including, where I'm including it, and what I have access to.

### Javascript
4 words. Lint hard, lint often.


## Features
#### Libraries/Javascript
- [jQuery](https://jquery.com/)
- [Bootstrap 4](https://v4-alpha.getbootstrap.com/) Note Style is commented out by default
- [Modernizr](https://modernizr.com/)
- [AirBnB React Syntax Style Guide](https://github.com/airbnb/javascript/tree/master/react)
- [ES6](http://es6-features.org) (with [Babel](https://babeljs.io))

#### Style Tools
- [Sass](http://sass-lang.com/)
- [Auto Prefixer](https://github.com/postcss/autoprefixer)
- [Modularscale Sass](https://github.com/modularscale/modularscale-sass)
- [CSS Nano](http://cssnano.co/)

#### Build Tools
- [Gulp](http://gulpjs.com/)
- [Browser Sync](https://www.browsersync.io/)
- [Yarn](https://yarnpkg.com/en/)
- [ESLint](http://eslint.org/) based upon [AirBnB Best Practices](https://github.com/airbnb/javascript/tree/master/linters)
- [Babel](https://babeljs.io/)

## Getting Started
  1. Clone the repo `git clone git@github.com:drewdecarme/boilerplate-simple-webapp.git`
  2. Enter the working directory `cd boilerplate-simple-webapp`
  3. Install dependencies `yarn install` (If you don't have yarn installed, you can install it by following the instructions [here](https://yarnpkg.com/lang/en/docs/install/))
  4. Start the solution `yarn start`
  5. A browser window will open with the solution (if it doesn't open, navigate to [http://localhost:9000/](http://localhost:9000))

### Common Scripts
  1. `yarn start` Starts the development instance
  3. `yarn build` Builds the project via the asset pipeline
  4. `yarn test` Runs all of the unit tests
  5. `yarn lint` Lints the src directory
  6. `yarn lint:fix` Runs the linting autofixer on the src directory
  6. `yarn preview` Previews the final build

## To Do
- [ ] Port linter from React Project to this project
