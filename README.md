# SeamCore

![Screenshot of SeamCore](https://raw.githubusercontent.com/bbody/SeamCore/master/images/screenshot.png)

## Description

SeamCore is a tool to Correlate and Visualize Coal Deposits Automatically and visualize them in 3D. It was an entry to the [Unearthed Sydney 2015 Hackathon](https://unearthed.solutions/u/competitions/unearthed-sydney-2015) by the team Fracking Awesome which attained second place. Code is quite hacked together and rebuilt as a purely static site. [SeamCore Preview](https://seamcore.bbody.io/).

## Technologies used

JavaScript
- [ThreeJS](https://threejs.org/)
- [Browserify](http://browserify.org/)
- [Node](https://nodejs.org/)
- [Uglify](https://github.com/mishoo/UglifyJS)

Styles
- [Sass](http://sass-lang.com/) via ([node-sass](https://github.com/sass/node-sass))

Markup
- [Nunjucks](https://mozilla.github.io/nunjucks/)

Automation
- [Gulp](http://gulpjs.com)
- [Travis](https://travis-ci.org/bbody/SeamCore)

Code Management
- [Git](https://git-scm.com/)

## Automated tasks

This project uses [Gulp](http://gulpjs.com) to run automated tasks for development and production builds.
The tasks are as follows:

`gulp --production`: Same as `gulp serve --production` also run `gulp test` and  not boot up production server

`gulp serve`: Compiles preprocessors and boots up development server
`gulp serve --open`: Same as `gulp serve` but will also open up site/app in your default browser
`gulp serve --production`: Same as `gulp serve` but will run all production tasks so you can view the site/app in it's final optimized form

`gulp test`: Lints all `*.js` file in the `source` folder using eslint

***Adding the `--debug` option to any gulp task displays extra debugging information (ex. data being loaded into your templates)***
