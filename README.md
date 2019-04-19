Minimal Gulp-Sass-Pug starter
==============================================================

A blank-sheet playground starter kit based on Sass and Pug. There’s not a lot here, it’s not a framework, has no support for compiling .js or images, and may not work on your setup. The gulpfile may not be the most elegant either, and you might have different views on tabbing, etc.

I made this purely as a starter for my own stand-alone experiments with css. That said, free to grab and fandoogle it to your own dastardly purposes.


## tl;dr
0. clone it
1. `npm install`
2. `npm start`

## Outline

Run this to:
1. watch files in `./src/_pug` and `./src/_sass` for changes
2. compile `*.pug` to `*.html` in `./_site`
2. compile `*.sass` a single `main.css` file in `./_site`
3. invoke a server to render the page from `./_site` (in Firefox)

## Features

- [Gulp 4](https://gulpjs.com)
- [Autoprefixer](https://github.com/postcss/autoprefixer)
- [Bourbon](https://www.bourbon.io)
- [Normalize](https://necolas.github.io/normalize.css/)
- [Pug](https://pugjs.org/)
- [Browser Sync](https://www.browsersync.io)

## Requirements

This assumes [NodeJS](https://nodejs.org/) is already installed in your favourite manner.

## Installation

`npm install` (might be wise to run `npm update --save-dev` first)
Then either `npm start` or `gulp`

To rebuild the site folder run `gulp build`

To watch for changes after a manual rebuild `gulp watch`

