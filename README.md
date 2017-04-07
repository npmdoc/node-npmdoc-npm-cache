# api documentation for  [npm-cache (v0.6.5)](https://github.com/swarajban/npm-cache)  [![npm package](https://img.shields.io/npm/v/npmdoc-npm-cache.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-npm-cache) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-npm-cache.svg)](https://travis-ci.org/npmdoc/node-npmdoc-npm-cache)
#### cache dependency manager installs to local machine

[![NPM](https://nodei.co/npm/npm-cache.png?downloads=true)](https://www.npmjs.com/package/npm-cache)

[![apidoc](https://npmdoc.github.io/node-npmdoc-npm-cache/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-npm-cache_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-npm-cache/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-npm-cache/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-npm-cache/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "swaraj"
    },
    "bin": {
        "npm-cache": "index.js"
    },
    "bugs": {
        "url": "https://github.com/swarajban/npm-cache/issues"
    },
    "contributors": [
        {
            "name": "Aaron Nordyke",
            "email": "aaron.nordyke@gmail.com"
        }
    ],
    "dependencies": {
        "async": "1.5.0",
        "fs-extra": "^0.26.2",
        "fstream": "^1.0.8",
        "lodash": "3.10.1",
        "md5": "2.0.0",
        "nomnom": "1.8.1",
        "rimraf": "^2.5.4",
        "shelljs": "0.5.3",
        "tar-fs": "1.14.0",
        "tmp": "^0.0.28",
        "which": "^1.2.0"
    },
    "description": "cache dependency manager installs to local machine",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "096e81fbd53cd4252ef1f79c5ecbc49b95ceef5c",
        "tarball": "https://registry.npmjs.org/npm-cache/-/npm-cache-0.6.5.tgz"
    },
    "gitHead": "dcc12d1acc94ead195dd2c4d2526a3f88053a806",
    "homepage": "https://github.com/swarajban/npm-cache",
    "keywords": [
        "npm",
        "cache",
        "install",
        "bower",
        "jspm",
        "composer",
        "local"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "swaraj",
            "email": "swarajban@gmail.com"
        }
    ],
    "name": "npm-cache",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/swarajban/npm-cache.git"
    },
    "scripts": {},
    "version": "0.6.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module npm-cache](#apidoc.module.npm-cache)
