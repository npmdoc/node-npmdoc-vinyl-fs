# api documentation for  [vinyl-fs (v2.4.4)](http://github.com/wearefractal/vinyl-fs)  [![npm package](https://img.shields.io/npm/v/npmdoc-vinyl-fs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-vinyl-fs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-vinyl-fs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-vinyl-fs)
#### Vinyl adapter for the file system

[![NPM](https://nodei.co/npm/vinyl-fs.png?downloads=true)](https://www.npmjs.com/package/vinyl-fs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-vinyl-fs_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-vinyl-fs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Fractal",
        "email": "contact@wearefractal.com",
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
            "name": "contra",
            "email": "contra@wearefractal.com"
        },
        {
            "name": "fractal",
            "email": "contact@wearefractal.com"
        },
        {
            "name": "phated",
            "email": "blaine.bublitz@gmail.com"
        }
    ],
    "name": "vinyl-fs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module vinyl-fs](#apidoc.module.vinyl-fs)
1.  [function <span class="apidocSignatureSpan">vinyl-fs.</span>dest (outFolder, opt)](#apidoc.element.vinyl-fs.dest)
1.  [function <span class="apidocSignatureSpan">vinyl-fs.</span>src (glob, opt)](#apidoc.element.vinyl-fs.src)
1.  [function <span class="apidocSignatureSpan">vinyl-fs.</span>symlink (outFolder, opt)](#apidoc.element.vinyl-fs.symlink)
1.  object <span class="apidocSignatureSpan">vinyl-fs.</span>fileOperations

#### [module vinyl-fs.fileOperations](#apidoc.module.vinyl-fs.fileOperations)
1.  [function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>closeFd (propagatedErr, fd, callback)](#apidoc.element.vinyl-fs.fileOperations.closeFd)
1.  [function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>getModeDiff (fsMode, vinylMode)](#apidoc.element.vinyl-fs.fileOperations.getModeDiff)
1.  [function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>getTimesDiff (fsStat, vinylStat)](#apidoc.element.vinyl-fs.fileOperations.getTimesDiff)
1.  [function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>isOwner (fsStat)](#apidoc.element.vinyl-fs.fileOperations.isOwner)
1.  [function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>updateMetadata (fd, file, callback)](#apidoc.element.vinyl-fs.fileOperations.updateMetadata)
1.  [function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>writeFile (path, data, options, callback)](#apidoc.element.vinyl-fs.fileOperations.writeFile)



# <a name="apidoc.module.vinyl-fs"></a>[module vinyl-fs](#apidoc.module.vinyl-fs)

#### <a name="apidoc.element.vinyl-fs.dest"></a>[function <span class="apidocSignatureSpan">vinyl-fs.</span>dest (outFolder, opt)](#apidoc.element.vinyl-fs.dest)
- description and source-code
```javascript
function dest(outFolder, opt) {
  if (!opt) {
    opt = {};
  }

  function saveFile(file, enc, cb) {
    prepareWrite(outFolder, file, opt, function(err, writePath) {
      if (err) {
        return cb(err);
      }
      writeContents(writePath, file, cb);
    });
  }

  var saveStream = through2.obj(opt, saveFile);
  if (!opt.sourcemaps) {
    // Sink the save stream to start flowing
    // Do this on nextTick, it will flow at slowest speed of piped streams
    process.nextTick(sink(saveStream));

    return saveStream;
  }

  var sourcemapOpt = opt.sourcemaps;
  if (typeof sourcemapOpt === 'boolean') {
    sourcemapOpt = {};
  }
  if (typeof sourcemapOpt === 'string') {
    sourcemapOpt = {
      path: sourcemapOpt,
    };
  }

  var mapStream = sourcemaps.write(sourcemapOpt.path, sourcemapOpt);
  var outputStream = duplexify.obj(mapStream, saveStream);
  mapStream.pipe(saveStream);

  // Sink the output stream to start flowing
  // Do this on nextTick, it will flow at slowest speed of piped streams
  process.nextTick(sink(outputStream));

  return outputStream;
}
```
- example usage
```shell
...
var log = function(file, cb) {
  console.log(file.path);
  cb(null, file);
};

vfs.src(['./js/**/*.js', '!./js/vendor/*.js'])
  .pipe(map(log))
  .pipe(vfs.dest('./output'));
'''

## API

### 'src(globs[, options])'

Takes a glob string or an array of glob strings as the first argument and an options object as the second.
...
```

#### <a name="apidoc.element.vinyl-fs.src"></a>[function <span class="apidocSignatureSpan">vinyl-fs.</span>src (glob, opt)](#apidoc.element.vinyl-fs.src)
- description and source-code
```javascript
function src(glob, opt) {
  var options = assign({
    read: true,
    buffer: true,
    stripBOM: true,
    sourcemaps: false,
    passthrough: false,
    followSymlinks: true,
  }, opt);

  // Don't pass 'read' option on to through2
  var read = options.read !== false;
  options.read = undefined;

  var inputPass;

  if (!isValidGlob(glob)) {
    throw new Error('Invalid glob argument: ' + glob);
  }

  var globStream = gs.create(glob, options);

  var outputStream = globStream
    .pipe(wrapWithVinylFile(options));

  if (options.since != null) {
    outputStream = outputStream
      .pipe(filterSince(options.since));
  }

  if (read) {
    outputStream = outputStream
      .pipe(getContents(options));
  }

  if (options.passthrough === true) {
    inputPass = through2.obj(options);
    outputStream = duplexify.obj(inputPass, merge(outputStream, inputPass));
  }
  if (options.sourcemaps === true) {
    outputStream = outputStream
      .pipe(sourcemaps.init({ loadMaps: true }));
  }
  globStream.on('error', outputStream.emit.bind(outputStream, 'error'));
  return outputStream;
}
```
- example usage
```shell
...
var vfs = require('vinyl-fs');

var log = function(file, cb) {
  console.log(file.path);
  cb(null, file);
};

vfs.src(['./js/**/*.js', '!./js/vendor/*.js'])
  .pipe(map(log))
  .pipe(vfs.dest('./output'));
'''

## API

### 'src(globs[, options])'
...
```

#### <a name="apidoc.element.vinyl-fs.symlink"></a>[function <span class="apidocSignatureSpan">vinyl-fs.</span>symlink (outFolder, opt)](#apidoc.element.vinyl-fs.symlink)
- description and source-code
```javascript
function symlink(outFolder, opt) {
  function linkFile(file, enc, cb) {
    var srcPath = file.path;
    var symType = (file.isDirectory() ? 'dir' : 'file');
    prepareWrite(outFolder, file, opt, function(err, writePath) {
      if (err) {
        return cb(err);
      }
      fs.symlink(srcPath, writePath, symType, function(err) {
        if (err && err.code !== 'EEXIST') {
          return cb(err);
        }
        cb(null, file);
      });
    });
  }

  var stream = through2.obj(opt, linkFile);
  // TODO: option for either backpressure or lossy
  stream.resume();
  return stream;
}
```
- example usage
```shell
...

Type: 'String'

Default: 'process.cwd()'

##### 'options.base'

The folder relative to the cwd. This is used to determine the file names when saving in '.symlink()'. Can also be a function that
 takes in a file and returns a folder path.

Type: 'String' or 'Function'

Default: The 'cwd' resolved to the folder path.

##### 'options.dirMode'
...
```



# <a name="apidoc.module.vinyl-fs.fileOperations"></a>[module vinyl-fs.fileOperations](#apidoc.module.vinyl-fs.fileOperations)

#### <a name="apidoc.element.vinyl-fs.fileOperations.closeFd"></a>[function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>closeFd (propagatedErr, fd, callback)](#apidoc.element.vinyl-fs.fileOperations.closeFd)
- description and source-code
```javascript
function closeFd(propagatedErr, fd, callback) {
  if (typeof fd !== 'number') {
    return callback(propagatedErr);
  }

  fs.close(fd, onClosed);

  function onClosed(closeErr) {
    if (propagatedErr || closeErr) {
      return callback(propagatedErr || closeErr);
    }

    callback();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vinyl-fs.fileOperations.getModeDiff"></a>[function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>getModeDiff (fsMode, vinylMode)](#apidoc.element.vinyl-fs.fileOperations.getModeDiff)
- description and source-code
```javascript
function getModeDiff(fsMode, vinylMode) {
  var modeDiff = 0;

  if (typeof vinylMode === 'number') {
    modeDiff = (vinylMode ^ fsMode) & MASK_MODE;
  }

  return modeDiff;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vinyl-fs.fileOperations.getTimesDiff"></a>[function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>getTimesDiff (fsStat, vinylStat)](#apidoc.element.vinyl-fs.fileOperations.getTimesDiff)
- description and source-code
```javascript
function getTimesDiff(fsStat, vinylStat) {

  if (!isValidDate(vinylStat.mtime)) {
    return;
  }

  if (isEqual(vinylStat.mtime, fsStat.mtime) &&
      isEqual(vinylStat.atime, fsStat.atime)) {
    return;
  }

  var atime;
  if (isValidDate(vinylStat.atime)) {
    atime = vinylStat.atime;
  } else {
    atime = fsStat.atime;
  }

  if (!isValidDate(atime)) {
    atime = undefined;
  }

  var timesDiff = {
    mtime: vinylStat.mtime,
    atime: atime,
  };

  return timesDiff;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vinyl-fs.fileOperations.isOwner"></a>[function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>isOwner (fsStat)](#apidoc.element.vinyl-fs.fileOperations.isOwner)
- description and source-code
```javascript
function isOwner(fsStat) {
  var hasGetuid = (typeof process.getuid === 'function');
  var hasGeteuid = (typeof process.geteuid === 'function');

  // If we don't have either, assume we don't have permissions.
  // This should only happen on Windows.
  // Windows basically noops fchmod and errors on futimes called on directories.
  if (!hasGeteuid && !hasGetuid) {
    return false;
  }

  var uid;
  if (hasGeteuid) {
    uid = process.geteuid();
  } else {
    uid = process.getuid();
  }

  if (fsStat.uid !== uid && uid !== 0) {
    return false;
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vinyl-fs.fileOperations.updateMetadata"></a>[function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>updateMetadata (fd, file, callback)](#apidoc.element.vinyl-fs.fileOperations.updateMetadata)
- description and source-code
```javascript
function updateMetadata(fd, file, callback) {

  fs.fstat(fd, onStat);

  function onStat(err, stat) {
    if (err) {
      return callback(err, fd);
    }

    // Check if mode needs to be updated
    var modeDiff = getModeDiff(stat.mode, file.stat.mode);

    // Check if atime/mtime need to be updated
    var timesDiff = getTimesDiff(stat, file.stat);

    // Set file.stat to the reflect current state on disk
    assign(file.stat, stat);

    // Nothing to do
    if (!modeDiff && !timesDiff) {
      return callback(null, fd);
    }

    // Check access, 'futimes' and 'fchmod' only work if we own the file,
    // or if we are effectively root.
    if (!isOwner(stat)) {
      return callback(null, fd);
    }

    if (modeDiff) {
      return mode();
    }
    times();

    function mode() {
      var mode = stat.mode ^ modeDiff;

      fs.fchmod(fd, mode, onFchmod);

      function onFchmod(fchmodErr) {
        if (!fchmodErr) {
          file.stat.mode = mode;
        }
        if (timesDiff) {
          return times(fchmodErr);
        }
        callback(fchmodErr, fd);
      }
    }

    function times(fchmodErr) {
      fs.futimes(fd, timesDiff.atime, timesDiff.mtime, onFutimes);

      function onFutimes(futimesErr) {
        if (!futimesErr) {
          file.stat.atime = timesDiff.atime;
          file.stat.mtime = timesDiff.mtime;
        }
        callback(fchmodErr || futimesErr, fd);
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vinyl-fs.fileOperations.writeFile"></a>[function <span class="apidocSignatureSpan">vinyl-fs.fileOperations.</span>writeFile (path, data, options, callback)](#apidoc.element.vinyl-fs.fileOperations.writeFile)
- description and source-code
```javascript
function writeFile(path, data, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }

  if (!Buffer.isBuffer(data)) {
    callback(new TypeError('Data must be a Buffer'));
    return;
  }

  if (!options) {
    options = {};
  }

  // Default the same as node
  var mode = options.mode || DEFAULT_FILE_MODE;
  var flag = options.flag || 'w';
  var position = APPEND_MODE_REGEXP.test(flag) ? null : 0;

  fs.open(path, flag, mode, onOpen);

  function onOpen(err, fd) {
    if (err) {
      return onComplete(err);
    }

    fs.write(fd, data, 0, data.length, position, onComplete);

    function onComplete(err) {
      callback(err, fd);
    }
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
