karma-jasmine-ajax
==========

Karma adapter for Jasmine plugin for faking Ajax responses in your tests.

With latest dependency on `jasmine-ajax`. when you just use `karma-jasmine-ajax`,
you will find that, it has a very old dependency version on `jasmine-ajax`, and
the author is not convenient to modify for some reason, you can just use this.

Installation
------------

```sh
$ npm install karma-jasmine-ajax-eisoo --save-dev
```

Karma will autoload all the plugins start with `karma-`, so you just add `jasmine-ajax` to the `frameworks` key in your Karma configuration, especially before `jasmine`, or it will cause problem because of dependency.

```js
module.exports = function(config) {
  config.set({
    frameworks: ['jasmine-ajax', 'jasmine']
  });
}
```

Usage
-----

Please see https://github.com/pivotal/jasmine-ajax for details how to use `jasmine-ajax`