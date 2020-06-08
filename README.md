Minimal Gulp-Sass-Pug starter
==============================================================

A blank-sheet playground starter kit based on [Sass](http://sass-lang.com) and [Pug](https://pugjs.org/) and run with [Gulp](https://gulpjs.com). There’s not a lot here, it’s not a framework, has no support for compiling .js ~~or images~~, and may not work on your setup. The gulpfile may not be the most elegant either, and you might have different views on tabbing, etc.

I made this purely as a starter for my own stand-alone experiments with css. That said, free to grab and fandoogle it to your own dastardly purposes.


## tl;dr

Clone this repo, then:

1. `npm install`
2. `npm start`

## Outline

Running this will:

1. watch files in `./src/_pug/` and `./src/_sass/` for changes
1. compile `*.pug` to `*.html` files under `./_site/`
1. compile `*.sass` to `./_site/main.css`
1. invoke a server to render the page from `./_site` (set to open in Firefox)

## Features

- [Gulp 4](https://gulpjs.com)
- [Normalize](https://necolas.github.io/normalize.css/)
- [Bourbon](https://www.bourbon.io)
- [PostCSS](https://postcss.org)
	- [Autoprefixer](https://github.com/postcss/autoprefixer)
	- [cssnano](https://cssnano.co)
- [Pug](https://pugjs.org/)
- [Imagemin](https://github.com/imagemin/imagemin)
- [Browsersync](https://www.browsersync.io)

## Installation

### Requirements

This assumes [NodeJS](https://nodejs.org/) is already installed in your favourite manner.

Clone or download to somewhere sensible, then:

```
$ npm install
```

It might be wise to run `npm update --save-dev` first to freshen-up the versions. Or if [npm-check-updates](https://github.com/raineorshine/npm-check-updates) is installed run `ncu -u` then `npm install`.

Then run either `npm start` or simply just `gulp`.

### Useful commands

Clobber and rebuild the site folder:

```
$ gulp build
```

Watch for changes after a manual rebuild:

```
$ gulp watch
```

Clobber the site folder without rebuilding:
```
$ gulp clean
```

## Usage
Edit the `.pug` and `.sass` files as you see fit, and these will be compiled to the site folder. It's probably cleaner to let `main.sass` import the `.sass` partials, or just shove all your sass into main.sass and ignore the other files. Nomalize will be included anyway.

Edit `gulpfile.js` to change browsersync settings if Firefox isn’t your bag, and change the postCSS options to suit your specific compatibility preferences.

See the various documentation pages (linked above) for full configuration details. Or better still, grab a copy of the excellent [Dash](https://kapeli.com/dash) docset reader.