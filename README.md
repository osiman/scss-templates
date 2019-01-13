

## Getting Started

Bu proje scss için template oluşturmaya yarar

## Requirements
- Node/NPM
- LibSass
- Gulp

## Features
- Live reloading with BrowserSync
- Image Minification
- Github Pages deployment
- Sass linting (based on [default](https://github.com/sasstools/sass-lint/blob/master/lib/config/sass-lint.yml) config)
- Autoprefixer configuration
- SMACSS and Atomic Design-based folder structure
- `px` to `em`, `px` to `rem` and other useful functions.
- Mixins for inlining media queries.
* Useful CSS helper classes.
* Default print styles, performance optimized.
* "Delete-key friendly." Easy to strip out parts you don't need.
- Includes:
  - [`Normalize.css`](https://necolas.github.com/normalize.css/)
    for CSS normalizations and common bug fixes
  - [`CSS Pesticide`](https://pesticide.io)
    for easy CSS debugging
  - [`jQuery`](https://jquery.com/) via CDN, with a local fallback
  - [`Modernizr`](http://modernizr.com/), via CDN, for feature
    detection
  - [`Apache Server Configs`](https://github.com/h5bp/server-configs-apache)
    that, among other, improve the web site's performance and security

## Dependencies
```
  "browser-sync": "^2.0.0-rc4",
  "colors": "^1.1.2",
  "del": "^2.0.2",
  "gulp-autoprefixer": "^2.1.0",
  "gulp-concat": "^2.4.3",
  "gulp-gh-pages": "^0.4.0",
  "gulp-imagemin": "^2.1.0",
  "gulp-jshint": "^1.9.0",
  "gulp-minify-css": "^0.3.12",
  "gulp-minify-html": "^0.1.8",
  "gulp-notify": "^2.2.0",
  "gulp-plumber": "^0.6.6",
  "gulp-rename": "^1.2.0",
  "gulp-sass": "^1.3.2",
  "gulp-sass-lint": "1.0.1",
  "gulp-size": "^1.2.0",
  "gulp-sourcemaps": "^1.5.2",
  "gulp-uglify": "^1.0.2",
  "imagemin-pngquant": "^4.0.0",
  "sassdoc": "^2.1.15",
  "vinyl-paths": "^2.0.0"
```

## Tasks
- clean:dist
- styles
- browser-sync
- deploy
- js-app
- js-libs
- sass-lint
- minify-html
- watch
- imagemin
- stats
- sassdoc
- themes
- default
  - clean:dist
  - browser-sync
  - js-app
  - js-libs
  - imgmin
  - minify-html
  - styles
  - watch
- build
  - clean:dist
  - js-app
  - js-libs
  - imgmin
  - minify-html
  - styles
  - copy
- audit
  - sass-lint
  - stats

## Directory structure

```
┌── .gitignore
├── .htaccess
├── .sass-lint.yml
├── .travis.yml
├── src
│   ├── browserconfig.xml
│   ├── crossdomain.xml
│   ├── humans.txt
│   ├── icons
│   │   ├── apple-touch-icon-114x114-precomposed.png
│   │   ├── apple-touch-icon-57x57-precomposed.png
│   │   ├── apple-touch-icon-72x72-precomposed.png
│   │   ├── apple-touch-icon-precomposed.png
│   │   ├── apple-touch-icon.png
│   │   ├── favicon.ico
│   │   └── favicon.png
│   ├── img
│   ├── index.html
│   ├── js
│   ├── robots.txt
│   └── scss
│       ├── atoms
│       │   └── _index.scss
│       ├── base
│       │   ├── _base.scss
│       │   └── _index.scss
│       ├── layout
│       │   └── _index.scss
│       ├── libs
│       │   ├── _index.scss
│       │   ├── _normalize.scss
│       │   └── _pesticide.scss
│       ├── molecules
│       │   └── _index.scss
│       ├── organisms
│       │   └── _index.scss
│       ├── overrides
│       │   └── _index.scss
│       ├── states
│       │   ├── _index.scss
│       │   └── _print.scss
│       ├── themes
│       │   └── rebeccapurple.scss
│       ├── utilities
│       │   ├── _colors.scss
│       │   ├── _config.scss
│       │   ├── _fonts.scss
│       │   ├── _functions.scss
│       │   ├── _index.scss
│       │   ├── _mixins.scss
│       │   └── _typography.scss
│       ├── styles.scss
│       └── _shame.scss
├── gulpfile.js
└── package.json
```

## Bugs & Support
Developed by [@MinaMarkham](http://twitter.com/MinaMarkham). Please list all bugs and feature requests in the Github issue tracker.

## Thanks & Resources

This toolkit is based on the work of the following fine people & projects.

- [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate)
- [Scalable and Modular Architecture for CSS](http://smacss.com/book) (<abbr title="Scalable and Modular Architecture for CSS">SMACSS</abbr>)
- [Atomic Design](http://atomicdesign.bradfrost.com)
