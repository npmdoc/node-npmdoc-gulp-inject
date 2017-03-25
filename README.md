# api documentation for  [gulp-inject (v4.2.0)](https://github.com/klei/gulp-inject)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-inject.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-inject)
#### A javascript, stylesheet and webcomponent injection plugin for Gulp, i.e. inject file references into your index.html

[![NPM](https://nodei.co/npm/gulp-inject.png?downloads=true)](https://www.npmjs.com/package/gulp-inject)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-inject/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp_inject_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-inject/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-gulp-inject/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Joakim Carlstein",
        "email": "joakim@klei.se",
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
            "name": "joakimbeng",
            "email": "joakim@klei.se"
        }
    ],
    "name": "gulp-inject",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-inject](#apidoc.module.gulp-inject)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform (filepath, i, length, sourceFile, targetFile)](#apidoc.element.gulp-inject.transform)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.haml (filepath)](#apidoc.element.gulp-inject.transform.haml)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.html (filepath)](#apidoc.element.gulp-inject.transform.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.jade (filepath)](#apidoc.element.gulp-inject.transform.jade)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.jsx (filepath)](#apidoc.element.gulp-inject.transform.jsx)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.less (filepath)](#apidoc.element.gulp-inject.transform.less)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.pug (filepath)](#apidoc.element.gulp-inject.transform.pug)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.sass (filepath)](#apidoc.element.gulp-inject.transform.sass)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.scss (filepath)](#apidoc.element.gulp-inject.transform.scss)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.slim (filepath)](#apidoc.element.gulp-inject.transform.slim)
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform.slm (filepath)](#apidoc.element.gulp-inject.transform.slm)

#### [module gulp-inject.transform](#apidoc.module.gulp-inject.transform)
1.  boolean <span class="apidocSignatureSpan">gulp-inject.transform.</span>selfClosingTag
1.  [function <span class="apidocSignatureSpan">gulp-inject.</span>transform (filepath, i, length, sourceFile, targetFile)](#apidoc.element.gulp-inject.transform.transform)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>haml (filepath)](#apidoc.element.gulp-inject.transform.haml)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>html (filepath)](#apidoc.element.gulp-inject.transform.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>jade (filepath)](#apidoc.element.gulp-inject.transform.jade)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>jsx (filepath)](#apidoc.element.gulp-inject.transform.jsx)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>less (filepath)](#apidoc.element.gulp-inject.transform.less)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>pug (filepath)](#apidoc.element.gulp-inject.transform.pug)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>sass (filepath)](#apidoc.element.gulp-inject.transform.sass)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>scss (filepath)](#apidoc.element.gulp-inject.transform.scss)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>slim (filepath)](#apidoc.element.gulp-inject.transform.slim)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>slm (filepath)](#apidoc.element.gulp-inject.transform.slm)

#### [module gulp-inject.transform.haml](#apidoc.module.gulp-inject.transform.haml)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>haml (filepath)](#apidoc.element.gulp-inject.transform.haml.haml)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.haml.coffee)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>css (filepath)](#apidoc.element.gulp-inject.transform.haml.css)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>html (filepath)](#apidoc.element.gulp-inject.transform.haml.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>image (filepath)](#apidoc.element.gulp-inject.transform.haml.image)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>js (filepath)](#apidoc.element.gulp-inject.transform.haml.js)

#### [module gulp-inject.transform.html](#apidoc.module.gulp-inject.transform.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>html (filepath)](#apidoc.element.gulp-inject.transform.html.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.html.coffee)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>css (filepath)](#apidoc.element.gulp-inject.transform.html.css)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>image (filepath)](#apidoc.element.gulp-inject.transform.html.image)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>js (filepath)](#apidoc.element.gulp-inject.transform.html.js)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>jsx (filepath)](#apidoc.element.gulp-inject.transform.html.jsx)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>map (filepath)](#apidoc.element.gulp-inject.transform.html.map)

#### [module gulp-inject.transform.jade](#apidoc.module.gulp-inject.transform.jade)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>jade (filepath)](#apidoc.element.gulp-inject.transform.jade.jade)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.jade.coffee)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>css (filepath)](#apidoc.element.gulp-inject.transform.jade.css)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>html (filepath)](#apidoc.element.gulp-inject.transform.jade.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>image (filepath)](#apidoc.element.gulp-inject.transform.jade.image)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>js (filepath)](#apidoc.element.gulp-inject.transform.jade.js)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>jsx (filepath)](#apidoc.element.gulp-inject.transform.jade.jsx)

#### [module gulp-inject.transform.jsx](#apidoc.module.gulp-inject.transform.jsx)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>jsx ()](#apidoc.element.gulp-inject.transform.jsx.jsx)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>coffee ()](#apidoc.element.gulp-inject.transform.jsx.coffee)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>css ()](#apidoc.element.gulp-inject.transform.jsx.css)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>html ()](#apidoc.element.gulp-inject.transform.jsx.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>image ()](#apidoc.element.gulp-inject.transform.jsx.image)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>js ()](#apidoc.element.gulp-inject.transform.jsx.js)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>map ()](#apidoc.element.gulp-inject.transform.jsx.map)

#### [module gulp-inject.transform.less](#apidoc.module.gulp-inject.transform.less)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>less (filepath)](#apidoc.element.gulp-inject.transform.less.less)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.less.</span>css (filepath)](#apidoc.element.gulp-inject.transform.less.css)

#### [module gulp-inject.transform.pug](#apidoc.module.gulp-inject.transform.pug)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>pug (filepath)](#apidoc.element.gulp-inject.transform.pug.pug)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.pug.coffee)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>css (filepath)](#apidoc.element.gulp-inject.transform.pug.css)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>html (filepath)](#apidoc.element.gulp-inject.transform.pug.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>image (filepath)](#apidoc.element.gulp-inject.transform.pug.image)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>js (filepath)](#apidoc.element.gulp-inject.transform.pug.js)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>jsx (filepath)](#apidoc.element.gulp-inject.transform.pug.jsx)

#### [module gulp-inject.transform.sass](#apidoc.module.gulp-inject.transform.sass)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>sass (filepath)](#apidoc.element.gulp-inject.transform.sass.sass)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.sass.</span>css (filepath)](#apidoc.element.gulp-inject.transform.sass.css)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.sass.</span>scss (filepath)](#apidoc.element.gulp-inject.transform.sass.scss)

#### [module gulp-inject.transform.scss](#apidoc.module.gulp-inject.transform.scss)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>scss (filepath)](#apidoc.element.gulp-inject.transform.scss.scss)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.scss.</span>css (filepath)](#apidoc.element.gulp-inject.transform.scss.css)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.scss.</span>sass (filepath)](#apidoc.element.gulp-inject.transform.scss.sass)

#### [module gulp-inject.transform.slim](#apidoc.module.gulp-inject.transform.slim)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>slim (filepath)](#apidoc.element.gulp-inject.transform.slim.slim)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.slim.coffee)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>css (filepath)](#apidoc.element.gulp-inject.transform.slim.css)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>html (filepath)](#apidoc.element.gulp-inject.transform.slim.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>image (filepath)](#apidoc.element.gulp-inject.transform.slim.image)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>js (filepath)](#apidoc.element.gulp-inject.transform.slim.js)

#### [module gulp-inject.transform.slm](#apidoc.module.gulp-inject.transform.slm)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.</span>slm (filepath)](#apidoc.element.gulp-inject.transform.slm.slm)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.slm.coffee)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>css (filepath)](#apidoc.element.gulp-inject.transform.slm.css)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>html (filepath)](#apidoc.element.gulp-inject.transform.slm.html)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>image (filepath)](#apidoc.element.gulp-inject.transform.slm.image)
1.  [function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>js (filepath)](#apidoc.element.gulp-inject.transform.slm.js)



# <a name="apidoc.module.gulp-inject"></a>[module gulp-inject](#apidoc.module.gulp-inject)

#### <a name="apidoc.element.gulp-inject.transform"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform (filepath, i, length, sourceFile, targetFile)](#apidoc.element.gulp-inject.transform)
- description and source-code
```javascript
transform = function (filepath, i, length, sourceFile, targetFile) {
  var type;
  if (targetFile && targetFile.path) {
    var ext = extname(targetFile.path);
    type = typeFromExt(ext);
  }
  if (!isTargetType(type)) {
    type = DEFAULT_TARGET;
  }
  var func = transform[type];
  if (func) {
    return func.apply(transform, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.haml"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.haml (filepath)](#apidoc.element.gulp-inject.transform.haml)
- description and source-code
```javascript
transform.haml = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.html"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.html (filepath)](#apidoc.element.gulp-inject.transform.html)
- description and source-code
```javascript
transform.html = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jade"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.jade (filepath)](#apidoc.element.gulp-inject.transform.jade)
- description and source-code
```javascript
transform.jade = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jsx"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.jsx (filepath)](#apidoc.element.gulp-inject.transform.jsx)
- description and source-code
```javascript
transform.jsx = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.less"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.less (filepath)](#apidoc.element.gulp-inject.transform.less)
- description and source-code
```javascript
transform.less = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.pug"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.pug (filepath)](#apidoc.element.gulp-inject.transform.pug)
- description and source-code
```javascript
transform.pug = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.sass"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.sass (filepath)](#apidoc.element.gulp-inject.transform.sass)
- description and source-code
```javascript
transform.sass = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.scss"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.scss (filepath)](#apidoc.element.gulp-inject.transform.scss)
- description and source-code
```javascript
transform.scss = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slim"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.slim (filepath)](#apidoc.element.gulp-inject.transform.slim)
- description and source-code
```javascript
transform.slim = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slm"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform.slm (filepath)](#apidoc.element.gulp-inject.transform.slm)
- description and source-code
```javascript
transform.slm = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform"></a>[module gulp-inject.transform](#apidoc.module.gulp-inject.transform)

#### <a name="apidoc.element.gulp-inject.transform.transform"></a>[function <span class="apidocSignatureSpan">gulp-inject.</span>transform (filepath, i, length, sourceFile, targetFile)](#apidoc.element.gulp-inject.transform.transform)
- description and source-code
```javascript
transform = function (filepath, i, length, sourceFile, targetFile) {
  var type;
  if (targetFile && targetFile.path) {
    var ext = extname(targetFile.path);
    type = typeFromExt(ext);
  }
  if (!isTargetType(type)) {
    type = DEFAULT_TARGET;
  }
  var func = transform[type];
  if (func) {
    return func.apply(transform, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.haml"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>haml (filepath)](#apidoc.element.gulp-inject.transform.haml)
- description and source-code
```javascript
haml = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.html"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>html (filepath)](#apidoc.element.gulp-inject.transform.html)
- description and source-code
```javascript
html = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jade"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>jade (filepath)](#apidoc.element.gulp-inject.transform.jade)
- description and source-code
```javascript
jade = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jsx"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>jsx (filepath)](#apidoc.element.gulp-inject.transform.jsx)
- description and source-code
```javascript
jsx = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.less"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>less (filepath)](#apidoc.element.gulp-inject.transform.less)
- description and source-code
```javascript
less = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.pug"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>pug (filepath)](#apidoc.element.gulp-inject.transform.pug)
- description and source-code
```javascript
pug = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.sass"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>sass (filepath)](#apidoc.element.gulp-inject.transform.sass)
- description and source-code
```javascript
sass = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.scss"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>scss (filepath)](#apidoc.element.gulp-inject.transform.scss)
- description and source-code
```javascript
scss = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slim"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>slim (filepath)](#apidoc.element.gulp-inject.transform.slim)
- description and source-code
```javascript
slim = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slm"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>slm (filepath)](#apidoc.element.gulp-inject.transform.slm)
- description and source-code
```javascript
slm = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.haml"></a>[module gulp-inject.transform.haml](#apidoc.module.gulp-inject.transform.haml)

#### <a name="apidoc.element.gulp-inject.transform.haml.haml"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>haml (filepath)](#apidoc.element.gulp-inject.transform.haml.haml)
- description and source-code
```javascript
haml = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.haml.coffee"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.haml.coffee)
- description and source-code
```javascript
coffee = function (filepath) {
  return '%script{type:"text/coffeescript", src:"' + filepath + '"}';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.haml.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>css (filepath)](#apidoc.element.gulp-inject.transform.haml.css)
- description and source-code
```javascript
css = function (filepath) {
  return '%link{rel:"stylesheet", href:"' + filepath + '"}';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.haml.html"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>html (filepath)](#apidoc.element.gulp-inject.transform.haml.html)
- description and source-code
```javascript
html = function (filepath) {
  return '%link{rel:"import", href:"' + filepath + '"}';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.haml.image"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>image (filepath)](#apidoc.element.gulp-inject.transform.haml.image)
- description and source-code
```javascript
image = function (filepath) {
  return '%img{src:"' + filepath + '"}';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.haml.js"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.haml.</span>js (filepath)](#apidoc.element.gulp-inject.transform.haml.js)
- description and source-code
```javascript
js = function (filepath) {
  return '%script{src:"' + filepath + '"}';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.html"></a>[module gulp-inject.transform.html](#apidoc.module.gulp-inject.transform.html)

#### <a name="apidoc.element.gulp-inject.transform.html.html"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>html (filepath)](#apidoc.element.gulp-inject.transform.html.html)
- description and source-code
```javascript
html = function (filepath) {
  return '<link rel="import" href="' + filepath + '"' + end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.html.coffee"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.html.coffee)
- description and source-code
```javascript
coffee = function (filepath) {
  return '<script type="text/coffeescript" src="' + filepath + '"></script>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.html.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>css (filepath)](#apidoc.element.gulp-inject.transform.html.css)
- description and source-code
```javascript
css = function (filepath) {
  return '<link rel="stylesheet" href="' + filepath + '"' + end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.html.image"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>image (filepath)](#apidoc.element.gulp-inject.transform.html.image)
- description and source-code
```javascript
image = function (filepath) {
  return '<img src="' + filepath + '"' + end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.html.js"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>js (filepath)](#apidoc.element.gulp-inject.transform.html.js)
- description and source-code
```javascript
js = function (filepath) {
  return '<script src="' + filepath + '"></script>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.html.jsx"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>jsx (filepath)](#apidoc.element.gulp-inject.transform.html.jsx)
- description and source-code
```javascript
jsx = function (filepath) {
  return '<script type="text/jsx" src="' + filepath + '"></script>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.html.map"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.html.</span>map (filepath)](#apidoc.element.gulp-inject.transform.html.map)
- description and source-code
```javascript
map = function (filepath) {
  return '<script src="' + filepath + '"></script>';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.jade"></a>[module gulp-inject.transform.jade](#apidoc.module.gulp-inject.transform.jade)

#### <a name="apidoc.element.gulp-inject.transform.jade.jade"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>jade (filepath)](#apidoc.element.gulp-inject.transform.jade.jade)
- description and source-code
```javascript
jade = function (filepath) {
  return 'include ' + filepath;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jade.coffee"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.jade.coffee)
- description and source-code
```javascript
coffee = function (filepath) {
  return 'script(type="text/coffeescript", src="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jade.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>css (filepath)](#apidoc.element.gulp-inject.transform.jade.css)
- description and source-code
```javascript
css = function (filepath) {
  return 'link(rel="stylesheet", href="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jade.html"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>html (filepath)](#apidoc.element.gulp-inject.transform.jade.html)
- description and source-code
```javascript
html = function (filepath) {
  return 'link(rel="import", href="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jade.image"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>image (filepath)](#apidoc.element.gulp-inject.transform.jade.image)
- description and source-code
```javascript
image = function (filepath) {
  return 'img(src="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jade.js"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>js (filepath)](#apidoc.element.gulp-inject.transform.jade.js)
- description and source-code
```javascript
js = function (filepath) {
  return 'script(src="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jade.jsx"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jade.</span>jsx (filepath)](#apidoc.element.gulp-inject.transform.jade.jsx)
- description and source-code
```javascript
jsx = function (filepath) {
  return 'script(type="text/jsx", src="' + filepath + '")';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.jsx"></a>[module gulp-inject.transform.jsx](#apidoc.module.gulp-inject.transform.jsx)

#### <a name="apidoc.element.gulp-inject.transform.jsx.jsx"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>jsx ()](#apidoc.element.gulp-inject.transform.jsx.jsx)
- description and source-code
```javascript
jsx = function () {
  var originalOption = transform.selfClosingTag;
  transform.selfClosingTag = true;
  var result = transform.html[type].apply(transform.html, arguments);
  transform.selfClosingTag = originalOption;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jsx.coffee"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>coffee ()](#apidoc.element.gulp-inject.transform.jsx.coffee)
- description and source-code
```javascript
coffee = function () {
  var originalOption = transform.selfClosingTag;
  transform.selfClosingTag = true;
  var result = transform.html[type].apply(transform.html, arguments);
  transform.selfClosingTag = originalOption;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jsx.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>css ()](#apidoc.element.gulp-inject.transform.jsx.css)
- description and source-code
```javascript
css = function () {
  var originalOption = transform.selfClosingTag;
  transform.selfClosingTag = true;
  var result = transform.html[type].apply(transform.html, arguments);
  transform.selfClosingTag = originalOption;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jsx.html"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>html ()](#apidoc.element.gulp-inject.transform.jsx.html)
- description and source-code
```javascript
html = function () {
  var originalOption = transform.selfClosingTag;
  transform.selfClosingTag = true;
  var result = transform.html[type].apply(transform.html, arguments);
  transform.selfClosingTag = originalOption;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jsx.image"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>image ()](#apidoc.element.gulp-inject.transform.jsx.image)
- description and source-code
```javascript
image = function () {
  var originalOption = transform.selfClosingTag;
  transform.selfClosingTag = true;
  var result = transform.html[type].apply(transform.html, arguments);
  transform.selfClosingTag = originalOption;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jsx.js"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>js ()](#apidoc.element.gulp-inject.transform.jsx.js)
- description and source-code
```javascript
js = function () {
  var originalOption = transform.selfClosingTag;
  transform.selfClosingTag = true;
  var result = transform.html[type].apply(transform.html, arguments);
  transform.selfClosingTag = originalOption;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.jsx.map"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.jsx.</span>map ()](#apidoc.element.gulp-inject.transform.jsx.map)
- description and source-code
```javascript
map = function () {
  var originalOption = transform.selfClosingTag;
  transform.selfClosingTag = true;
  var result = transform.html[type].apply(transform.html, arguments);
  transform.selfClosingTag = originalOption;
  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.less"></a>[module gulp-inject.transform.less](#apidoc.module.gulp-inject.transform.less)

#### <a name="apidoc.element.gulp-inject.transform.less.less"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>less (filepath)](#apidoc.element.gulp-inject.transform.less.less)
- description and source-code
```javascript
less = function (filepath) {
  return '@import "' + filepath + '";';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.less.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.less.</span>css (filepath)](#apidoc.element.gulp-inject.transform.less.css)
- description and source-code
```javascript
css = function (filepath) {
  return '@import "' + filepath + '";';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.pug"></a>[module gulp-inject.transform.pug](#apidoc.module.gulp-inject.transform.pug)

#### <a name="apidoc.element.gulp-inject.transform.pug.pug"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>pug (filepath)](#apidoc.element.gulp-inject.transform.pug.pug)
- description and source-code
```javascript
pug = function (filepath) {
  return 'include ' + filepath;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.pug.coffee"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.pug.coffee)
- description and source-code
```javascript
coffee = function (filepath) {
  return 'script(type="text/coffeescript", src="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.pug.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>css (filepath)](#apidoc.element.gulp-inject.transform.pug.css)
- description and source-code
```javascript
css = function (filepath) {
  return 'link(rel="stylesheet", href="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.pug.html"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>html (filepath)](#apidoc.element.gulp-inject.transform.pug.html)
- description and source-code
```javascript
html = function (filepath) {
  return 'link(rel="import", href="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.pug.image"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>image (filepath)](#apidoc.element.gulp-inject.transform.pug.image)
- description and source-code
```javascript
image = function (filepath) {
  return 'img(src="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.pug.js"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>js (filepath)](#apidoc.element.gulp-inject.transform.pug.js)
- description and source-code
```javascript
js = function (filepath) {
  return 'script(src="' + filepath + '")';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.pug.jsx"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.pug.</span>jsx (filepath)](#apidoc.element.gulp-inject.transform.pug.jsx)
- description and source-code
```javascript
jsx = function (filepath) {
  return 'script(type="text/jsx", src="' + filepath + '")';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.sass"></a>[module gulp-inject.transform.sass](#apidoc.module.gulp-inject.transform.sass)

#### <a name="apidoc.element.gulp-inject.transform.sass.sass"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>sass (filepath)](#apidoc.element.gulp-inject.transform.sass.sass)
- description and source-code
```javascript
sass = function (filepath) {
  return '@import "' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.sass.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.sass.</span>css (filepath)](#apidoc.element.gulp-inject.transform.sass.css)
- description and source-code
```javascript
css = function (filepath) {
  return '@import "' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.sass.scss"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.sass.</span>scss (filepath)](#apidoc.element.gulp-inject.transform.sass.scss)
- description and source-code
```javascript
scss = function (filepath) {
  return '@import "' + filepath + '"';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.scss"></a>[module gulp-inject.transform.scss](#apidoc.module.gulp-inject.transform.scss)

#### <a name="apidoc.element.gulp-inject.transform.scss.scss"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>scss (filepath)](#apidoc.element.gulp-inject.transform.scss.scss)
- description and source-code
```javascript
scss = function (filepath) {
  return '@import "' + filepath + '";';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.scss.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.scss.</span>css (filepath)](#apidoc.element.gulp-inject.transform.scss.css)
- description and source-code
```javascript
css = function (filepath) {
  return '@import "' + filepath + '";';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.scss.sass"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.scss.</span>sass (filepath)](#apidoc.element.gulp-inject.transform.scss.sass)
- description and source-code
```javascript
sass = function (filepath) {
  return '@import "' + filepath + '";';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.slim"></a>[module gulp-inject.transform.slim](#apidoc.module.gulp-inject.transform.slim)

#### <a name="apidoc.element.gulp-inject.transform.slim.slim"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>slim (filepath)](#apidoc.element.gulp-inject.transform.slim.slim)
- description and source-code
```javascript
slim = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slim.coffee"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.slim.coffee)
- description and source-code
```javascript
coffee = function (filepath) {
  return 'script type="text/coffeescript" src="' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slim.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>css (filepath)](#apidoc.element.gulp-inject.transform.slim.css)
- description and source-code
```javascript
css = function (filepath) {
  return 'link rel="stylesheet" href="' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slim.html"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>html (filepath)](#apidoc.element.gulp-inject.transform.slim.html)
- description and source-code
```javascript
html = function (filepath) {
  return 'link rel="import" href="' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slim.image"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>image (filepath)](#apidoc.element.gulp-inject.transform.slim.image)
- description and source-code
```javascript
image = function (filepath) {
  return 'img src="' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slim.js"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slim.</span>js (filepath)](#apidoc.element.gulp-inject.transform.slim.js)
- description and source-code
```javascript
js = function (filepath) {
  return 'script src="' + filepath + '"';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-inject.transform.slm"></a>[module gulp-inject.transform.slm](#apidoc.module.gulp-inject.transform.slm)

#### <a name="apidoc.element.gulp-inject.transform.slm.slm"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.</span>slm (filepath)](#apidoc.element.gulp-inject.transform.slm.slm)
- description and source-code
```javascript
slm = function (filepath) {
  var ext = extname(filepath);
  var type = typeFromExt(ext);
  var func = transform[targetType][type];
  if (func) {
    return func.apply(transform[targetType], arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slm.coffee"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>coffee (filepath)](#apidoc.element.gulp-inject.transform.slm.coffee)
- description and source-code
```javascript
coffee = function (filepath) {
  return 'script type="text/coffeescript" src="' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slm.css"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>css (filepath)](#apidoc.element.gulp-inject.transform.slm.css)
- description and source-code
```javascript
css = function (filepath) {
  return 'link rel="stylesheet" href="' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slm.html"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>html (filepath)](#apidoc.element.gulp-inject.transform.slm.html)
- description and source-code
```javascript
html = function (filepath) {
  return 'link rel="import" href="' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slm.image"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>image (filepath)](#apidoc.element.gulp-inject.transform.slm.image)
- description and source-code
```javascript
image = function (filepath) {
  return 'img src="' + filepath + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-inject.transform.slm.js"></a>[function <span class="apidocSignatureSpan">gulp-inject.transform.slm.</span>js (filepath)](#apidoc.element.gulp-inject.transform.slm.js)
- description and source-code
```javascript
js = function (filepath) {
  return 'script src="' + filepath + '"';
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
