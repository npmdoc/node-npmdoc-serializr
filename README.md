# npmdoc-serializr

#### api documentation for  [serializr (v1.1.11)](https://github.com/mobxjs/serializr#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-serializr.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-serializr) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-serializr.svg)](https://travis-ci.org/npmdoc/node-npmdoc-serializr)

#### Serialize and deserialize complex object graphs to JSON

[![NPM](https://nodei.co/npm/serializr.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/serializr)

- [https://npmdoc.github.io/node-npmdoc-serializr/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-serializr/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-serializr/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-serializr/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-serializr/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-serializr/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Michel Weststrate"
    },
    "bugs": {
        "url": "https://github.com/mobxjs/serializr/issues"
    },
    "dependencies": {},
    "description": "Serialize and deserialize complex object graphs to JSON",
    "devDependencies": {
        "babel-cli": "^6.11.4",
        "babel-plugin-transform-decorators-legacy": "^1.3.4",
        "babel-preset-es2015": "^6.9.0",
        "babel-preset-stage-1": "^6.5.0",
        "coveralls": "^2.11.9",
        "documentation": "^4.0.0-beta9",
        "eslint": "^2.12.0",
        "istanbul": "^0.4.4",
        "mobx": "^2.4.1 || ^3.0.0",
        "tape": "^4.5.1",
        "typescript": "^2.1.4",
        "uglify-js": "^2.6.4"
    },
    "directories": {},
    "dist": {
        "shasum": "88434cd5fcb9f82079223443e131f0ce4296cf8a",
        "tarball": "https://registry.npmjs.org/serializr/-/serializr-1.1.11.tgz"
    },
    "files": [
        "serializr.js",
        "serializr.min.js",
        "serializr.min.js.map",
        "serializr.d.ts"
    ],
    "gitHead": "eb6d0a682e72f8a75645e3a016c501e26ba5c7c4",
    "homepage": "https://github.com/mobxjs/serializr#readme",
    "keywords": [
        "serialize",
        "deserialize",
        "graph",
        "json",
        "mobx"
    ],
    "license": "MIT",
    "main": "serializr.js",
    "maintainers": [
        {
            "name": "mweststrate"
        }
    ],
    "name": "serializr",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mobxjs/serializr.git"
    },
    "scripts": {
        "build-docs": "documentation readme serializr.js --github --section API",
        "build-test": "npm run build-test-babel && npm run build-test-ts",
        "build-test-babel": "babel test/babel/babel.js -o test/babel/babel-compiled.js",
        "build-test-ts": "tsc -p test/typescript",
        "coverage": "npm run build-test && istanbul cover tape test/*.js",
        "lint": "eslint serializr.js",
        "prepublish": "npm run small-build && npm run build-docs",
        "small-build": "uglifyjs -m sort,toplevel -c --screw-ie8 --preamble '/** serializr - (c) Michel Weststrate 2016 - MIT Licensed */' --source-map serializr.min.js.map -o serializr.min.js serializr.js",
        "test": "npm run build-test && node test/index"
    },
    "typings": "serializr.d.ts",
    "version": "1.1.11",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
