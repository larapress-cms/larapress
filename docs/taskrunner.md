# Taskrunner

## Introduction

__Bower and Gulp are not required to use this CMS! Anyways, if you want to make a new build you'll need both of them.__

To get started you'll need npm. Installer packages can be found [here](http://nodejs.org).

### Bower

In order to keep all the frontend dependencies up to date we're utilizing [bower](http://bower.io).

> If you have trouble using bower you can find help on their website.

#### Example

```bash
cd $development/larapress
sudo npm install -g bower
bower install
```

__Make sure you `bower install` before running gulp tasks because they will use the frontend dependencies!__

### Gulp

We're using [gulp.js](http://gulpjs.com) for running build tasks.

> If you have trouble using gulp you can find help on their website.

There are several commands you can currently run from the command line:

* `gulp`
* `gulp watch`
* `gulp less`
* `gulp less-per-page`
* `gulp js`
* `gulp js-per-page`
* `gulp fallback`
* `gulp fonts`
* `gulp phpunit`

> Simply running `gulp` will run all the other tasks except `gulp watch` in a row.    
> Use `gulp watch` to make gulp.js watch your filesystem for changes and run the related task.

#### Example

```bash
cd $development/larapress
sudo npm install -g gulp
npm install
gulp
```

#### PHPUnit tests

Larapress comes with a gulp task for the PHPUnit tests to make things easier.
Simply run `gulp phpunit` to run the tests. If you just use `gulp` it will also run the phpunit tests.
Be aware that `gulp watch` wont run phpunit tests!
