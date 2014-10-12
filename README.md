# webfont-extractor

> Split webfont SVG into separate SVG files

## Getting Started
This plugin requires Grunt.

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-webfont-svg-extractor --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-webfont-svg-extractor');
```

## The "webfont_extractor" task

### Overview
In your project's Gruntfile, add a section named `webfont_extractor` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  webfont_svg_extractor: {
    options: {
      fontPath: "test/fixtures/glyphicons-halflings-regular.svg",
      cssPath: "test/fixtures/bootstrap.css",
      outputDir: "tmp/",
      regexp: /.(glyphicon-.*):before/
    }
  },
})
```

### Options

#### options.fontPath
Type: `String`

Path to the original webfont.

#### options.cssPath
Type: `String`
Default value: `'.'`

Path to the associated CSS file.

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_

## License
Copyright (c) 2014 . Licensed under the MIT license.
