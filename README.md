# npmdoc-gulp-inject

#### api documentation for  [gulp-inject (v4.2.0)](https://github.com/klei/gulp-inject)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-inject.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-inject) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-inject.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-inject)

#### A javascript, stylesheet and webcomponent injection plugin for Gulp, i.e. inject file references into your index.html

[![NPM](https://nodei.co/npm/gulp-inject.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gulp-inject)

- [https://npmdoc.github.io/node-npmdoc-gulp-inject/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gulp-inject/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-inject/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-inject/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-inject/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-inject/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Joakim Carlstein",
        "url": "http://joakim.beng.se"
    },
    "bugs": {
        "url": "https://github.com/klei/gulp-inject/issues"
    },
    "dependencies": {
        "arrify": "^1.0.1",
        "escape-string-regexp": "^1.0.5",
        "event-stream": "^3.1.0",
        "group-array": "^0.3.0",
        "gulp-util": "^3.0.0",
        "stream-to-array": "^2.3.0",
        "through2": "^2.0.1"
    },
    "description": "A javascript, stylesheet and webcomponent injection plugin for Gulp, i.e. inject file references into your index.html",
    "devDependencies": {
        "mocha": "~2.0.1",
        "should": "^4.0.4",
        "standard-version": "^2.2.1",
        "strip-color": "^0.1.0",
        "xo": "^0.13.0"
    },
    "directories": {},
    "dist": {
        "shasum": "5d6af52f24963aa0de22993dec846e1e792ab653",
        "tarball": "https://registry.npmjs.org/gulp-inject/-/gulp-inject-4.2.0.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "gitHead": "c978fd7494c9f005040340555a41b081e4081655",
    "homepage": "https://github.com/klei/gulp-inject",
    "keywords": [
        "gulpplugin",
        "inject",
        "stylesheets",
        "webcomponents",
        "scripts",
        "index"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "joakimbeng"
        }
    ],
    "name": "gulp-inject",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/klei/gulp-inject.git"
    },
    "scripts": {
        "lint": "xo",
        "pretest": "npm run -s lint",
        "release": "standard-version",
        "test": "mocha -R spec src/**/*_test.js"
    },
    "version": "4.2.0",
    "xo": {
        "space": true,
        "envs": [
            "node"
        ],
        "rules": {
            "object-shorthand": [
                2,
                "never"
            ]
        }
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
