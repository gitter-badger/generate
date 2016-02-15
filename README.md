# generate [![NPM version](https://img.shields.io/npm/v/generate.svg)](https://www.npmjs.com/package/generate) [![Build Status](https://img.shields.io/travis/generate/generate.svg)](https://travis-ci.org/generate/generate)

> Fast, composable, highly extendable project generator with a user-friendly and expressive API.

You might also be interested in [verb](https://github.com/verbose/verb).

## TOC

- [Install](#install)
- [What is generate?](#what-is-generate-)
  * [Feature Highlights](#feature-highlights)
- [Quickstart](#quickstart)
- [Related projects](#related-projects)
- [Generate docs](#generate-docs)
- [Running tests](#running-tests)
- [Contributing](#contributing)
- [Author](#author)
- [License](#license)

_(TOC generated by [verb](https://github.com/verbose/verb) using [markdown-toc](https://github.com/jonschlinkert/markdown-toc))_

## Install

Install globally with [npm](https://www.npmjs.com/)

```sh
$ npm i -g generate
```

## What is generate?

Generate is a fast, highly pluggable project generator, with a user-friendly CLI and an expressive API.

### Feature Highlights

* [x] Run local or globally-installed generators
* [x] Run sub-generators using simple dot-notation. Supports any level of nesting!
* [x] Run [gulp](http://gulpjs.com)-style "tasks" and uses some of the same underlying libraries as gulp
* [x] Built on [assemble-core](https://github.com/assemble/assemble-core) with support for both [gulp](http://gulpjs.com) and [assemble](https://github.com/assemble/assemble) plugins
* [x] Generators can extend and use other generators
* [x] Generators, sub-generators and tasks can be run by command line, API, or both.
* [x] Run tasks from any generator or sub-generator, programmatically or via CLI
* [x] Easy to add functionality and features to generate using via plugins
* [x] Supports any template engine
* [x] First class support for template collections, including pagination, sorting, groups, and more.
* [x] supports middleware that can be run on all files or specific files, and at specific points during the _build process_ (like `onLoad`, `preRender`, `postRender`, etc)

Generate is also well-tested, with more than [1100 unit tests](./test).

## Quickstart

**1. generator.js**

Create a `generator.js` file, and add the following code:

```js
module.exports = function(app) {
  app.task('default', function(cb) {
    console.log('task > default');
    cb();
  });

  app.task('foo', function(cb) {
    console.log('task > foo');
    cb();
  });
};
```

**2. Run `gen`**

In the command line run:

* `gen` to execute the `default` task
* `gen foo` to execute the `foo` task

## Related projects

* [assemble](https://www.npmjs.com/package/assemble): Assemble is a powerful, extendable and easy to use static site generator for node.js. Used… [more](https://www.npmjs.com/package/assemble) | [homepage](https://github.com/assemble/assemble)
* [base](https://www.npmjs.com/package/base): base is the foundation for creating modular, unit testable and highly pluggable node.js applications, starting… [more](https://www.npmjs.com/package/base) | [homepage](https://github.com/node-base/base)
* [update](https://www.npmjs.com/package/update): Easily keep anything in your project up-to-date by installing the updaters you want to use… [more](https://www.npmjs.com/package/update) | [homepage](https://github.com/update/update)
* [verb](https://www.npmjs.com/package/verb): Documentation generator for GitHub projects. Verb is extremely powerful, easy to use, and is used… [more](https://www.npmjs.com/package/verb) | [homepage](https://github.com/verbose/verb)

## Generate docs

Generate readme and API documentation with [verb](https://github.com/verbose/verb):

```sh
$ npm i -d && npm run docs
```

Or, if [verb](https://github.com/verbose/verb) is installed globally:

```sh
$ verb
```

## Running tests

Install dev dependencies:

```sh
$ npm i -d && npm test
```

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/generate/issues/new).

## Author

**Jon Schlinkert**

* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2016 [Jon Schlinkert](https://github.com/jonschlinkert)
Released under the [MIT license](https://github.com/generate/generate/blob/master/LICENSE).

***

_This file was generated by [verb](https://github.com/verbose/verb), v0.9.0, on February 15, 2016._