1.  [function <span class="apidocSignatureSpan">npm-cache.</span>cacheDependencyManager (config)](#apidoc.element.npm-cache.cacheDependencyManager)
1.  object <span class="apidocSignatureSpan">npm-cache.</span>bowerConfig
1.  object <span class="apidocSignatureSpan">npm-cache.</span>cacheDependencyManager.prototype
1.  object <span class="apidocSignatureSpan">npm-cache.</span>composerConfig
1.  object <span class="apidocSignatureSpan">npm-cache.</span>jspmConfig
1.  object <span class="apidocSignatureSpan">npm-cache.</span>logger
1.  object <span class="apidocSignatureSpan">npm-cache.</span>npmConfig
1.  object <span class="apidocSignatureSpan">npm-cache.</span>parseUtils

#### [module npm-cache.bowerConfig](#apidoc.module.npm-cache.bowerConfig)
1.  [function <span class="apidocSignatureSpan">npm-cache.bowerConfig.</span>getCliVersion ()](#apidoc.element.npm-cache.bowerConfig.getCliVersion)
1.  [function <span class="apidocSignatureSpan">npm-cache.bowerConfig.</span>getFileHash (filePath)](#apidoc.element.npm-cache.bowerConfig.getFileHash)
1.  string <span class="apidocSignatureSpan">npm-cache.bowerConfig.</span>cliName
1.  string <span class="apidocSignatureSpan">npm-cache.bowerConfig.</span>configPath
1.  string <span class="apidocSignatureSpan">npm-cache.bowerConfig.</span>installCommand
1.  string <span class="apidocSignatureSpan">npm-cache.bowerConfig.</span>installDirectory

#### [module npm-cache.cacheDependencyManager](#apidoc.module.npm-cache.cacheDependencyManager)
1.  [function <span class="apidocSignatureSpan">npm-cache.</span>cacheDependencyManager (config)](#apidoc.element.npm-cache.cacheDependencyManager.cacheDependencyManager)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.</span>getAvailableDefaultManagers ()](#apidoc.element.npm-cache.cacheDependencyManager.getAvailableDefaultManagers)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.</span>getAvailableManagers ()](#apidoc.element.npm-cache.cacheDependencyManager.getAvailableManagers)
1.  object <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.</span>managers

#### [module npm-cache.cacheDependencyManager.prototype](#apidoc.module.npm-cache.cacheDependencyManager.prototype)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>archiveDependencies (cacheDirectory, cachePath, callback)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.archiveDependencies)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>backupFile (backupPath, file)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.backupFile)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>cacheLogError (error)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.cacheLogError)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>cacheLogInfo (message)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.cacheLogInfo)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>installCachedDependencies (cachePath, compressedCacheExists, callback)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.installCachedDependencies)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>installDependencies ()](#apidoc.element.npm-cache.cacheDependencyManager.prototype.installDependencies)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>loadDependencies (callback)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.loadDependencies)
1.  [function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>restoreFile (backupPath, file)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.restoreFile)

#### [module npm-cache.composerConfig](#apidoc.module.npm-cache.composerConfig)
1.  [function <span class="apidocSignatureSpan">npm-cache.composerConfig.</span>getCliVersion ()](#apidoc.element.npm-cache.composerConfig.getCliVersion)
1.  [function <span class="apidocSignatureSpan">npm-cache.composerConfig.</span>getFileHash (filePath)](#apidoc.element.npm-cache.composerConfig.getFileHash)
1.  string <span class="apidocSignatureSpan">npm-cache.composerConfig.</span>cliName
1.  string <span class="apidocSignatureSpan">npm-cache.composerConfig.</span>configPath
1.  string <span class="apidocSignatureSpan">npm-cache.composerConfig.</span>installCommand
1.  string <span class="apidocSignatureSpan">npm-cache.composerConfig.</span>installDirectory

#### [module npm-cache.jspmConfig](#apidoc.module.npm-cache.jspmConfig)
1.  [function <span class="apidocSignatureSpan">npm-cache.jspmConfig.</span>getCliVersion ()](#apidoc.element.npm-cache.jspmConfig.getCliVersion)
1.  [function <span class="apidocSignatureSpan">npm-cache.jspmConfig.</span>getFileHash ()](#apidoc.element.npm-cache.jspmConfig.getFileHash)
1.  string <span class="apidocSignatureSpan">npm-cache.jspmConfig.</span>addToArchiveAndRestore
1.  string <span class="apidocSignatureSpan">npm-cache.jspmConfig.</span>cliName
1.  string <span class="apidocSignatureSpan">npm-cache.jspmConfig.</span>configPath
1.  string <span class="apidocSignatureSpan">npm-cache.jspmConfig.</span>installCommand
1.  string <span class="apidocSignatureSpan">npm-cache.jspmConfig.</span>installDirectory

#### [module npm-cache.logger](#apidoc.module.npm-cache.logger)
1.  [function <span class="apidocSignatureSpan">npm-cache.logger.</span>logError (errorMessage)](#apidoc.element.npm-cache.logger.logError)
1.  [function <span class="apidocSignatureSpan">npm-cache.logger.</span>logInfo (message)](#apidoc.element.npm-cache.logger.logInfo)

#### [module npm-cache.npmConfig](#apidoc.module.npm-cache.npmConfig)
1.  [function <span class="apidocSignatureSpan">npm-cache.npmConfig.</span>getCliVersion ()](#apidoc.element.npm-cache.npmConfig.getCliVersion)
1.  [function <span class="apidocSignatureSpan">npm-cache.npmConfig.</span>getFileHash (filePath)](#apidoc.element.npm-cache.npmConfig.getFileHash)
1.  string <span class="apidocSignatureSpan">npm-cache.npmConfig.</span>cliName
1.  string <span class="apidocSignatureSpan">npm-cache.npmConfig.</span>configPath
1.  string <span class="apidocSignatureSpan">npm-cache.npmConfig.</span>installCommand
1.  string <span class="apidocSignatureSpan">npm-cache.npmConfig.</span>installDirectory

#### [module npm-cache.parseUtils](#apidoc.module.npm-cache.parseUtils)
1.  [function <span class="apidocSignatureSpan">npm-cache.parseUtils.</span>getManagerArgs ()](#apidoc.element.npm-cache.parseUtils.getManagerArgs)
1.  [function <span class="apidocSignatureSpan">npm-cache.parseUtils.</span>getNpmCacheArgs ()](#apidoc.element.npm-cache.parseUtils.getNpmCacheArgs)



# <a name="apidoc.module.npm-cache"></a>[module npm-cache](#apidoc.module.npm-cache)

#### <a name="apidoc.element.npm-cache.cacheDependencyManager"></a>[function <span class="apidocSignatureSpan">npm-cache.</span>cacheDependencyManager (config)](#apidoc.element.npm-cache.cacheDependencyManager)
- description and source-code
```javascript
function CacheDependencyManager(config) {
  this.config = config;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.npm-cache.bowerConfig"></a>[module npm-cache.bowerConfig](#apidoc.module.npm-cache.bowerConfig)

#### <a name="apidoc.element.npm-cache.bowerConfig.getCliVersion"></a>[function <span class="apidocSignatureSpan">npm-cache.bowerConfig.</span>getCliVersion ()](#apidoc.element.npm-cache.bowerConfig.getCliVersion)
- description and source-code
```javascript
function getNpmVersion() {
  return shell.exec('bower --version', {silent: true}).output.trim();
}
```
- example usage
```shell
...
}

// Get hash of dependency config file
var hash = this.config.getFileHash(this.config.configPath);
hash = md5(cacheVersion + hash);
this.cacheLogInfo('hash of ' + this.config.configPath + ': ' + hash);
// cachePath is absolute path to where local cache of dependencies is located
var cacheDirectory = path.resolve(this.config.cacheDirectory, this.config.cliName, this.config.getCliVersion());
var cachePathArchive = path.resolve(cacheDirectory, hash + '.tar.gz');
var cachePathNotArchived = path.resolve(cacheDirectory, hash);

// Check if local cache of dependencies exists
var cacheArchiveExists = fs.existsSync(cachePathArchive);
var cacheNotArchivedExists = fs.existsSync(cachePathNotArchived);
if (!this.config.forceRefresh && (cacheArchiveExists || cacheNotArchivedExists)) {
...
```

#### <a name="apidoc.element.npm-cache.bowerConfig.getFileHash"></a>[function <span class="apidocSignatureSpan">npm-cache.bowerConfig.</span>getFileHash (filePath)](#apidoc.element.npm-cache.bowerConfig.getFileHash)
- description and source-code
```javascript
function getFileHash(filePath) {
  var json = JSON.parse(fs.readFileSync(filePath));
  return md5(JSON.stringify({
    dependencies: json.dependencies,
    devDependencies: json.devDependencies,
    overrides: json.overrides
  }));
}
```
- example usage
```shell
...

  async.each(
    managers,
    function calculateHash (managerName) {
      var managerConfig = require(availableManagers[managerName]);
      managerConfig.cacheDirectory = opts.cacheDirectory;

      var hash = managerConfig.getFileHash(managerConfig.configPath);
      console.log(hash);
    }
  );
};


// Recursively lists files in directory up to maxDepth
...
```



# <a name="apidoc.module.npm-cache.cacheDependencyManager"></a>[module npm-cache.cacheDependencyManager](#apidoc.module.npm-cache.cacheDependencyManager)

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.cacheDependencyManager"></a>[function <span class="apidocSignatureSpan">npm-cache.</span>cacheDependencyManager (config)](#apidoc.element.npm-cache.cacheDependencyManager.cacheDependencyManager)
- description and source-code
```javascript
function CacheDependencyManager(config) {
  this.config = config;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.getAvailableDefaultManagers"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.</span>getAvailableDefaultManagers ()](#apidoc.element.npm-cache.cacheDependencyManager.getAvailableDefaultManagers)
- description and source-code
```javascript
getAvailableDefaultManagers = function () {
  return _.pick(CacheDependencyManager.getAvailableManagers(), ['composer', 'npm', 'bower']);
}
```
- example usage
```shell
...
  }
);

// If no managers were specified, try installing everything by default!
if (_.isEmpty(managers)) {
  // add all keys from available managers as keys here
  _.forEach(
    CacheDependencyManager.getAvailableDefaultManagers(),
    function addManager (managerPath, manager) {
      managers[manager] = '';
    }
  );
}

return managers;
...
```

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.getAvailableManagers"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.</span>getAvailableManagers ()](#apidoc.element.npm-cache.cacheDependencyManager.getAvailableManagers)
- description and source-code
```javascript
getAvailableManagers = function () {
  if (CacheDependencyManager.managers === undefined) {
    CacheDependencyManager.managers = {};
    var files = fs.readdirSync(__dirname);
    var managerRegex = /(\S+)Config\.js/;
    files.forEach(
      function addAvailableManager (file) {
        var result = managerRegex.exec(file);
        if (result !== null) {
          var managerName = result[1];
          CacheDependencyManager.managers[managerName] = path.join(__dirname, file);
        }
      }
    );
  }
  return CacheDependencyManager.managers;
}
```
- example usage
```shell
...

// npm-cache command handlers

// main method for installing specified dependencies
var installDependencies = function (opts) {
prepareCacheDirectory(opts.cacheDirectory);

var availableManagers = CacheDependencyManager.getAvailableManagers();
var managerArguments = ParseUtils.getManagerArgs();
var managers = Object.keys(managerArguments);

async.each(
  managers,
  function startManager (managerName, callback) {
    var managerConfig = require(availableManagers[managerName]);
...
```



# <a name="apidoc.module.npm-cache.cacheDependencyManager.prototype"></a>[module npm-cache.cacheDependencyManager.prototype](#apidoc.module.npm-cache.cacheDependencyManager.prototype)

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.prototype.archiveDependencies"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>archiveDependencies (cacheDirectory, cachePath, callback)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.archiveDependencies)
- description and source-code
```javascript
archiveDependencies = function (cacheDirectory, cachePath, callback) {
  var self = this;
  var error = null;
  var installedDirectory = getAbsolutePath(this.config.installDirectory);
  var fileBackupDirectory = getFileBackupPath(installedDirectory);
  this.cacheLogInfo('archiving dependencies from ' + installedDirectory);

  if (!fs.existsSync(installedDirectory)) {
    this.cacheLogInfo('skipping archive. Install directory does not exist.');
    return error;
  }

  if (this.config.addToArchiveAndRestore) {
    this.backupFile(fileBackupDirectory, this.config.addToArchiveAndRestore);
  }

  // Make sure cache directory is created
  fs.mkdirsSync(cacheDirectory);

  var tmpName = tmp.tmpNameSync({
    dir: cacheDirectory
  });
  tmp.setGracefulCleanup();

  function onError(error) {
    self.cacheLogError('error tar-ing ' + installedDirectory + ' :' + error);
    onFinally();
    callback(error);
  }

  function onEnd() {
    if (fs.existsSync(cachePath)) {
      fs.removeSync(cachePath);
    }
    fs.renameSync(tmpName, cachePath);
    self.cacheLogInfo('installed and archived dependencies');
    onFinally();
    callback();
  }

  function onFinally() {
    if (fs.existsSync(fileBackupDirectory)) {
      fs.removeSync(fileBackupDirectory);
    }

    if (fs.existsSync(tmpName)) {
      fs.removeSync(tmpName);
    }
  }

  var installedDirectoryStream = fstream.Reader({path: installedDirectory}).on('error', onError);
  // TODO: speed this up
  if (this.config.noArchive) {
    installedDirectoryStream
      .on('end', onEnd)
      .pipe(fstream.Writer({path: tmpName, type: 'Directory'}));

  } else {
    tar.pack(installedDirectory)
      .pipe(zlib.createGzip())
      .pipe(fs.createWriteStream(tmpName))
      .on('error', onError)
      .on('finish', onEnd);
  }
}
```
- example usage
```shell
...
    if (error !== null) {
      callback(error);
      return;
    }

    // Try to archive newly installed dependencies
    var cachePathWithInstalledDirectory = path.resolve(cachePathNotArchived, this.config.installDirectory);
      this.archiveDependencies(
      this.config.noArchive ? cachePathNotArchived : cacheDirectory,
      this.config.noArchive ? cachePathWithInstalledDirectory : cachePathArchive,
      callback
    );
  }
};
...
```

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.prototype.backupFile"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>backupFile (backupPath, file)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.backupFile)
- description and source-code
```javascript
backupFile = function (backupPath, file) {
  var sourceFile = getAbsolutePath(file);
  var backupFilename = getFileBackupFilename(file);
  var backupFile = path.join(backupPath, backupFilename);
  if (!fs.existsSync(sourceFile)) {
    this.cacheLogError('backup file [file not found]:' + file);
    return;
  }

  fs.mkdirsSync(backupPath);
  fs.copySync(sourceFile, backupFile);
  this.cacheLogInfo('backup file: ' + file);
}
```
- example usage
```shell
...

if (!fs.existsSync(installedDirectory)) {
  this.cacheLogInfo('skipping archive. Install directory does not exist.');
  return error;
}

if (this.config.addToArchiveAndRestore) {
  this.backupFile(fileBackupDirectory, this.config.addToArchiveAndRestore);
}

// Make sure cache directory is created
fs.mkdirsSync(cacheDirectory);

var tmpName = tmp.tmpNameSync({
  dir: cacheDirectory
...
```

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.prototype.cacheLogError"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>cacheLogError (error)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.cacheLogError)
- description and source-code
```javascript
cacheLogError = function (error) {
  logger.logError('[' + this.config.cliName + '] ' + error);
}
```
- example usage
```shell
...
CacheDependencyManager.prototype.installDependencies = function () {
  var error = null;
  var installCommand = this.config.installCommand + ' ' + this.config.installOptions;
  installCommand = installCommand.trim();
  this.cacheLogInfo('running [' + installCommand + ']...');
  if (shell.exec(installCommand).code !== 0) {
    error = 'error running ' + this.config.installCommand;
    this.cacheLogError(error);
  } else {
    this.cacheLogInfo('installed ' + this.config.cliName + ' dependencies, now archiving');
  }
  return error;
};

CacheDependencyManager.prototype.backupFile = function (backupPath, file) {
...
```

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.prototype.cacheLogInfo"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>cacheLogInfo (message)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.cacheLogInfo)
- description and source-code
```javascript
cacheLogInfo = function (message) {
  logger.logInfo('[' + this.config.cliName + '] ' + message);
}
```
- example usage
```shell
...
};


CacheDependencyManager.prototype.installDependencies = function () {
var error = null;
var installCommand = this.config.installCommand + ' ' + this.config.installOptions;
installCommand = installCommand.trim();
this.cacheLogInfo('running [' + installCommand + ']...');
if (shell.exec(installCommand).code !== 0) {
  error = 'error running ' + this.config.installCommand;
  this.cacheLogError(error);
} else {
  this.cacheLogInfo('installed ' + this.config.cliName + ' dependencies, now archiving');
}
return error;
...
```

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.prototype.installCachedDependencies"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>installCachedDependencies (cachePath, compressedCacheExists, callback)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.installCachedDependencies)
- description and source-code
```javascript
installCachedDependencies = function (cachePath, compressedCacheExists, callback) {
  var self = this;
  var installDirectory = getAbsolutePath(this.config.installDirectory);
  var fileBackupDirectory = getFileBackupPath(installDirectory);
  var targetPath = path.dirname(installDirectory);
  this.cacheLogInfo('clearing installed dependencies at ' + installDirectory);
  fs.removeSync(installDirectory);
  this.cacheLogInfo('...cleared');
  this.cacheLogInfo('retrieving dependencies from ' + cachePath);

  function onError(error) {
    self.cacheLogError('Error retrieving ' + cachePath + ': ' + error);
    callback(error);
  }
  function onEnd() {
    if (self.config.addToArchiveAndRestore) {
      self.restoreFile(fileBackupDirectory, self.config.addToArchiveAndRestore);
      fs.removeSync(fileBackupDirectory);
    }
    self.cacheLogInfo('done extracting');
    callback();
  }

  if (compressedCacheExists) {
    fs.createReadStream(cachePath)
      .pipe(zlib.createGunzip())
      .pipe(tar.extract(installDirectory))
      .on('error', onError)
      .on('finish', onEnd);
  } else {
    fstream.Reader(cachePath)
        .on('error', onError)
        .on('end', onEnd)
        .pipe(fstream.Writer(targetPath));
  }
}
```
- example usage
```shell
...
// Check if local cache of dependencies exists
var cacheArchiveExists = fs.existsSync(cachePathArchive);
var cacheNotArchivedExists = fs.existsSync(cachePathNotArchived);
if (!this.config.forceRefresh && (cacheArchiveExists || cacheNotArchivedExists)) {
  this.cacheLogInfo('cache exists');

  // Try to retrieve cached dependencies
  this.installCachedDependencies(
    cacheArchiveExists ? cachePathArchive : cachePathNotArchived,
    cacheArchiveExists,
    callback
  );

} else { // install dependencies with CLI tool and cache
  // Try to install dependencies using package manager
...
```

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.prototype.installDependencies"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>installDependencies ()](#apidoc.element.npm-cache.cacheDependencyManager.prototype.installDependencies)
- description and source-code
```javascript
installDependencies = function () {
  var error = null;
  var installCommand = this.config.installCommand + ' ' + this.config.installOptions;
  installCommand = installCommand.trim();
  this.cacheLogInfo('running [' + installCommand + ']...');
  if (shell.exec(installCommand).code !== 0) {
    error = 'error running ' + this.config.installCommand;
    this.cacheLogError(error);
  } else {
    this.cacheLogInfo('installed ' + this.config.cliName + ' dependencies, now archiving');
  }
  return error;
}
```
- example usage
```shell
...
  cacheArchiveExists ? cachePathArchive : cachePathNotArchived,
  cacheArchiveExists,
  callback
);

  } else { // install dependencies with CLI tool and cache
// Try to install dependencies using package manager
error = this.installDependencies();
if (error !== null) {
  callback(error);
  return;
}

// Try to archive newly installed dependencies
var cachePathWithInstalledDirectory = path.resolve(cachePathNotArchived, this.config.installDirectory);
...
```

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.prototype.loadDependencies"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>loadDependencies (callback)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.loadDependencies)
- description and source-code
```javascript
loadDependencies = function (callback) {
  var self = this;
  var error = null;

  // Check if config file for dependency manager exists
  if (! fs.existsSync(this.config.configPath)) {
    this.cacheLogInfo('Dependency config file ' + this.config.configPath + ' does not exist. Skipping install');
    callback(null);
    return;
  }
  this.cacheLogInfo('config file exists');

  // Check if package manger CLI is installed
  try {
    which.sync(this.config.cliName);
    this.cacheLogInfo('cli exists');
  }
  catch (e) {
    error = 'Command line tool ' + this.config.cliName + ' not installed';
    this.cacheLogError(error);
    callback(error);
    return;
  }

  // Get hash of dependency config file
  var hash = this.config.getFileHash(this.config.configPath);
  hash = md5(cacheVersion + hash);
  this.cacheLogInfo('hash of ' + this.config.configPath + ': ' + hash);
  // cachePath is absolute path to where local cache of dependencies is located
  var cacheDirectory = path.resolve(this.config.cacheDirectory, this.config.cliName, this.config.getCliVersion());
  var cachePathArchive = path.resolve(cacheDirectory, hash + '.tar.gz');
  var cachePathNotArchived = path.resolve(cacheDirectory, hash);

  // Check if local cache of dependencies exists
  var cacheArchiveExists = fs.existsSync(cachePathArchive);
  var cacheNotArchivedExists = fs.existsSync(cachePathNotArchived);
  if (!this.config.forceRefresh && (cacheArchiveExists || cacheNotArchivedExists)) {
    this.cacheLogInfo('cache exists');

    // Try to retrieve cached dependencies
    this.installCachedDependencies(
      cacheArchiveExists ? cachePathArchive : cachePathNotArchived,
      cacheArchiveExists,
      callback
    );

  } else { // install dependencies with CLI tool and cache
    // Try to install dependencies using package manager
    error = this.installDependencies();
    if (error !== null) {
      callback(error);
      return;
    }

    // Try to archive newly installed dependencies
    var cachePathWithInstalledDirectory = path.resolve(cachePathNotArchived, this.config.installDirectory);
      this.archiveDependencies(
      this.config.noArchive ? cachePathNotArchived : cacheDirectory,
      this.config.noArchive ? cachePathWithInstalledDirectory : cachePathArchive,
      callback
    );
  }
}
```
- example usage
```shell
...
function startManager (managerName, callback) {
  var managerConfig = require(availableManagers[managerName]);
  managerConfig.cacheDirectory = opts.cacheDirectory;
  managerConfig.forceRefresh = opts.forceRefresh;
  managerConfig.noArchive = opts.noArchive;
  managerConfig.installOptions = managerArguments[managerName];
  var manager = new CacheDependencyManager(managerConfig);
  manager.loadDependencies(callback);
},
function onInstalled (error) {
  if (error === null) {
    logger.logInfo('successfully installed all dependencies');
    process.exit(0);
  } else {
    logger.logError('error installing dependencies');
...
```

#### <a name="apidoc.element.npm-cache.cacheDependencyManager.prototype.restoreFile"></a>[function <span class="apidocSignatureSpan">npm-cache.cacheDependencyManager.prototype.</span>restoreFile (backupPath, file)](#apidoc.element.npm-cache.cacheDependencyManager.prototype.restoreFile)
- description and source-code
```javascript
restoreFile = function (backupPath, file) {
  var sourceFile = getAbsolutePath(file);
  var backupFilename = getFileBackupFilename(file);
  var backupFile = path.join(backupPath, backupFilename);
  if (!fs.existsSync(backupFile)) {
    this.cacheLogError('restore file [file not found]:' + file);
    return;
  }

  fs.copySync(backupFile, sourceFile);
  this.cacheLogInfo('restore file: ' + file);
}
```
- example usage
```shell
...

function onError(error) {
  self.cacheLogError('Error retrieving ' + cachePath + ': ' + error);
  callback(error);
}
function onEnd() {
  if (self.config.addToArchiveAndRestore) {
    self.restoreFile(fileBackupDirectory, self.config.addToArchiveAndRestore);
    fs.removeSync(fileBackupDirectory);
  }
  self.cacheLogInfo('done extracting');
  callback();
}

if (compressedCacheExists) {
...
```



# <a name="apidoc.module.npm-cache.composerConfig"></a>[module npm-cache.composerConfig](#apidoc.module.npm-cache.composerConfig)

#### <a name="apidoc.element.npm-cache.composerConfig.getCliVersion"></a>[function <span class="apidocSignatureSpan">npm-cache.composerConfig.</span>getCliVersion ()](#apidoc.element.npm-cache.composerConfig.getCliVersion)
- description and source-code
```javascript
getCliVersion = function () {
  var version = 'UnknownComposer';
  var versionString = shell.exec('composer --version', {silent: true}).output;
  // Example below:
  //    Composer version 1.0.0-alpha9 2014-12-07 17:15:20
  var versionRegex = /Composer version (\S+)/;
  var result = versionRegex.exec(versionString);
  if (result !== null) {
    version = result[1];
  } else {
    logger.logInfo('Could not find composer version from version string: ' + versionString);
  }
  return version;
}
```
- example usage
```shell
...
}

// Get hash of dependency config file
var hash = this.config.getFileHash(this.config.configPath);
hash = md5(cacheVersion + hash);
this.cacheLogInfo('hash of ' + this.config.configPath + ': ' + hash);
// cachePath is absolute path to where local cache of dependencies is located
var cacheDirectory = path.resolve(this.config.cacheDirectory, this.config.cliName, this.config.getCliVersion());
var cachePathArchive = path.resolve(cacheDirectory, hash + '.tar.gz');
var cachePathNotArchived = path.resolve(cacheDirectory, hash);

// Check if local cache of dependencies exists
var cacheArchiveExists = fs.existsSync(cachePathArchive);
var cacheNotArchivedExists = fs.existsSync(cachePathNotArchived);
if (!this.config.forceRefresh && (cacheArchiveExists || cacheNotArchivedExists)) {
...
```

#### <a name="apidoc.element.npm-cache.composerConfig.getFileHash"></a>[function <span class="apidocSignatureSpan">npm-cache.composerConfig.</span>getFileHash (filePath)](#apidoc.element.npm-cache.composerConfig.getFileHash)
- description and source-code
```javascript
function getFileHash(filePath) {
  var json = JSON.parse(fs.readFileSync(filePath));

  if (isUsingComposerLock) {
    return json['content-hash'];
  }

  return md5(JSON.stringify({
    packages: json.require,
    packagesDev: json['require-dev'],
    repos: json.repositories
  }));
}
```
- example usage
```shell
...

  async.each(
    managers,
    function calculateHash (managerName) {
      var managerConfig = require(availableManagers[managerName]);
      managerConfig.cacheDirectory = opts.cacheDirectory;

      var hash = managerConfig.getFileHash(managerConfig.configPath);
      console.log(hash);
    }
  );
};


// Recursively lists files in directory up to maxDepth
...
```



# <a name="apidoc.module.npm-cache.jspmConfig"></a>[module npm-cache.jspmConfig](#apidoc.module.npm-cache.jspmConfig)

#### <a name="apidoc.element.npm-cache.jspmConfig.getCliVersion"></a>[function <span class="apidocSignatureSpan">npm-cache.jspmConfig.</span>getCliVersion ()](#apidoc.element.npm-cache.jspmConfig.getCliVersion)
- description and source-code
```javascript
function getJspmVersion() {
    var rawMultilineOutput = shell.exec('jspm --version', {silent: true}).output;
    var version = rawMultilineOutput.split('\n')[0] || 'UnknownVersion';
    return version.trim();
}
```
- example usage
```shell
...
}

// Get hash of dependency config file
var hash = this.config.getFileHash(this.config.configPath);
hash = md5(cacheVersion + hash);
this.cacheLogInfo('hash of ' + this.config.configPath + ': ' + hash);
// cachePath is absolute path to where local cache of dependencies is located
var cacheDirectory = path.resolve(this.config.cacheDirectory, this.config.cliName, this.config.getCliVersion());
var cachePathArchive = path.resolve(cacheDirectory, hash + '.tar.gz');
var cachePathNotArchived = path.resolve(cacheDirectory, hash);

// Check if local cache of dependencies exists
var cacheArchiveExists = fs.existsSync(cachePathArchive);
var cacheNotArchivedExists = fs.existsSync(cachePathNotArchived);
if (!this.config.forceRefresh && (cacheArchiveExists || cacheNotArchivedExists)) {
...
```

#### <a name="apidoc.element.npm-cache.jspmConfig.getFileHash"></a>[function <span class="apidocSignatureSpan">npm-cache.jspmConfig.</span>getFileHash ()](#apidoc.element.npm-cache.jspmConfig.getFileHash)
- description and source-code
```javascript
function getConfigurationHash() {
    return md5(JSON.stringify({
        'package.json => jspm': getPackageJson().jspm,
        'config.js': getProjectFileContents(configFile)
    }));
}
```
- example usage
```shell
...

  async.each(
    managers,
    function calculateHash (managerName) {
      var managerConfig = require(availableManagers[managerName]);
      managerConfig.cacheDirectory = opts.cacheDirectory;

      var hash = managerConfig.getFileHash(managerConfig.configPath);
      console.log(hash);
    }
  );
};


// Recursively lists files in directory up to maxDepth
...
```



# <a name="apidoc.module.npm-cache.logger"></a>[module npm-cache.logger](#apidoc.module.npm-cache.logger)

#### <a name="apidoc.element.npm-cache.logger.logError"></a>[function <span class="apidocSignatureSpan">npm-cache.logger.</span>logError (errorMessage)](#apidoc.element.npm-cache.logger.logError)
- description and source-code
```javascript
logError = function (errorMessage) {
  console.log('[npm-cache] [ERROR] ' + errorMessage);
}
```
- example usage
```shell
...
      manager.loadDependencies(callback);
    },
    function onInstalled (error) {
      if (error === null) {
        logger.logInfo('successfully installed all dependencies');
        process.exit(0);
      } else {
        logger.logError('error installing dependencies');
        process.exit(1);
      }
    }
  );
};

var reportHash = function (opts) {
...
```

#### <a name="apidoc.element.npm-cache.logger.logInfo"></a>[function <span class="apidocSignatureSpan">npm-cache.logger.</span>logInfo (message)](#apidoc.element.npm-cache.logger.logInfo)
- description and source-code
```javascript
logInfo = function (message) {
  console.log('[npm-cache] [INFO] ' + message);
}
```
- example usage
```shell
...

  var npmCacheArgs = ParseUtils.getNpmCacheArgs();
  parser.parse(npmCacheArgs);
};

// Creates cache directory if it does not exist yet
var prepareCacheDirectory = function (cacheDirectory) {
  logger.logInfo('using ' + cacheDirectory + ' as cache directory');
  if (! fs.existsSync(cacheDirectory)) {
    // create directory if it doesn't exist
    fs.mkdirsSync(cacheDirectory);
    logger.logInfo('creating cache directory');
  }
};
...
```



# <a name="apidoc.module.npm-cache.npmConfig"></a>[module npm-cache.npmConfig](#apidoc.module.npm-cache.npmConfig)

#### <a name="apidoc.element.npm-cache.npmConfig.getCliVersion"></a>[function <span class="apidocSignatureSpan">npm-cache.npmConfig.</span>getCliVersion ()](#apidoc.element.npm-cache.npmConfig.getCliVersion)
- description and source-code
```javascript
function getNpmVersion() {
  return shell.exec('npm --version', {silent: true}).output.trim();
}
```
- example usage
```shell
...
}

// Get hash of dependency config file
var hash = this.config.getFileHash(this.config.configPath);
hash = md5(cacheVersion + hash);
this.cacheLogInfo('hash of ' + this.config.configPath + ': ' + hash);
// cachePath is absolute path to where local cache of dependencies is located
var cacheDirectory = path.resolve(this.config.cacheDirectory, this.config.cliName, this.config.getCliVersion());
var cachePathArchive = path.resolve(cacheDirectory, hash + '.tar.gz');
var cachePathNotArchived = path.resolve(cacheDirectory, hash);

// Check if local cache of dependencies exists
var cacheArchiveExists = fs.existsSync(cachePathArchive);
var cacheNotArchivedExists = fs.existsSync(cachePathNotArchived);
if (!this.config.forceRefresh && (cacheArchiveExists || cacheNotArchivedExists)) {
...
```

#### <a name="apidoc.element.npm-cache.npmConfig.getFileHash"></a>[function <span class="apidocSignatureSpan">npm-cache.npmConfig.</span>getFileHash (filePath)](#apidoc.element.npm-cache.npmConfig.getFileHash)
- description and source-code
```javascript
function getFileHash(filePath) {
  var json = JSON.parse(fs.readFileSync(filePath));
  return md5(JSON.stringify({
    dependencies: json.dependencies,
    devDependencies: json.devDependencies
  }));
}
```
- example usage
```shell
...

  async.each(
    managers,
    function calculateHash (managerName) {
      var managerConfig = require(availableManagers[managerName]);
      managerConfig.cacheDirectory = opts.cacheDirectory;

      var hash = managerConfig.getFileHash(managerConfig.configPath);
      console.log(hash);
    }
  );
};


// Recursively lists files in directory up to maxDepth
...
```



# <a name="apidoc.module.npm-cache.parseUtils"></a>[module npm-cache.parseUtils](#apidoc.module.npm-cache.parseUtils)

#### <a name="apidoc.element.npm-cache.parseUtils.getManagerArgs"></a>[function <span class="apidocSignatureSpan">npm-cache.parseUtils.</span>getManagerArgs ()](#apidoc.element.npm-cache.parseUtils.getManagerArgs)
- description and source-code
```javascript
getManagerArgs = function () {
  var managers = {};
  var allArguments = process.argv.slice(3); // strip off 'node', 'index.js', and 'install' from arguments list
  var availableManagers = CacheDependencyManager.getAvailableManagers();
  var currManager = null;

  // First determine which managers were requested by looking at command line arguments
  _.forEach(
    allArguments,
    function addManagerArgument (argument) {
      if (argument in availableManagers) {
        managers[argument] = '';
        currManager = argument;
      } else if (currManager !== null) {
        managers[currManager] += argument + ' ';
      }
    }
  );

  // If no managers were specified, try installing everything by default!
  if (_.isEmpty(managers)) {
    // add all keys from available managers as keys here
    _.forEach(
      CacheDependencyManager.getAvailableDefaultManagers(),
      function addManager (managerPath, manager) {
        managers[manager] = '';
      }
    );
  }

  return managers;
}
```
- example usage
```shell
...
// npm-cache command handlers

// main method for installing specified dependencies
var installDependencies = function (opts) {
prepareCacheDirectory(opts.cacheDirectory);

var availableManagers = CacheDependencyManager.getAvailableManagers();
var managerArguments = ParseUtils.getManagerArgs();
var managers = Object.keys(managerArguments);

async.each(
  managers,
  function startManager (managerName, callback) {
    var managerConfig = require(availableManagers[managerName]);
    managerConfig.cacheDirectory = opts.cacheDirectory;
...
```

#### <a name="apidoc.element.npm-cache.parseUtils.getNpmCacheArgs"></a>[function <span class="apidocSignatureSpan">npm-cache.parseUtils.</span>getNpmCacheArgs ()](#apidoc.element.npm-cache.parseUtils.getNpmCacheArgs)
- description and source-code
```javascript
getNpmCacheArgs = function () {
  var npmCacheArgs = [];

  var availableManagers = CacheDependencyManager.getAvailableManagers();

  var allArguments = process.argv.slice(2);
  for (var i = 0; i < allArguments.length; i++) {
    var currArgument = allArguments[i];
    if (currArgument in availableManagers) {
      break;
    } else {
      npmCacheArgs.push(currArgument);
    }
  }
  return npmCacheArgs;
}
```
- example usage
```shell
...
  '\tnpm-cache install --forceRefresh  bower\t# force installing dependencies from package manager without cache',
  '\tnpm-cache install --noArchive npm\t# do not compress/archive the cached dependencies',
  '\tnpm-cache clean\t# cleans out all cached files in cache directory',
  '\tnpm-cache hash\t# reports the current working hash'
];
parser.help(examples.join('\n'));

var npmCacheArgs = ParseUtils.getNpmCacheArgs();
parser.parse(npmCacheArgs);
};

// Creates cache directory if it does not exist yet
var prepareCacheDirectory = function (cacheDirectory) {
logger.logInfo('using ' + cacheDirectory + ' as cache directory');
if (! fs.existsSync(cacheDirectory)) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
