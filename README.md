_s_gulp
===

This is a fork of the useful starter theme `_s`, or `underscores` by Automattic that uses [Gulp.js](http://gulpjs.com) to build the theme's resource files.  For details on `_s` check out the [Automattic/_s](https://github.com/Automattic/_s) repository.

The goal of `_s_gulp` is to give you a foundation to create your own Gulp build stream. Currently this fork covers:
* SCSS -> CSS processing
* Bower JavaScript dependancies
* JSHint for more error-free JavaScript 
* Concatinating JavaScript files
* Optimizing images
* Watch for file changes to trigger Livereload

Getting Started
---------------

`_s_gulp` depends on [Node.js](http://nodejs.org/) and [npm](http://npmjs.org/). Additionally if you want to use Bower and Scss you will need to make sure you have [bower](http://bower.io), [Ruby](http://www.ruby-lang.org/en/downloads/) and [Sass](http://sass-lang.com/download.html) installed.

##### Use npm to download all of the build dependencies

```sh
$ npm install
```

##### Download Bower components

```sh
$ bower install
```

Usage
-----

The `gulpfile.js` file defines the paths to your build scss, js and image files.  By default the build files will exist in the following directories:

* SCSS - `/build/scss`
* JavaScript - `/build/js`
* Images - `/build/images`

During the build process the files will be processed, optimized and moved to the proper locations for `_s`.

##### Run all tasks, default
```sh
$ gulp
```

##### Watch for changes to run tasks and livereload
```sh
$ gulp watch
```
