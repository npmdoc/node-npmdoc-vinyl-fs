# npmdoc-vinyl-fs

#### api documentation for  [vinyl-fs (v2.4.4)](http://github.com/wearefractal/vinyl-fs)  [![npm package](https://img.shields.io/npm/v/npmdoc-vinyl-fs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-vinyl-fs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-vinyl-fs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-vinyl-fs)

#### Vinyl adapter for the file system

[![NPM](https://nodei.co/npm/vinyl-fs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/vinyl-fs)

- [https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Fractal",
        "url": "http://wearefractal.com/"
    },
    "bugs": {
        "url": "https://github.com/wearefractal/vinyl-fs/issues"
    },
    "dependencies": {
        "duplexify": "^3.2.0",
        "glob-stream": "^5.3.2",
        "graceful-fs": "^4.0.0",
        "gulp-sourcemaps": "1.6.0",
        "is-valid-glob": "^0.3.0",
        "lazystream": "^1.0.0",
        "lodash.isequal": "^4.0.0",
        "merge-stream": "^1.0.0",
        "mkdirp": "^0.5.0",
        "object-assign": "^4.0.0",
        "readable-stream": "^2.0.4",
        "strip-bom": "^2.0.0",
        "strip-bom-stream": "^1.0.0",
        "through2": "^2.0.0",
        "through2-filter": "^2.0.0",
        "vali-date": "^1.0.0",
        "vinyl": "^1.0.0"
    },
    "description": "Vinyl adapter for the file system",
    "devDependencies": {
        "buffer-equal": "^0.0.1",
        "default-resolution": "^1.0.1",
        "del": "^2.2.0",
        "eslint": "^1.10.3",
        "eslint-config-gulp": "^2.0.0",
        "expect": "^1.14.0",
        "github-changes": "^1.0.1",
        "istanbul": "^0.3.0",
        "istanbul-coveralls": "^1.0.1",
        "jscs": "^2.4.0",
        "jscs-preset-gulp": "^1.0.0",
        "mocha": "^2.0.0",
        "mocha-lcov-reporter": "^1.0.0",
        "rimraf": "^2.2.5",
        "should": "^7.0.0",
        "sinon": "^1.10.3"
    },
    "directories": {},
    "dist": {
        "shasum": "be6ff3270cb55dfd7d3063640de81f25d7532239",
        "tarball": "https://registry.npmjs.org/vinyl-fs/-/vinyl-fs-2.4.4.tgz"
    },
    "engines": {
        "node": ">=0.10"
    },
    "files": [
        "index.js",
        "lib"
    ],
    "gitHead": "8779a407d76ded1880a9fa6300dc007afd9a94f6",
    "homepage": "http://github.com/wearefractal/vinyl-fs",
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "contra"
        },
        {
            "name": "fractal"
        },
        {
            "name": "phated"
        }
    ],
    "name": "vinyl-fs",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/wearefractal/vinyl-fs.git"
    },
    "scripts": {
        "changelog": "github-changes -o gulpjs -r vinyl-fs -b master -f ./CHANGELOG.md --order-semver --use-commit-body",
        "cover": "istanbul cover _mocha",
        "coveralls": "npm run cover && istanbul-coveralls",
        "lint": "eslint . && jscs index.js lib/ test/",
        "test": "npm run lint && mocha"
    },
    "version": "2.4.4"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
