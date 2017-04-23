# npmdoc-buffer

#### api documentation for  [buffer (v5.0.6)](https://github.com/feross/buffer)  [![npm package](https://img.shields.io/npm/v/npmdoc-buffer.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-buffer) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-buffer.svg)](https://travis-ci.org/npmdoc/node-npmdoc-buffer)

#### Node.js Buffer API, for the browser

[![NPM](https://nodei.co/npm/buffer.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/buffer)

- [https://npmdoc.github.io/node-npmdoc-buffer/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-buffer/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-buffer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-buffer/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-buffer/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-buffer/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Feross Aboukhadijeh",
        "url": "http://feross.org"
    },
    "bugs": {
        "url": "https://github.com/feross/buffer/issues"
    },
    "contributors": [
        {
            "name": "Romain Beauxis"
        },
        {
            "name": "James Halliday"
        }
    ],
    "dependencies": {
        "base64-js": "^1.0.2",
        "ieee754": "^1.1.4"
    },
    "description": "Node.js Buffer API, for the browser",
    "devDependencies": {
        "benchmark": "^2.0.0",
        "browserify": "^14.0.0",
        "concat-stream": "^1.4.7",
        "hyperquest": "^2.0.0",
        "is-buffer": "^1.1.1",
        "is-nan": "^1.0.1",
        "split": "^1.0.0",
        "standard": "*",
        "tape": "^4.0.0",
        "through2": "^2.0.0",
        "uglify-js": "^2.7.3",
        "zuul": "^3.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "2ea669f7eec0b6eda05b08f8b5ff661b28573588",
        "tarball": "https://registry.npmjs.org/buffer/-/buffer-5.0.6.tgz"
    },
    "gitHead": "cf0c27e9bc645fdcfeefaac9f8da0172475a5277",
    "homepage": "https://github.com/feross/buffer",
    "jspm": {
        "map": {
            "./index.js": {
                "node": "@node/buffer"
            }
        }
    },
    "keywords": [
        "arraybuffer",
        "browser",
        "browserify",
        "buffer",
        "compatible",
        "dataview",
        "uint8array"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "feross"
        }
    ],
    "name": "buffer",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/feross/buffer.git"
    },
    "scripts": {
        "perf": "browserify --debug perf/bracket-notation.js > perf/bundle.js && open perf/index.html",
        "perf-node": "node perf/bracket-notation.js && node perf/concat.js && node perf/copy-big.js && node perf/copy.js && node perf/new-big.js && node perf/new.js && node perf/readDoubleBE.js && node perf/readFloatBE.js && node perf/readUInt32LE.js && node perf/slice.js && node perf/writeFloatBE.js",
        "size": "browserify -r ./ | uglifyjs -c -m | gzip | wc -c",
        "test": "standard && node ./bin/test.js",
        "test-browser-es5": "zuul --ui tape -- test/*.js",
        "test-browser-es5-local": "zuul --ui tape --local -- test/*.js",
        "test-browser-es6": "zuul --ui tape -- test/*.js test/node/*.js",
        "test-browser-es6-local": "zuul --ui tape --local -- test/*.js test/node/*.js",
        "test-node": "tape test/*.js test/node/*.js",
        "update-authors": "./bin/update-authors.sh"
    },
    "standard": {
        "ignore": [
            "test/node/**/*.js",
            "test/_polyfill.js",
            "perf/**/*.js"
        ]
    },
    "version": "5.0.6",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
