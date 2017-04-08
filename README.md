# api documentation for  [fs.extra (v1.3.2)](https://github.com/coolaj86/utile-fs)  [![npm package](https://img.shields.io/npm/v/npmdoc-fs.extra.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fs.extra) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fs.extra.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fs.extra)
#### fs.move and fs.copy for Node.JS

[![NPM](https://nodei.co/npm/fs.extra.png?downloads=true)](https://www.npmjs.com/package/fs.extra)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fs.extra/build/screenCapture.buildNpmdoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-fs.extra%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fs.extra/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fs.extra/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fs.extra/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "AJ ONeal",
        "email": "awesome@coolaj86@.com",
        "url": "http://coolaj86.com/"
    },
    "bugs": {
        "url": "https://github.com/coolaj86/utile-fs/issues"
    },
    "dependencies": {
        "fs-extra": "~0.6.1",
        "mkdirp": "~0.3.5",
        "walk": "^2.3.9"
    },
    "description": "fs.move and fs.copy for Node.JS",
    "devDependencies": {
        "sequence": "~2.2.1"
    },
    "directories": {},
    "dist": {
        "shasum": "dd023f93013bee24531f1b33514c37b20fd93349",
        "tarball": "https://registry.npmjs.org/fs.extra/-/fs.extra-1.3.2.tgz"
    },
    "engines": {
        "node": "*"
    },
    "homepage": "https://github.com/coolaj86/utile-fs",
    "licenses": [
        {
            "type": "MIT",
            "url": "http://www.opensource.org/licenses/mit-license.php"
        },
        {
            "type": "Apache License, Version 2.0",
            "url": "http://www.apache.org/licenses/LICENSE-2.0"
        }
    ],
    "main": "fs.extra",
    "maintainers": [
        {
            "name": "coolaj86",
            "email": "coolaj86@gmail.com"
        }
    ],
    "name": "fs.extra",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/coolaj86/utile-fs.git"
    },
    "scripts": {
        "test": "node test.js"
    },
    "version": "1.3.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fs.extra](#apidoc.module.fs.extra)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>FileReadStream (path, options)](#apidoc.element.fs.extra.FileReadStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>FileWriteStream (path, options)](#apidoc.element.fs.extra.FileWriteStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>ReadStream (path, options)](#apidoc.element.fs.extra.ReadStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs.extra.Stats)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>WriteStream (path, options)](#apidoc.element.fs.extra.WriteStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>_toUnixTimestamp (time)](#apidoc.element.fs.extra._toUnixTimestamp)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>access (path, mode, callback)](#apidoc.element.fs.extra.access)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>accessSync (path, mode)](#apidoc.element.fs.extra.accessSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>appendFile (path, data, options, callback_)](#apidoc.element.fs.extra.appendFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>appendFileSync (path, data, options)](#apidoc.element.fs.extra.appendFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>chmod (path, mode, callback)](#apidoc.element.fs.extra.chmod)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>chmodSync (path, mode)](#apidoc.element.fs.extra.chmodSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>chown (path, uid, gid, callback)](#apidoc.element.fs.extra.chown)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>chownSync (path, uid, gid)](#apidoc.element.fs.extra.chownSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>close (fd, callback)](#apidoc.element.fs.extra.close)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>closeSync (fd)](#apidoc.element.fs.extra.closeSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>copy (src, dst, opts, cb)](#apidoc.element.fs.extra.copy)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>copyRecursive (src, dst, cb)](#apidoc.element.fs.extra.copyRecursive)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>createFile (file, callback)](#apidoc.element.fs.extra.createFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>createFileSync (file)](#apidoc.element.fs.extra.createFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>createReadStream (path, options)](#apidoc.element.fs.extra.createReadStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>createWriteStream (path, options)](#apidoc.element.fs.extra.createWriteStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>delete (dir, cb)](#apidoc.element.fs.extra.delete)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>deleteSync (dir)](#apidoc.element.fs.extra.deleteSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>exists (path, callback)](#apidoc.element.fs.extra.exists)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>existsSync (path)](#apidoc.element.fs.extra.existsSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>extra.ReadStream (path, options)](#apidoc.element.fs.extra.extra.ReadStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>extra.Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs.extra.extra.Stats)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>extra.WriteStream (path, options)](#apidoc.element.fs.extra.extra.WriteStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>extra.mkdirs (p, mode, f, made)](#apidoc.element.fs.extra.extra.mkdirs)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fchmod (fd, mode, callback)](#apidoc.element.fs.extra.fchmod)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fchmodSync (fd, mode)](#apidoc.element.fs.extra.fchmodSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fchown (fd, uid, gid, callback)](#apidoc.element.fs.extra.fchown)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fchownSync (fd, uid, gid)](#apidoc.element.fs.extra.fchownSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fdatasync (fd, callback)](#apidoc.element.fs.extra.fdatasync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fdatasyncSync (fd)](#apidoc.element.fs.extra.fdatasyncSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fstat (fd, callback)](#apidoc.element.fs.extra.fstat)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fstatSync (fd)](#apidoc.element.fs.extra.fstatSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fsync (fd, callback)](#apidoc.element.fs.extra.fsync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>fsyncSync (fd)](#apidoc.element.fs.extra.fsyncSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>ftruncate (fd, len, callback)](#apidoc.element.fs.extra.ftruncate)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>ftruncateSync (fd, len)](#apidoc.element.fs.extra.ftruncateSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>futimes (fd, atime, mtime, callback)](#apidoc.element.fs.extra.futimes)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>futimesSync (fd, atime, mtime)](#apidoc.element.fs.extra.futimesSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>link (existingPath, newPath, callback)](#apidoc.element.fs.extra.link)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>linkSync (existingPath, newPath)](#apidoc.element.fs.extra.linkSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>lstat (path, callback)](#apidoc.element.fs.extra.lstat)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>lstatSync (path)](#apidoc.element.fs.extra.lstatSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdir (path, mode, callback)](#apidoc.element.fs.extra.mkdir)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdirRecursive (p, mode, f, made)](#apidoc.element.fs.extra.mkdirRecursive)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdirRecursiveSync (p, mode, made)](#apidoc.element.fs.extra.mkdirRecursiveSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdirSync (path, mode)](#apidoc.element.fs.extra.mkdirSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdirp (p, mode, f, made)](#apidoc.element.fs.extra.mkdirp)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdirpSync (p, mode, made)](#apidoc.element.fs.extra.mkdirpSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdirs (p, mode, f, made)](#apidoc.element.fs.extra.mkdirs)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdirsSync (p, mode, made)](#apidoc.element.fs.extra.mkdirsSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdtemp (prefix, options, callback)](#apidoc.element.fs.extra.mkdtemp)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdtempSync (prefix, options)](#apidoc.element.fs.extra.mkdtempSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>move (src, dst, cb)](#apidoc.element.fs.extra.move)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>open (path, flags, mode, callback_)](#apidoc.element.fs.extra.open)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>openSync (path, flags, mode)](#apidoc.element.fs.extra.openSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>outputFile (file, data, encoding, callback)](#apidoc.element.fs.extra.outputFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>outputFileSync (file, data, encoding)](#apidoc.element.fs.extra.outputFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>outputJSON (file, data, callback)](#apidoc.element.fs.extra.outputJSON)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>outputJSONSync (file, data)](#apidoc.element.fs.extra.outputJSONSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>outputJson (file, data, callback)](#apidoc.element.fs.extra.outputJson)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>outputJsonSync (file, data)](#apidoc.element.fs.extra.outputJsonSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>read (fd, buffer, offset, length, position, callback)](#apidoc.element.fs.extra.read)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readFile (path, options, callback_)](#apidoc.element.fs.extra.readFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readFileSync (path, options)](#apidoc.element.fs.extra.readFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readJSON (file, callback)](#apidoc.element.fs.extra.readJSON)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readJSONFile (file, callback)](#apidoc.element.fs.extra.readJSONFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readJSONFileSync (file)](#apidoc.element.fs.extra.readJSONFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readJSONSync (file)](#apidoc.element.fs.extra.readJSONSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readJson (file, callback)](#apidoc.element.fs.extra.readJson)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readJsonFile (file, callback)](#apidoc.element.fs.extra.readJsonFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readJsonFileSync (file)](#apidoc.element.fs.extra.readJsonFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readJsonSync (file)](#apidoc.element.fs.extra.readJsonSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readSync (fd, buffer, offset, length, position)](#apidoc.element.fs.extra.readSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readdir (path, options, callback)](#apidoc.element.fs.extra.readdir)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readdirSync (path, options)](#apidoc.element.fs.extra.readdirSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readlink (path, options, callback)](#apidoc.element.fs.extra.readlink)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>readlinkSync (path, options)](#apidoc.element.fs.extra.readlinkSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>realpath (p, options, callback)](#apidoc.element.fs.extra.realpath)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>realpathSync (p, options)](#apidoc.element.fs.extra.realpathSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>remove (dir, cb)](#apidoc.element.fs.extra.remove)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>removeSync (dir)](#apidoc.element.fs.extra.removeSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>rename (oldPath, newPath, callback)](#apidoc.element.fs.extra.rename)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>renameSync (oldPath, newPath)](#apidoc.element.fs.extra.renameSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>rmdir (path, callback)](#apidoc.element.fs.extra.rmdir)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>rmdirSync (path)](#apidoc.element.fs.extra.rmdirSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>rmrf (dir, cb)](#apidoc.element.fs.extra.rmrf)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>rmrfSync (dir)](#apidoc.element.fs.extra.rmrfSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>stat (path, callback)](#apidoc.element.fs.extra.stat)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>statSync (path)](#apidoc.element.fs.extra.statSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>symlink (target, path, type_, callback_)](#apidoc.element.fs.extra.symlink)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>symlinkSync (target, path, type)](#apidoc.element.fs.extra.symlinkSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>touch ()](#apidoc.element.fs.extra.touch)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>touchSync ()](#apidoc.element.fs.extra.touchSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>truncate (path, len, callback)](#apidoc.element.fs.extra.truncate)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>truncateSync (path, len)](#apidoc.element.fs.extra.truncateSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>unlink (path, callback)](#apidoc.element.fs.extra.unlink)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>unlinkSync (path)](#apidoc.element.fs.extra.unlinkSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>unwatchFile (filename, listener)](#apidoc.element.fs.extra.unwatchFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>utimes (path, atime, mtime, callback)](#apidoc.element.fs.extra.utimes)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>utimesSync (path, atime, mtime)](#apidoc.element.fs.extra.utimesSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>walk (path, opts)](#apidoc.element.fs.extra.walk)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>watch (filename, options, listener)](#apidoc.element.fs.extra.watch)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>watchFile (filename, options, listener)](#apidoc.element.fs.extra.watchFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>write (fd, buffer, offset, length, position, callback)](#apidoc.element.fs.extra.write)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeFile (path, data, options, callback_)](#apidoc.element.fs.extra.writeFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeFileSync (path, data, options)](#apidoc.element.fs.extra.writeFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeJSON (file, obj, callback)](#apidoc.element.fs.extra.writeJSON)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeJSONFile (file, obj, callback)](#apidoc.element.fs.extra.writeJSONFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeJSONFileSync (file, obj)](#apidoc.element.fs.extra.writeJSONFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeJSONSync (file, obj)](#apidoc.element.fs.extra.writeJSONSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeJson (file, obj, callback)](#apidoc.element.fs.extra.writeJson)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeJsonFile (file, obj, callback)](#apidoc.element.fs.extra.writeJsonFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeJsonFileSync (file, obj)](#apidoc.element.fs.extra.writeJsonFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeJsonSync (file, obj)](#apidoc.element.fs.extra.writeJsonSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>writeSync (fd, buffer, offset, length, position)](#apidoc.element.fs.extra.writeSync)
1.  number <span class="apidocSignatureSpan">fs.extra.</span>F_OK
1.  number <span class="apidocSignatureSpan">fs.extra.</span>R_OK
1.  number <span class="apidocSignatureSpan">fs.extra.</span>W_OK
1.  number <span class="apidocSignatureSpan">fs.extra.</span>X_OK
1.  object <span class="apidocSignatureSpan">fs.extra.</span>constants
1.  object <span class="apidocSignatureSpan">fs.extra.</span>extra.ReadStream.prototype
1.  object <span class="apidocSignatureSpan">fs.extra.</span>extra.Stats.prototype
1.  object <span class="apidocSignatureSpan">fs.extra.</span>extra.WriteStream.prototype
1.  object <span class="apidocSignatureSpan">fs.extra.</span>extra.jsonfile
1.  object <span class="apidocSignatureSpan">fs.extra.</span>jsonfile

#### [module fs.extra.ReadStream](#apidoc.module.fs.extra.ReadStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>ReadStream (path, options)](#apidoc.element.fs.extra.ReadStream.ReadStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.ReadStream.</span>super_ (options)](#apidoc.element.fs.extra.ReadStream.super_)

#### [module fs.extra.ReadStream.prototype](#apidoc.module.fs.extra.ReadStream.prototype)
1.  [function <span class="apidocSignatureSpan">fs.extra.ReadStream.prototype.</span>_read (n)](#apidoc.element.fs.extra.ReadStream.prototype._read)
1.  [function <span class="apidocSignatureSpan">fs.extra.ReadStream.prototype.</span>close (cb)](#apidoc.element.fs.extra.ReadStream.prototype.close)
1.  [function <span class="apidocSignatureSpan">fs.extra.ReadStream.prototype.</span>destroy ()](#apidoc.element.fs.extra.ReadStream.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">fs.extra.ReadStream.prototype.</span>open ()](#apidoc.element.fs.extra.ReadStream.prototype.open)

#### [module fs.extra.Stats](#apidoc.module.fs.extra.Stats)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs.extra.Stats.Stats)

#### [module fs.extra.Stats.prototype](#apidoc.module.fs.extra.Stats.prototype)
1.  [function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>_checkModeProperty (property)](#apidoc.element.fs.extra.Stats.prototype._checkModeProperty)
1.  [function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isBlockDevice ()](#apidoc.element.fs.extra.Stats.prototype.isBlockDevice)
1.  [function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isCharacterDevice ()](#apidoc.element.fs.extra.Stats.prototype.isCharacterDevice)
1.  [function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isDirectory ()](#apidoc.element.fs.extra.Stats.prototype.isDirectory)
1.  [function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isFIFO ()](#apidoc.element.fs.extra.Stats.prototype.isFIFO)
1.  [function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isFile ()](#apidoc.element.fs.extra.Stats.prototype.isFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isSocket ()](#apidoc.element.fs.extra.Stats.prototype.isSocket)
1.  [function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isSymbolicLink ()](#apidoc.element.fs.extra.Stats.prototype.isSymbolicLink)

#### [module fs.extra.WriteStream](#apidoc.module.fs.extra.WriteStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>WriteStream (path, options)](#apidoc.element.fs.extra.WriteStream.WriteStream)
1.  [function <span class="apidocSignatureSpan">fs.extra.WriteStream.</span>super_ (options)](#apidoc.element.fs.extra.WriteStream.super_)

#### [module fs.extra.WriteStream.prototype](#apidoc.module.fs.extra.WriteStream.prototype)
1.  [function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>_write (data, encoding, cb)](#apidoc.element.fs.extra.WriteStream.prototype._write)
1.  [function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>_writev (data, cb)](#apidoc.element.fs.extra.WriteStream.prototype._writev)
1.  [function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>close (cb)](#apidoc.element.fs.extra.WriteStream.prototype.close)
1.  [function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>destroy ()](#apidoc.element.fs.extra.WriteStream.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>destroySoon (chunk, encoding, cb)](#apidoc.element.fs.extra.WriteStream.prototype.destroySoon)
1.  [function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>open ()](#apidoc.element.fs.extra.WriteStream.prototype.open)

#### [module fs.extra.jsonfile](#apidoc.module.fs.extra.jsonfile)
1.  [function <span class="apidocSignatureSpan">fs.extra.jsonfile.</span>readFile (file, callback)](#apidoc.element.fs.extra.jsonfile.readFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.jsonfile.</span>readFileSync (file)](#apidoc.element.fs.extra.jsonfile.readFileSync)
1.  [function <span class="apidocSignatureSpan">fs.extra.jsonfile.</span>writeFile (file, obj, callback)](#apidoc.element.fs.extra.jsonfile.writeFile)
1.  [function <span class="apidocSignatureSpan">fs.extra.jsonfile.</span>writeFileSync (file, obj)](#apidoc.element.fs.extra.jsonfile.writeFileSync)
1.  number <span class="apidocSignatureSpan">fs.extra.jsonfile.</span>spaces

#### [module fs.extra.mkdirs](#apidoc.module.fs.extra.mkdirs)
1.  [function <span class="apidocSignatureSpan">fs.extra.</span>mkdirs (p, mode, f, made)](#apidoc.element.fs.extra.mkdirs.mkdirs)
1.  [function <span class="apidocSignatureSpan">fs.extra.mkdirs.</span>mkdirP (p, mode, f, made)](#apidoc.element.fs.extra.mkdirs.mkdirP)
1.  [function <span class="apidocSignatureSpan">fs.extra.mkdirs.</span>mkdirp (p, mode, f, made)](#apidoc.element.fs.extra.mkdirs.mkdirp)
1.  [function <span class="apidocSignatureSpan">fs.extra.mkdirs.</span>sync (p, mode, made)](#apidoc.element.fs.extra.mkdirs.sync)



# <a name="apidoc.module.fs.extra"></a>[module fs.extra](#apidoc.module.fs.extra)

#### <a name="apidoc.element.fs.extra.FileReadStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>FileReadStream (path, options)](#apidoc.element.fs.extra.FileReadStream)
- description and source-code
```javascript
function ReadStream(path, options) {
  if (!(this instanceof ReadStream))
    return new ReadStream(path, options);

  if (options === undefined)
    options = {};
  else if (typeof options === 'string')
    options = { encoding: options };
  else if (options === null || typeof options !== 'object')
    throw new TypeError('"options" argument must be a string or an object');

  // a little bit bigger buffer and water marks by default
  options = Object.create(options);
  if (options.highWaterMark === undefined)
    options.highWaterMark = 64 * 1024;

  Readable.call(this, options);

  this.path = path;
  this.fd = options.fd === undefined ? null : options.fd;
  this.flags = options.flags === undefined ? 'r' : options.flags;
  this.mode = options.mode === undefined ? 0o666 : options.mode;

  this.start = options.start;
  this.end = options.end;
  this.autoClose = options.autoClose === undefined ? true : options.autoClose;
  this.pos = undefined;
  this.bytesRead = 0;

  if (this.start !== undefined) {
    if (typeof this.start !== 'number') {
      throw new TypeError('"start" option must be a Number');
    }
    if (this.end === undefined) {
      this.end = Infinity;
    } else if (typeof this.end !== 'number') {
      throw new TypeError('"end" option must be a Number');
    }

    if (this.start > this.end) {
      throw new Error('"start" option must be <= "end" option');
    }

    this.pos = this.start;
  }

  if (typeof this.fd !== 'number')
    this.open();

  this.on('end', function() {
    if (this.autoClose) {
      this.destroy();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.FileWriteStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>FileWriteStream (path, options)](#apidoc.element.fs.extra.FileWriteStream)
- description and source-code
```javascript
function WriteStream(path, options) {
  if (!(this instanceof WriteStream))
    return new WriteStream(path, options);

  if (options === undefined)
    options = {};
  else if (typeof options === 'string')
    options = { encoding: options };
  else if (options === null || typeof options !== 'object')
    throw new TypeError('"options" argument must be a string or an object');

  options = Object.create(options);

  Writable.call(this, options);

  this.path = path;
  this.fd = options.fd === undefined ? null : options.fd;
  this.flags = options.flags === undefined ? 'w' : options.flags;
  this.mode = options.mode === undefined ? 0o666 : options.mode;

  this.start = options.start;
  this.autoClose = options.autoClose === undefined ? true : !!options.autoClose;
  this.pos = undefined;
  this.bytesWritten = 0;

  if (this.start !== undefined) {
    if (typeof this.start !== 'number') {
      throw new TypeError('"start" option must be a Number');
    }
    if (this.start < 0) {
      throw new Error('"start" must be >= zero');
    }

    this.pos = this.start;
  }

  if (options.encoding)
    this.setDefaultEncoding(options.encoding);

  if (typeof this.fd !== 'number')
    this.open();

  // dispose on finish.
  this.once('finish', function() {
    if (this.autoClose) {
      this.close();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.ReadStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>ReadStream (path, options)](#apidoc.element.fs.extra.ReadStream)
- description and source-code
```javascript
function ReadStream(path, options) {
  if (!(this instanceof ReadStream))
    return new ReadStream(path, options);

  if (options === undefined)
    options = {};
  else if (typeof options === 'string')
    options = { encoding: options };
  else if (options === null || typeof options !== 'object')
    throw new TypeError('"options" argument must be a string or an object');

  // a little bit bigger buffer and water marks by default
  options = Object.create(options);
  if (options.highWaterMark === undefined)
    options.highWaterMark = 64 * 1024;

  Readable.call(this, options);

  this.path = path;
  this.fd = options.fd === undefined ? null : options.fd;
  this.flags = options.flags === undefined ? 'r' : options.flags;
  this.mode = options.mode === undefined ? 0o666 : options.mode;

  this.start = options.start;
  this.end = options.end;
  this.autoClose = options.autoClose === undefined ? true : options.autoClose;
  this.pos = undefined;
  this.bytesRead = 0;

  if (this.start !== undefined) {
    if (typeof this.start !== 'number') {
      throw new TypeError('"start" option must be a Number');
    }
    if (this.end === undefined) {
      this.end = Infinity;
    } else if (typeof this.end !== 'number') {
      throw new TypeError('"end" option must be a Number');
    }

    if (this.start > this.end) {
      throw new Error('"start" option must be <= "end" option');
    }

    this.pos = this.start;
  }

  if (typeof this.fd !== 'number')
    this.open();

  this.on('end', function() {
    if (this.autoClose) {
      this.destroy();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.Stats"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs.extra.Stats)
- description and source-code
```javascript
function Stats( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec) {
  this.dev = dev;
  this.mode = mode;
  this.nlink = nlink;
  this.uid = uid;
  this.gid = gid;
  this.rdev = rdev;
  this.blksize = blksize;
  this.ino = ino;
  this.size = size;
  this.blocks = blocks;
  this.atime = new Date(atim_msec);
  this.mtime = new Date(mtim_msec);
  this.ctime = new Date(ctim_msec);
  this.birthtime = new Date(birthtim_msec);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.WriteStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>WriteStream (path, options)](#apidoc.element.fs.extra.WriteStream)
- description and source-code
```javascript
function WriteStream(path, options) {
  if (!(this instanceof WriteStream))
    return new WriteStream(path, options);

  if (options === undefined)
    options = {};
  else if (typeof options === 'string')
    options = { encoding: options };
  else if (options === null || typeof options !== 'object')
    throw new TypeError('"options" argument must be a string or an object');

  options = Object.create(options);

  Writable.call(this, options);

  this.path = path;
  this.fd = options.fd === undefined ? null : options.fd;
  this.flags = options.flags === undefined ? 'w' : options.flags;
  this.mode = options.mode === undefined ? 0o666 : options.mode;

  this.start = options.start;
  this.autoClose = options.autoClose === undefined ? true : !!options.autoClose;
  this.pos = undefined;
  this.bytesWritten = 0;

  if (this.start !== undefined) {
    if (typeof this.start !== 'number') {
      throw new TypeError('"start" option must be a Number');
    }
    if (this.start < 0) {
      throw new Error('"start" must be >= zero');
    }

    this.pos = this.start;
  }

  if (options.encoding)
    this.setDefaultEncoding(options.encoding);

  if (typeof this.fd !== 'number')
    this.open();

  // dispose on finish.
  this.once('finish', function() {
    if (this.autoClose) {
      this.close();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra._toUnixTimestamp"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>_toUnixTimestamp (time)](#apidoc.element.fs.extra._toUnixTimestamp)
- description and source-code
```javascript
function toUnixTimestamp(time) {
  if (typeof time === 'string' && +time == time) {
    return +time;
  }
  if (typeof time === 'number') {
    if (!Number.isFinite(time) || time < 0) {
      return Date.now() / 1000;
    }
    return time;
  }
  if (util.isDate(time)) {
    // convert to 123.456 UNIX timestamp
    return time.getTime() / 1000;
  }
  throw new Error('Cannot parse time: ' + time);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.access"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>access (path, mode, callback)](#apidoc.element.fs.extra.access)
- description and source-code
```javascript
access = function (path, mode, callback) {
  if (typeof mode === 'function') {
    callback = mode;
    mode = fs.F_OK;
  } else if (typeof callback !== 'function') {
    throw new TypeError('"callback" argument must be a function');
  }

  if (!nullCheck(path, callback))
    return;

  mode = mode | 0;
  var req = new FSReqWrap();
  req.oncomplete = makeCallback(callback);
  binding.access(pathModule._makeLong(path), mode, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.accessSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>accessSync (path, mode)](#apidoc.element.fs.extra.accessSync)
- description and source-code
```javascript
accessSync = function (path, mode) {
  nullCheck(path);

  if (mode === undefined)
    mode = fs.F_OK;
  else
    mode = mode | 0;

  binding.access(pathModule._makeLong(path), mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.appendFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>appendFile (path, data, options, callback_)](#apidoc.element.fs.extra.appendFile)
- description and source-code
```javascript
appendFile = function (path, data, options, callback_) {
  var callback = maybeCallback(arguments[arguments.length - 1]);

  if (!options || typeof options === 'function') {
    options = { encoding: 'utf8', mode: 0o666, flag: 'a' };
  } else if (typeof options === 'string') {
    options = { encoding: options, mode: 0o666, flag: 'a' };
  } else if (typeof options !== 'object') {
    throwOptionsError(options);
  }

  if (!options.flag)
    options = util._extend({ flag: 'a' }, options);

  // force append behavior when using a supplied file descriptor
  if (isFd(path))
    options.flag = 'a';

  fs.writeFile(path, data, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.appendFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>appendFileSync (path, data, options)](#apidoc.element.fs.extra.appendFileSync)
- description and source-code
```javascript
appendFileSync = function (path, data, options) {
  if (!options) {
    options = { encoding: 'utf8', mode: 0o666, flag: 'a' };
  } else if (typeof options === 'string') {
    options = { encoding: options, mode: 0o666, flag: 'a' };
  } else if (typeof options !== 'object') {
    throwOptionsError(options);
  }

  if (!options.flag)
    options = util._extend({ flag: 'a' }, options);

  // force append behavior when using a supplied file descriptor
  if (isFd(path))
    options.flag = 'a';

  fs.writeFileSync(path, data, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.chmod"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>chmod (path, mode, callback)](#apidoc.element.fs.extra.chmod)
- description and source-code
```javascript
chmod = function (path, mode, callback) {
  callback = makeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.chmod(pathModule._makeLong(path),
                modeNum(mode),
                req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.chmodSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>chmodSync (path, mode)](#apidoc.element.fs.extra.chmodSync)
- description and source-code
```javascript
chmodSync = function (path, mode) {
  nullCheck(path);
  return binding.chmod(pathModule._makeLong(path), modeNum(mode));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.chown"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>chown (path, uid, gid, callback)](#apidoc.element.fs.extra.chown)
- description and source-code
```javascript
chown = function (path, uid, gid, callback) {
  callback = makeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.chown(pathModule._makeLong(path), uid, gid, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.chownSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>chownSync (path, uid, gid)](#apidoc.element.fs.extra.chownSync)
- description and source-code
```javascript
chownSync = function (path, uid, gid) {
  nullCheck(path);
  return binding.chown(pathModule._makeLong(path), uid, gid);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.close"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>close (fd, callback)](#apidoc.element.fs.extra.close)
- description and source-code
```javascript
close = function (fd, callback) {
  var req = new FSReqWrap();
  req.oncomplete = makeCallback(callback);
  binding.close(fd, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.closeSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>closeSync (fd)](#apidoc.element.fs.extra.closeSync)
- description and source-code
```javascript
closeSync = function (fd) {
  return binding.close(fd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.copy"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>copy (src, dst, opts, cb)](#apidoc.element.fs.extra.copy)
- description and source-code
```javascript
function copy(src, dst, opts, cb) {
  if ('function' === typeof opts) {
    cb = opts;
    opts = null;
  }
  opts = opts || {};

  function copyHelper(err) {
    var is
      , os
      ;

    if (!err && !(opts.replace || opts.overwrite)) {
      return cb(new Error("File " + dst + " exists."));
    }

    fs.stat(src, function (err, stat) {
      if (err) {
        return cb(err);
      }

      is = fs.createReadStream(src);
      os = fs.createWriteStream(dst);

      is.pipe(os);
      os.on('close', function (err) {
        if (err) {
          return cb(err);
        }

        fs.utimes(dst, stat.atime, stat.mtime, cb);
      });
    });
  }

  cb = cb || noop;
  fs.stat(dst, copyHelper);
}
```
- example usage
```shell
...

fs.copy
===

Creates an 'fs.readStream' and 'fs.writeStream' and uses 'util.pump' to efficiently copy.

'''javascript
fs.copy('foo.txt', 'bar.txt', { replace: false }, function (err) {
  if (err) {
    // i.e. file already exists or can't write to directory
    throw err;
  }

  console.log("Copied 'foo.txt' to 'bar.txt');
});
...
```

#### <a name="apidoc.element.fs.extra.copyRecursive"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>copyRecursive (src, dst, cb)](#apidoc.element.fs.extra.copyRecursive)
- description and source-code
```javascript
function run(src, dst, cb) {

  function syncDirs(cb, src, dst) {
    var walker = fsWalk(src)
      ;

    walker.on('directory', function (root, stat, next) {
      var newDir = path.join(dst, root.substr(src.length + 1), stat.name)
        ;

      fsMkdirp(newDir, stat.mode, next);
    });

    walker.on('end', function () {
      cb();
    });
  }

  function syncFiles(cb, src, dst) {
    var walker = fsWalk(src)
      ;

    walker.on('file', function (root, stat, next) {
      var curFile = path.join(root, stat.name)
        , newFile = path.join(dst, root.substr(src.length + 1), stat.name)
        ;

      fsCopy(curFile, newFile, function (err) {
        if (err) {
          cb(err);
          return;
        }
        next();
      });
    });

    walker.on('end', function () {
      cb();
    });
  }

  dst = path.resolve(process.cwd(), dst);

  fsMkdirp(path.join(dst), function () {
    fs.realpath(src, function (err, rsrc) {
      fs.realpath(dst, function (err, rdst) {
        syncDirs(function () {
          syncFiles(cb, rsrc, rdst);
        }, rsrc, rdst);
      });
    });
  });
}
```
- example usage
```shell
...

fs.copyRecursive
===

Basically a local 'rsync', uses 'fs.copy' to recursively copy files and folders (with correct permissions).

'''javascript
fs.copyRecursive('./foo', './bar', function (err) {
  if (err) {
    throw err;
  }

  console.log("Copied './foo' to './bar');
});
'''
...
```

#### <a name="apidoc.element.fs.extra.createFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>createFile (file, callback)](#apidoc.element.fs.extra.createFile)
- description and source-code
```javascript
function createFile(file, callback) {
  function makeFile() {
    fs.writeFile(file, '', function(err) {
      if (err)
        callback(err)
      else
        callback(null);
    })
  }

  exists(file, function(fileExists) {
    if (fileExists)
      return callback(null);
    else {
      var dir = path.dirname(file);

      exists(dir, function(dirExists) {
        if (!dirExists) {
          mkdir.mkdirs(dir, function(err) {
            if (err)
              callback(err)
            else
              makeFile();
          })
        } else {
          makeFile();
        }
      })
    }
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.createFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>createFileSync (file)](#apidoc.element.fs.extra.createFileSync)
- description and source-code
```javascript
function createFileSync(file) {
  if (existsSync(file))
    return;

  var dir = path.dirname(file);
  if (!existsSync(dir))
    mkdir.mkdirsSync(dir);

  fs.writeFileSync(file, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.createReadStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>createReadStream (path, options)](#apidoc.element.fs.extra.createReadStream)
- description and source-code
```javascript
createReadStream = function (path, options) {
  return new ReadStream(path, options);
}
```
- example usage
```shell
...
      }

      fs.stat(src, function (err, stat) {
if (err) {
  return cb(err);
}

is = fs.createReadStream(src);
os = fs.createWriteStream(dst);

is.pipe(os);
os.on('close', function (err) {
  if (err) {
    return cb(err);
  }
...
```

#### <a name="apidoc.element.fs.extra.createWriteStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>createWriteStream (path, options)](#apidoc.element.fs.extra.createWriteStream)
- description and source-code
```javascript
createWriteStream = function (path, options) {
  return new WriteStream(path, options);
}
```
- example usage
```shell
...

      fs.stat(src, function (err, stat) {
if (err) {
  return cb(err);
}

is = fs.createReadStream(src);
os = fs.createWriteStream(dst);

is.pipe(os);
os.on('close', function (err) {
  if (err) {
    return cb(err);
  }
...
```

#### <a name="apidoc.element.fs.extra.delete"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>delete (dir, cb)](#apidoc.element.fs.extra.delete)
- description and source-code
```javascript
function rmrf(dir, cb) {
    if (cb != null) {
        return rimraf(dir, cb);
    } else {
        return rimraf(dir, (function() {}));
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.deleteSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>deleteSync (dir)](#apidoc.element.fs.extra.deleteSync)
- description and source-code
```javascript
function rmrfSync(dir) {
    return rimraf.sync(dir);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.exists"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>exists (path, callback)](#apidoc.element.fs.extra.exists)
- description and source-code
```javascript
exists = function (path, callback) {
  if (!nullCheck(path, cb)) return;
  var req = new FSReqWrap();
  req.oncomplete = cb;
  binding.stat(pathModule._makeLong(path), req);
  function cb(err, stats) {
    if (callback) callback(err ? false : true);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.existsSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>existsSync (path)](#apidoc.element.fs.extra.existsSync)
- description and source-code
```javascript
existsSync = function (path) {
  try {
    nullCheck(path);
    binding.stat(pathModule._makeLong(path), statValues);
    return true;
  } catch (e) {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.extra.ReadStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>extra.ReadStream (path, options)](#apidoc.element.fs.extra.extra.ReadStream)
- description and source-code
```javascript
function ReadStream(path, options) {
  if (!(this instanceof ReadStream))
    return new ReadStream(path, options);

  if (options === undefined)
    options = {};
  else if (typeof options === 'string')
    options = { encoding: options };
  else if (options === null || typeof options !== 'object')
    throw new TypeError('"options" argument must be a string or an object');

  // a little bit bigger buffer and water marks by default
  options = Object.create(options);
  if (options.highWaterMark === undefined)
    options.highWaterMark = 64 * 1024;

  Readable.call(this, options);

  this.path = path;
  this.fd = options.fd === undefined ? null : options.fd;
  this.flags = options.flags === undefined ? 'r' : options.flags;
  this.mode = options.mode === undefined ? 0o666 : options.mode;

  this.start = options.start;
  this.end = options.end;
  this.autoClose = options.autoClose === undefined ? true : options.autoClose;
  this.pos = undefined;
  this.bytesRead = 0;

  if (this.start !== undefined) {
    if (typeof this.start !== 'number') {
      throw new TypeError('"start" option must be a Number');
    }
    if (this.end === undefined) {
      this.end = Infinity;
    } else if (typeof this.end !== 'number') {
      throw new TypeError('"end" option must be a Number');
    }

    if (this.start > this.end) {
      throw new Error('"start" option must be <= "end" option');
    }

    this.pos = this.start;
  }

  if (typeof this.fd !== 'number')
    this.open();

  this.on('end', function() {
    if (this.autoClose) {
      this.destroy();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.extra.Stats"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>extra.Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs.extra.extra.Stats)
- description and source-code
```javascript
function Stats( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec) {
  this.dev = dev;
  this.mode = mode;
  this.nlink = nlink;
  this.uid = uid;
  this.gid = gid;
  this.rdev = rdev;
  this.blksize = blksize;
  this.ino = ino;
  this.size = size;
  this.blocks = blocks;
  this.atime = new Date(atim_msec);
  this.mtime = new Date(mtim_msec);
  this.ctime = new Date(ctim_msec);
  this.birthtime = new Date(birthtim_msec);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.extra.WriteStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>extra.WriteStream (path, options)](#apidoc.element.fs.extra.extra.WriteStream)
- description and source-code
```javascript
function WriteStream(path, options) {
  if (!(this instanceof WriteStream))
    return new WriteStream(path, options);

  if (options === undefined)
    options = {};
  else if (typeof options === 'string')
    options = { encoding: options };
  else if (options === null || typeof options !== 'object')
    throw new TypeError('"options" argument must be a string or an object');

  options = Object.create(options);

  Writable.call(this, options);

  this.path = path;
  this.fd = options.fd === undefined ? null : options.fd;
  this.flags = options.flags === undefined ? 'w' : options.flags;
  this.mode = options.mode === undefined ? 0o666 : options.mode;

  this.start = options.start;
  this.autoClose = options.autoClose === undefined ? true : !!options.autoClose;
  this.pos = undefined;
  this.bytesWritten = 0;

  if (this.start !== undefined) {
    if (typeof this.start !== 'number') {
      throw new TypeError('"start" option must be a Number');
    }
    if (this.start < 0) {
      throw new Error('"start" must be >= zero');
    }

    this.pos = this.start;
  }

  if (options.encoding)
    this.setDefaultEncoding(options.encoding);

  if (typeof this.fd !== 'number')
    this.open();

  // dispose on finish.
  this.once('finish', function() {
    if (this.autoClose) {
      this.close();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.extra.mkdirs"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>extra.mkdirs (p, mode, f, made)](#apidoc.element.fs.extra.extra.mkdirs)
- description and source-code
```javascript
function mkdirP(p, mode, f, made) {
    if (typeof mode === 'function' || mode === undefined) {
        f = mode;
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    var cb = f || function () {};
    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    fs.mkdir(p, mode, function (er) {
        if (!er) {
            made = made || p;
            return cb(null, made);
        }
        switch (er.code) {
            case 'ENOENT':
                mkdirP(path.dirname(p), mode, function (er, made) {
                    if (er) cb(er, made);
                    else mkdirP(p, mode, cb, made);
                });
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                fs.stat(p, function (er2, stat) {
                    // if the stat fails, then that's super weird.
                    // let the original error be the failure reason.
                    if (er2 || !stat.isDirectory()) cb(er, made)
                    else cb(null, made);
                });
                break;
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fchmod"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fchmod (fd, mode, callback)](#apidoc.element.fs.extra.fchmod)
- description and source-code
```javascript
fchmod = function (fd, mode, callback) {
  var req = new FSReqWrap();
  req.oncomplete = makeCallback(callback);
  binding.fchmod(fd, modeNum(mode), req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fchmodSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fchmodSync (fd, mode)](#apidoc.element.fs.extra.fchmodSync)
- description and source-code
```javascript
fchmodSync = function (fd, mode) {
  return binding.fchmod(fd, modeNum(mode));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fchown"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fchown (fd, uid, gid, callback)](#apidoc.element.fs.extra.fchown)
- description and source-code
```javascript
fchown = function (fd, uid, gid, callback) {
  var req = new FSReqWrap();
  req.oncomplete = makeCallback(callback);
  binding.fchown(fd, uid, gid, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fchownSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fchownSync (fd, uid, gid)](#apidoc.element.fs.extra.fchownSync)
- description and source-code
```javascript
fchownSync = function (fd, uid, gid) {
  return binding.fchown(fd, uid, gid);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fdatasync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fdatasync (fd, callback)](#apidoc.element.fs.extra.fdatasync)
- description and source-code
```javascript
fdatasync = function (fd, callback) {
  var req = new FSReqWrap();
  req.oncomplete = makeCallback(callback);
  binding.fdatasync(fd, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fdatasyncSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fdatasyncSync (fd)](#apidoc.element.fs.extra.fdatasyncSync)
- description and source-code
```javascript
fdatasyncSync = function (fd) {
  return binding.fdatasync(fd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fstat"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fstat (fd, callback)](#apidoc.element.fs.extra.fstat)
- description and source-code
```javascript
fstat = function (fd, callback) {
  var req = new FSReqWrap();
  req.oncomplete = makeCallback(callback);
  binding.fstat(fd, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fstatSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fstatSync (fd)](#apidoc.element.fs.extra.fstatSync)
- description and source-code
```javascript
fstatSync = function (fd) {
  binding.fstat(fd, statValues);
  return statsFromValues();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fsync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fsync (fd, callback)](#apidoc.element.fs.extra.fsync)
- description and source-code
```javascript
fsync = function (fd, callback) {
  var req = new FSReqWrap();
  req.oncomplete = makeCallback(callback);
  binding.fsync(fd, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.fsyncSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>fsyncSync (fd)](#apidoc.element.fs.extra.fsyncSync)
- description and source-code
```javascript
fsyncSync = function (fd) {
  return binding.fsync(fd);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.ftruncate"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>ftruncate (fd, len, callback)](#apidoc.element.fs.extra.ftruncate)
- description and source-code
```javascript
ftruncate = function (fd, len, callback) {
  if (typeof len === 'function') {
    callback = len;
    len = 0;
  } else if (len === undefined) {
    len = 0;
  }
  var req = new FSReqWrap();
  req.oncomplete = makeCallback(callback);
  binding.ftruncate(fd, len, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.ftruncateSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>ftruncateSync (fd, len)](#apidoc.element.fs.extra.ftruncateSync)
- description and source-code
```javascript
ftruncateSync = function (fd, len) {
  if (len === undefined) {
    len = 0;
  }
  return binding.ftruncate(fd, len);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.futimes"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>futimes (fd, atime, mtime, callback)](#apidoc.element.fs.extra.futimes)
- description and source-code
```javascript
futimes = function (fd, atime, mtime, callback) {
  atime = toUnixTimestamp(atime);
  mtime = toUnixTimestamp(mtime);
  var req = new FSReqWrap();
  req.oncomplete = makeCallback(callback);
  binding.futimes(fd, atime, mtime, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.futimesSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>futimesSync (fd, atime, mtime)](#apidoc.element.fs.extra.futimesSync)
- description and source-code
```javascript
futimesSync = function (fd, atime, mtime) {
  atime = toUnixTimestamp(atime);
  mtime = toUnixTimestamp(mtime);
  binding.futimes(fd, atime, mtime);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.link"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>link (existingPath, newPath, callback)](#apidoc.element.fs.extra.link)
- description and source-code
```javascript
link = function (existingPath, newPath, callback) {
  callback = makeCallback(callback);
  if (!nullCheck(existingPath, callback)) return;
  if (!nullCheck(newPath, callback)) return;

  var req = new FSReqWrap();
  req.oncomplete = callback;

  binding.link(pathModule._makeLong(existingPath),
               pathModule._makeLong(newPath),
               req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.linkSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>linkSync (existingPath, newPath)](#apidoc.element.fs.extra.linkSync)
- description and source-code
```javascript
linkSync = function (existingPath, newPath) {
  nullCheck(existingPath);
  nullCheck(newPath);
  return binding.link(pathModule._makeLong(existingPath),
                      pathModule._makeLong(newPath));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.lstat"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>lstat (path, callback)](#apidoc.element.fs.extra.lstat)
- description and source-code
```javascript
lstat = function (path, callback) {
  callback = makeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.lstat(pathModule._makeLong(path), req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.lstatSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>lstatSync (path)](#apidoc.element.fs.extra.lstatSync)
- description and source-code
```javascript
lstatSync = function (path) {
  nullCheck(path);
  binding.lstat(pathModule._makeLong(path), statValues);
  return statsFromValues();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdir"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdir (path, mode, callback)](#apidoc.element.fs.extra.mkdir)
- description and source-code
```javascript
mkdir = function (path, mode, callback) {
  if (typeof mode === 'function') callback = mode;
  callback = makeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.mkdir(pathModule._makeLong(path),
                modeNum(mode, 0o777),
                req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdirRecursive"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdirRecursive (p, mode, f, made)](#apidoc.element.fs.extra.mkdirRecursive)
- description and source-code
```javascript
function mkdirP(p, mode, f, made) {
    if (typeof mode === 'function' || mode === undefined) {
        f = mode;
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    var cb = f || function () {};
    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    fs.mkdir(p, mode, function (er) {
        if (!er) {
            made = made || p;
            return cb(null, made);
        }
        switch (er.code) {
            case 'ENOENT':
                mkdirP(path.dirname(p), mode, function (er, made) {
                    if (er) cb(er, made);
                    else mkdirP(p, mode, cb, made);
                });
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                fs.stat(p, function (er2, stat) {
                    // if the stat fails, then that's super weird.
                    // let the original error be the failure reason.
                    if (er2 || !stat.isDirectory()) cb(er, made)
                    else cb(null, made);
                });
                break;
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdirRecursiveSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdirRecursiveSync (p, mode, made)](#apidoc.element.fs.extra.mkdirRecursiveSync)
- description and source-code
```javascript
function sync(p, mode, made) {
    if (mode === undefined) {
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    try {
        fs.mkdirSync(p, mode);
        made = made || p;
    }
    catch (err0) {
        switch (err0.code) {
            case 'ENOENT' :
                made = sync(path.dirname(p), mode, made);
                sync(p, mode, made);
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                var stat;
                try {
                    stat = fs.statSync(p);
                }
                catch (err1) {
                    throw err0;
                }
                if (!stat.isDirectory()) throw err0;
                break;
        }
    }

    return made;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdirSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdirSync (path, mode)](#apidoc.element.fs.extra.mkdirSync)
- description and source-code
```javascript
mkdirSync = function (path, mode) {
  nullCheck(path);
  return binding.mkdir(pathModule._makeLong(path),
                       modeNum(mode, 0o777));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdirp"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdirp (p, mode, f, made)](#apidoc.element.fs.extra.mkdirp)
- description and source-code
```javascript
function mkdirP(p, mode, f, made) {
    if (typeof mode === 'function' || mode === undefined) {
        f = mode;
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    var cb = f || function () {};
    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    fs.mkdir(p, mode, function (er) {
        if (!er) {
            made = made || p;
            return cb(null, made);
        }
        switch (er.code) {
            case 'ENOENT':
                mkdirP(path.dirname(p), mode, function (er, made) {
                    if (er) cb(er, made);
                    else mkdirP(p, mode, cb, made);
                });
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                fs.stat(p, function (er2, stat) {
                    // if the stat fails, then that's super weird.
                    // let the original error be the failure reason.
                    if (er2 || !stat.isDirectory()) cb(er, made)
                    else cb(null, made);
                });
                break;
        }
    });
}
```
- example usage
```shell
...

fs.mkdirRecursive
===

Included from <https://github.com/substack/node-mkdirp>

'''javascript
// fs.mkdirp(path, mode=(0777 & (~process.umask())), cb);

fs.mkdirp('/tmp/foo/bar/baz', function (err) {
if (err) {
  console.error(err);
} else {
  console.log('pow!')
}
...
```

#### <a name="apidoc.element.fs.extra.mkdirpSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdirpSync (p, mode, made)](#apidoc.element.fs.extra.mkdirpSync)
- description and source-code
```javascript
function sync(p, mode, made) {
    if (mode === undefined) {
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    try {
        fs.mkdirSync(p, mode);
        made = made || p;
    }
    catch (err0) {
        switch (err0.code) {
            case 'ENOENT' :
                made = sync(path.dirname(p), mode, made);
                sync(p, mode, made);
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                var stat;
                try {
                    stat = fs.statSync(p);
                }
                catch (err1) {
                    throw err0;
                }
                if (!stat.isDirectory()) throw err0;
                break;
        }
    }

    return made;
}
```
- example usage
```shell
...

fs.mkdirRecursiveSync
===

Included from <https://github.com/substack/node-mkdirp>

'''javascript
// fs.mkdirpSync(path, mode=(0777 & (~process.umask())));

try {
  fs.mkdirpSync('/tmp/foo/bar/baz');
} catch(e) {
  throw e;
}
'''
...
```

#### <a name="apidoc.element.fs.extra.mkdirs"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdirs (p, mode, f, made)](#apidoc.element.fs.extra.mkdirs)
- description and source-code
```javascript
function mkdirP(p, mode, f, made) {
    if (typeof mode === 'function' || mode === undefined) {
        f = mode;
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    var cb = f || function () {};
    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    fs.mkdir(p, mode, function (er) {
        if (!er) {
            made = made || p;
            return cb(null, made);
        }
        switch (er.code) {
            case 'ENOENT':
                mkdirP(path.dirname(p), mode, function (er, made) {
                    if (er) cb(er, made);
                    else mkdirP(p, mode, cb, made);
                });
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                fs.stat(p, function (er2, stat) {
                    // if the stat fails, then that's super weird.
                    // let the original error be the failure reason.
                    if (er2 || !stat.isDirectory()) cb(er, made)
                    else cb(null, made);
                });
                break;
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdirsSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdirsSync (p, mode, made)](#apidoc.element.fs.extra.mkdirsSync)
- description and source-code
```javascript
function sync(p, mode, made) {
    if (mode === undefined) {
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    try {
        fs.mkdirSync(p, mode);
        made = made || p;
    }
    catch (err0) {
        switch (err0.code) {
            case 'ENOENT' :
                made = sync(path.dirname(p), mode, made);
                sync(p, mode, made);
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                var stat;
                try {
                    stat = fs.statSync(p);
                }
                catch (err1) {
                    throw err0;
                }
                if (!stat.isDirectory()) throw err0;
                break;
        }
    }

    return made;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdtemp"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdtemp (prefix, options, callback)](#apidoc.element.fs.extra.mkdtemp)
- description and source-code
```javascript
mkdtemp = function (prefix, options, callback) {
  if (!prefix || typeof prefix !== 'string')
    throw new TypeError('filename prefix is required');

  options = options || {};
  if (typeof options === 'function') {
    callback = options;
    options = {};
  } else if (typeof options === 'string') {
    options = {encoding: options};
  }
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');

  callback = makeCallback(callback);
  if (!nullCheck(prefix, callback)) {
    return;
  }

  var req = new FSReqWrap();
  req.oncomplete = callback;

  binding.mkdtemp(prefix + 'XXXXXX', options.encoding, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdtempSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdtempSync (prefix, options)](#apidoc.element.fs.extra.mkdtempSync)
- description and source-code
```javascript
mkdtempSync = function (prefix, options) {
  if (!prefix || typeof prefix !== 'string')
    throw new TypeError('filename prefix is required');

  options = options || {};
  if (typeof options === 'string')
    options = {encoding: options};
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');
  nullCheck(prefix);

  return binding.mkdtemp(prefix + 'XXXXXX', options.encoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.move"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>move (src, dst, cb)](#apidoc.element.fs.extra.move)
- description and source-code
```javascript
function move(src, dst, cb) {
  function copyIfFailed(err) {
    if (!err) {
      return cb(null);
    }
    fsCopy(src, dst, function(err) {
      if (!err) {
        // TODO
        // should we revert the copy if the unlink fails?
        fs.unlink(src, cb);
      } else {
        cb(err);
      }
    });
  }

  cb = cb || noop;
  fs.stat(dst, function (err) {
    if (!err) {
      return cb(new Error("File " + dst + " exists."));
    }
    fs.rename(src, dst, copyIfFailed);
  });
}
```
- example usage
```shell
...

fs.move
===

Attempts 'fs.rename', then tries 'fs.copy' + 'fs.unlink' before failing.

'''javascript
fs.move('foo.txt', 'bar.txt', function (err) {
  if (err) {
    throw err;
  }

  console.log("Moved 'foo.txt' to 'bar.txt');
});
'''
...
```

#### <a name="apidoc.element.fs.extra.open"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>open (path, flags, mode, callback_)](#apidoc.element.fs.extra.open)
- description and source-code
```javascript
open = function (path, flags, mode, callback_) {
  var callback = makeCallback(arguments[arguments.length - 1]);
  mode = modeNum(mode, 0o666);

  if (!nullCheck(path, callback)) return;

  var req = new FSReqWrap();
  req.oncomplete = callback;

  binding.open(pathModule._makeLong(path),
               stringToFlags(flags),
               mode,
               req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.openSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>openSync (path, flags, mode)](#apidoc.element.fs.extra.openSync)
- description and source-code
```javascript
openSync = function (path, flags, mode) {
  mode = modeNum(mode, 0o666);
  nullCheck(path);
  return binding.open(pathModule._makeLong(path), stringToFlags(flags), mode);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.outputFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>outputFile (file, data, encoding, callback)](#apidoc.element.fs.extra.outputFile)
- description and source-code
```javascript
function outputFile(file, data, encoding, callback) {
  if (typeof encoding === 'function') {
    callback = encoding
    encoding = 'utf8'
  }

  var dir = path.dirname(file)
  exists(dir, function(itDoes) {
    if (itDoes) return fs.writeFile(file, data, encoding, callback)

    mkdir.mkdirs(dir, function(err) {
      if (err) return callback(err)

      fs.writeFile(file, data, encoding, callback)
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.outputFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>outputFileSync (file, data, encoding)](#apidoc.element.fs.extra.outputFileSync)
- description and source-code
```javascript
function outputFileSync(file, data, encoding) {
  var dir = path.dirname(file)
  if (existsSync(dir)) return fs.writeFileSync.apply(fs, arguments)
  mkdir.mkdirsSync(dir)
  fs.writeFileSync.apply(fs, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.outputJSON"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>outputJSON (file, data, callback)](#apidoc.element.fs.extra.outputJSON)
- description and source-code
```javascript
outputJSON = function (file, data, callback) {
  var dir = path.dirname(file)

  fs.exists(dir, function(itDoes) {
    if (itDoes) return jsonFile.writeFile(file, data, callback)

    mkdir.mkdirs(dir, function(err) {
      if (err) return callback(err)
      jsonFile.writeFile(file, data, callback)
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.outputJSONSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>outputJSONSync (file, data)](#apidoc.element.fs.extra.outputJSONSync)
- description and source-code
```javascript
outputJSONSync = function (file, data) {
  var dir = path.dirname(file)

  if (!fs.existsSync(dir))
    mkdir.mkdirsSync(dir)

  jsonFile.writeFileSync(file, data)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.outputJson"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>outputJson (file, data, callback)](#apidoc.element.fs.extra.outputJson)
- description and source-code
```javascript
outputJson = function (file, data, callback) {
  var dir = path.dirname(file)

  fs.exists(dir, function(itDoes) {
    if (itDoes) return jsonFile.writeFile(file, data, callback)

    mkdir.mkdirs(dir, function(err) {
      if (err) return callback(err)
      jsonFile.writeFile(file, data, callback)
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.outputJsonSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>outputJsonSync (file, data)](#apidoc.element.fs.extra.outputJsonSync)
- description and source-code
```javascript
outputJsonSync = function (file, data) {
  var dir = path.dirname(file)

  if (!fs.existsSync(dir))
    mkdir.mkdirsSync(dir)

  jsonFile.writeFileSync(file, data)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.read"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>read (fd, buffer, offset, length, position, callback)](#apidoc.element.fs.extra.read)
- description and source-code
```javascript
read = function (fd, buffer, offset, length, position, callback) {
  if (!(buffer instanceof Buffer)) {
    // legacy string interface (fd, length, position, encoding, callback)
    readWarned = printDeprecation('fs.read\'s legacy String interface ' +
                                  'is deprecated. Use the Buffer API as ' +
                                  'mentioned in the documentation instead.',
                                  readWarned);
    const cb = arguments[4];
    const encoding = arguments[3];

    assertEncoding(encoding);

    position = arguments[2];
    length = arguments[1];
    buffer = Buffer.allocUnsafe(length);
    offset = 0;

    callback = function(err, bytesRead) {
      if (!cb) return;
      if (err) return cb(err);

      if (bytesRead > 0) {
        tryToStringWithEnd(buffer, encoding, bytesRead, cb);
      } else {
        (cb)(err, '', bytesRead);
      }
    };
  }

  if (length === 0) {
    return process.nextTick(function() {
      callback && callback(null, 0, buffer);
    });
  }

  function wrapper(err, bytesRead) {
    // Retain a reference to buffer so that it can't be GC'ed too soon.
    callback && callback(err, bytesRead || 0, buffer);
  }

  var req = new FSReqWrap();
  req.oncomplete = wrapper;

  binding.read(fd, buffer, offset, length, position, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readFile (path, options, callback_)](#apidoc.element.fs.extra.readFile)
- description and source-code
```javascript
readFile = function (path, options, callback_) {
  var callback = maybeCallback(arguments[arguments.length - 1]);

  if (!options || typeof options === 'function') {
    options = { encoding: null, flag: 'r' };
  } else if (typeof options === 'string') {
    options = { encoding: options, flag: 'r' };
  } else if (typeof options !== 'object') {
    throwOptionsError(options);
  }

  var encoding = options.encoding;
  assertEncoding(encoding);

  var flag = options.flag || 'r';

  if (!nullCheck(path, callback))
    return;

  var context = new ReadFileContext(callback, encoding);
  context.isUserFd = isFd(path); // file descriptor ownership
  var req = new FSReqWrap();
  req.context = context;
  req.oncomplete = readFileAfterOpen;

  if (context.isUserFd) {
    process.nextTick(function() {
      req.oncomplete(null, path);
    });
    return;
  }

  binding.open(pathModule._makeLong(path),
               stringToFlags(flag),
               0o666,
               req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readFileSync (path, options)](#apidoc.element.fs.extra.readFileSync)
- description and source-code
```javascript
readFileSync = function (path, options) {
  if (!options) {
    options = { encoding: null, flag: 'r' };
  } else if (typeof options === 'string') {
    options = { encoding: options, flag: 'r' };
  } else if (typeof options !== 'object') {
    throwOptionsError(options);
  }

  var encoding = options.encoding;
  assertEncoding(encoding);

  var flag = options.flag || 'r';
  var isUserFd = isFd(path); // file descriptor ownership
  var fd = isUserFd ? path : fs.openSync(path, flag, 0o666);

  var st = tryStatSync(fd, isUserFd);
  var size = st.isFile() ? st.size : 0;
  var pos = 0;
  var buffer; // single buffer with file data
  var buffers; // list for when size is unknown

  if (size === 0) {
    buffers = [];
  } else {
    buffer = tryCreateBuffer(size, fd, isUserFd);
  }

  var bytesRead;

  if (size !== 0) {
    do {
      bytesRead = tryReadSync(fd, isUserFd, buffer, pos, size - pos);
      pos += bytesRead;
    } while (bytesRead !== 0 && pos < size);
  } else {
    do {
      // the kernel lies about many files.
      // Go ahead and try to read some bytes.
      buffer = Buffer.allocUnsafe(8192);
      bytesRead = tryReadSync(fd, isUserFd, buffer, 0, 8192);
      if (bytesRead !== 0) {
        buffers.push(buffer.slice(0, bytesRead));
      }
      pos += bytesRead;
    } while (bytesRead !== 0);
  }

  if (!isUserFd)
    fs.closeSync(fd);

  if (size === 0) {
    // data was collected into the buffers list.
    buffer = Buffer.concat(buffers, pos);
  } else if (pos < size) {
    buffer = buffer.slice(0, pos);
  }

  if (encoding) buffer = buffer.toString(encoding);
  return buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readJSON"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readJSON (file, callback)](#apidoc.element.fs.extra.readJSON)
- description and source-code
```javascript
readJSON = function (file, callback) {
  fs.readFile(file, 'utf8', function(err, data) {
    if (err) return callback(err, null);

    try {
      var obj = JSON.parse(data);
      callback(null, obj);
    } catch (err2) {
      callback(err2, null);
    }
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readJSONFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readJSONFile (file, callback)](#apidoc.element.fs.extra.readJSONFile)
- description and source-code
```javascript
readJSONFile = function (file, callback) {
  fs.readFile(file, 'utf8', function(err, data) {
    if (err) return callback(err, null);

    try {
      var obj = JSON.parse(data);
      callback(null, obj);
    } catch (err2) {
      callback(err2, null);
    }
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readJSONFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readJSONFileSync (file)](#apidoc.element.fs.extra.readJSONFileSync)
- description and source-code
```javascript
readJSONFileSync = function (file) {
  return JSON.parse(fs.readFileSync(file, 'utf8'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readJSONSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readJSONSync (file)](#apidoc.element.fs.extra.readJSONSync)
- description and source-code
```javascript
readJSONSync = function (file) {
  return JSON.parse(fs.readFileSync(file, 'utf8'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readJson"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readJson (file, callback)](#apidoc.element.fs.extra.readJson)
- description and source-code
```javascript
readJson = function (file, callback) {
  fs.readFile(file, 'utf8', function(err, data) {
    if (err) return callback(err, null);

    try {
      var obj = JSON.parse(data);
      callback(null, obj);
    } catch (err2) {
      callback(err2, null);
    }
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readJsonFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readJsonFile (file, callback)](#apidoc.element.fs.extra.readJsonFile)
- description and source-code
```javascript
readJsonFile = function (file, callback) {
  fs.readFile(file, 'utf8', function(err, data) {
    if (err) return callback(err, null);

    try {
      var obj = JSON.parse(data);
      callback(null, obj);
    } catch (err2) {
      callback(err2, null);
    }
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readJsonFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readJsonFileSync (file)](#apidoc.element.fs.extra.readJsonFileSync)
- description and source-code
```javascript
readJsonFileSync = function (file) {
  return JSON.parse(fs.readFileSync(file, 'utf8'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readJsonSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readJsonSync (file)](#apidoc.element.fs.extra.readJsonSync)
- description and source-code
```javascript
readJsonSync = function (file) {
  return JSON.parse(fs.readFileSync(file, 'utf8'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readSync (fd, buffer, offset, length, position)](#apidoc.element.fs.extra.readSync)
- description and source-code
```javascript
readSync = function (fd, buffer, offset, length, position) {
  var legacy = false;
  var encoding;

  if (!(buffer instanceof Buffer)) {
    // legacy string interface (fd, length, position, encoding, callback)
    readSyncWarned = printDeprecation('fs.readSync\'s legacy String interface' +
                                      'is deprecated. Use the Buffer API as ' +
                                      'mentioned in the documentation instead.',
                                      readSyncWarned);
    legacy = true;
    encoding = arguments[3];

    assertEncoding(encoding);

    position = arguments[2];
    length = arguments[1];
    buffer = Buffer.allocUnsafe(length);

    offset = 0;
  }

  if (length === 0) {
    if (legacy) {
      return ['', 0];
    } else {
      return 0;
    }
  }

  var r = binding.read(fd, buffer, offset, length, position);
  if (!legacy) {
    return r;
  }

  var str = (r > 0) ? buffer.toString(encoding, 0, r) : '';
  return [str, r];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readdir"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readdir (path, options, callback)](#apidoc.element.fs.extra.readdir)
- description and source-code
```javascript
readdir = function (path, options, callback) {
  options = options || {};
  if (typeof options === 'function') {
    callback = options;
    options = {};
  } else if (typeof options === 'string') {
    options = {encoding: options};
  }
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');

  callback = makeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.readdir(pathModule._makeLong(path), options.encoding, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readdirSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readdirSync (path, options)](#apidoc.element.fs.extra.readdirSync)
- description and source-code
```javascript
readdirSync = function (path, options) {
  options = options || {};
  if (typeof options === 'string')
    options = {encoding: options};
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');
  nullCheck(path);
  return binding.readdir(pathModule._makeLong(path), options.encoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readlink"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readlink (path, options, callback)](#apidoc.element.fs.extra.readlink)
- description and source-code
```javascript
readlink = function (path, options, callback) {
  options = options || {};
  if (typeof options === 'function') {
    callback = options;
    options = {};
  } else if (typeof options === 'string') {
    options = {encoding: options};
  }
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');
  callback = makeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.readlink(pathModule._makeLong(path), options.encoding, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.readlinkSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>readlinkSync (path, options)](#apidoc.element.fs.extra.readlinkSync)
- description and source-code
```javascript
readlinkSync = function (path, options) {
  options = options || {};
  if (typeof options === 'string')
    options = {encoding: options};
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');
  nullCheck(path);
  return binding.readlink(pathModule._makeLong(path), options.encoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.realpath"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>realpath (p, options, callback)](#apidoc.element.fs.extra.realpath)
- description and source-code
```javascript
function realpath(p, options, callback) {
  if (typeof callback !== 'function') {
    callback = maybeCallback(options);
    options = {};
  }

  if (!options) {
    options = {};
  } else if (typeof options === 'function') {
    options = {};
  } else if (typeof options === 'string') {
    options = {encoding: options};
  } else if (typeof options !== 'object') {
    throw new TypeError('"options" must be a string or an object');
  }
  if (!nullCheck(p, callback))
    return;

  p = p.toString('utf8');
  p = pathModule.resolve(p);

  const seenLinks = {};
  const knownHard = {};

  // current character position in p
  var pos;
  // the partial path so far, including a trailing slash if any
  var current;
  // the partial path without a trailing slash (except when pointing at a root)
  var base;
  // the partial path scanned in the previous round, with slash
  var previous;

  start();

  function start() {
    // Skip over roots
    var m = splitRootRe.exec(p);
    pos = m[0].length;
    current = m[0];
    base = m[0];
    previous = '';

    // On windows, check that the root exists. On unix there is no need.
    if (isWindows && !knownHard[base]) {
      fs.lstat(base, function(err) {
        if (err) return callback(err);
        knownHard[base] = true;
        LOOP();
      });
    } else {
      process.nextTick(LOOP);
    }
  }

  // walk down the path, swapping out linked pathparts for their real
  // values
  function LOOP() {
    // stop if scanned past end of path
    if (pos >= p.length) {
      return callback(null, encodeRealpathResult(p, options));
    }

    // find the next part
    nextPartRe.lastIndex = pos;
    var result = nextPartRe.exec(p);
    previous = current;
    current += result[0];
    base = previous + result[1];
    pos = nextPartRe.lastIndex;

    // continue if not a symlink
    if (knownHard[base]) {
      return process.nextTick(LOOP);
    }

    return fs.lstat(base, gotStat);
  }

  function gotStat(err, stat) {
    if (err) return callback(err);

    // if not a symlink, skip to the next path part
    if (!stat.isSymbolicLink()) {
      knownHard[base] = true;
      return process.nextTick(LOOP);
    }

    // stat & read the link if not read before
    // call gotTarget as soon as the link target is known
    // dev/ino always return 0 on windows, so skip the check.
    let id;
    if (!isWindows) {
      id = '${stat.dev.toString(32)}:${stat.ino.toString(32)}';
      if (seenLinks.hasOwnProperty(id)) {
        return gotTarget(null, seenLinks[id], base);
      }
    }
    fs.stat(base, function(err) {
      if (err) return callback(err);

      fs.readlink(base, function(err, target) {
        if (!isWindows) seenLinks[id] = target;
        gotTarget(err, target);
      });
    });
  }

  function gotTarget(err, target, base) {
    if (err) return callback(err);

    var resolvedLink = pathModule.resolve(previous, target);
    gotResolvedLink(resolvedLink);
  }

  function gotResolvedLink(resolvedLink) {
    // resolve the link, then start over
    p = pathModule.resolve(resolvedLink, p.slice(pos));
    start();
  }
}
```
- example usage
```shell
...
    cb();
  });
}

dst = path.resolve(process.cwd(), dst);

fsMkdirp(path.join(dst), function () {
  fs.realpath(src, function (err, rsrc) {
    fs.realpath(dst, function (err, rdst) {
      syncDirs(function () {
        syncFiles(cb, rsrc, rdst);
      }, rsrc, rdst);
    });
  });
});
...
```

#### <a name="apidoc.element.fs.extra.realpathSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>realpathSync (p, options)](#apidoc.element.fs.extra.realpathSync)
- description and source-code
```javascript
function realpathSync(p, options) {
  if (!options)
    options = {};
  else if (typeof options === 'string')
    options = {encoding: options};
  else if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');
  nullCheck(p);

  p = p.toString('utf8');
  p = pathModule.resolve(p);

  const seenLinks = {};
  const knownHard = {};
  const cache = options[realpathCacheKey];
  const original = p;

  const maybeCachedResult = cache && cache.get(p);
  if (maybeCachedResult) {
    return maybeCachedResult;
  }

  // current character position in p
  var pos;
  // the partial path so far, including a trailing slash if any
  var current;
  // the partial path without a trailing slash (except when pointing at a root)
  var base;
  // the partial path scanned in the previous round, with slash
  var previous;

  start();

  function start() {
    // Skip over roots
    var m = splitRootRe.exec(p);
    pos = m[0].length;
    current = m[0];
    base = m[0];
    previous = '';

    // On windows, check that the root exists. On unix there is no need.
    if (isWindows && !knownHard[base]) {
      fs.lstatSync(base);
      knownHard[base] = true;
    }
  }

  // walk down the path, swapping out linked pathparts for their real
  // values
  // NB: p.length changes.
  while (pos < p.length) {
    // find the next part
    nextPartRe.lastIndex = pos;
    var result = nextPartRe.exec(p);
    previous = current;
    current += result[0];
    base = previous + result[1];
    pos = nextPartRe.lastIndex;

    // continue if not a symlink
    if (knownHard[base] || (cache && cache.get(base) === base)) {
      continue;
    }

    var resolvedLink;
    const maybeCachedResolved = cache && cache.get(base);
    if (maybeCachedResolved) {
      resolvedLink = maybeCachedResolved;
    } else {
      var stat = fs.lstatSync(base);
      if (!stat.isSymbolicLink()) {
        knownHard[base] = true;
        if (cache) cache.set(base, base);
        continue;
      }

      // read the link if it wasn't read before
      // dev/ino always return 0 on windows, so skip the check.
      let linkTarget = null;
      let id;
      if (!isWindows) {
        id = '${stat.dev.toString(32)}:${stat.ino.toString(32)}';
        if (seenLinks.hasOwnProperty(id)) {
          linkTarget = seenLinks[id];
        }
      }
      if (linkTarget === null) {
        fs.statSync(base);
        linkTarget = fs.readlinkSync(base);
      }
      resolvedLink = pathModule.resolve(previous, linkTarget);

      if (cache) cache.set(base, resolvedLink);
      if (!isWindows) seenLinks[id] = linkTarget;
    }

    // resolve the link, then start over
    p = pathModule.resolve(resolvedLink, p.slice(pos));
    start();
  }

  if (cache) cache.set(original, p);
  return encodeRealpathResult(p, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.remove"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>remove (dir, cb)](#apidoc.element.fs.extra.remove)
- description and source-code
```javascript
function rmrf(dir, cb) {
    if (cb != null) {
        return rimraf(dir, cb);
    } else {
        return rimraf(dir, (function() {}));
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.removeSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>removeSync (dir)](#apidoc.element.fs.extra.removeSync)
- description and source-code
```javascript
function rmrfSync(dir) {
    return rimraf.sync(dir);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.rename"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>rename (oldPath, newPath, callback)](#apidoc.element.fs.extra.rename)
- description and source-code
```javascript
rename = function (oldPath, newPath, callback) {
  callback = makeCallback(callback);
  if (!nullCheck(oldPath, callback)) return;
  if (!nullCheck(newPath, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.rename(pathModule._makeLong(oldPath),
                 pathModule._makeLong(newPath),
                 req);
}
```
- example usage
```shell
...
    }

    cb = cb || noop;
    fs.stat(dst, function (err) {
      if (!err) {
        return cb(new Error("File " + dst + " exists."));
      }
      fs.rename(src, dst, copyIfFailed);
    });
  }

  module.exports = move;
}());
...
```

#### <a name="apidoc.element.fs.extra.renameSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>renameSync (oldPath, newPath)](#apidoc.element.fs.extra.renameSync)
- description and source-code
```javascript
renameSync = function (oldPath, newPath) {
  nullCheck(oldPath);
  nullCheck(newPath);
  return binding.rename(pathModule._makeLong(oldPath),
                        pathModule._makeLong(newPath));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.rmdir"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>rmdir (path, callback)](#apidoc.element.fs.extra.rmdir)
- description and source-code
```javascript
rmdir = function (path, callback) {
  callback = maybeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.rmdir(pathModule._makeLong(path), req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.rmdirSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>rmdirSync (path)](#apidoc.element.fs.extra.rmdirSync)
- description and source-code
```javascript
rmdirSync = function (path) {
  nullCheck(path);
  return binding.rmdir(pathModule._makeLong(path));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.rmrf"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>rmrf (dir, cb)](#apidoc.element.fs.extra.rmrf)
- description and source-code
```javascript
function rmrf(dir, cb) {
    if (cb != null) {
        return rimraf(dir, cb);
    } else {
        return rimraf(dir, (function() {}));
    }
}
```
- example usage
```shell
...
===

Included from <https://github.com/jprichardson/node-fs-extra>

Recursively deletes a directory (like 'rm -rf')

'''javascript
// fs.rmrf(dir, callback);

fs.rmrf('/choose/me/carefully/', function (err) {
  if (err) {
    console.error(err);
  }
});
'''
...
```

#### <a name="apidoc.element.fs.extra.rmrfSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>rmrfSync (dir)](#apidoc.element.fs.extra.rmrfSync)
- description and source-code
```javascript
function rmrfSync(dir) {
    return rimraf.sync(dir);
}
```
- example usage
```shell
...
===

Included from <https://github.com/jprichardson/node-fs-extra>

Recursively deletes a directory (like 'rm -rf')

'''javascript
// fs.rmrfSync(dir);

fs.rmrfSync('/choose/me/carefully/');
'''

fs.walk
===
...
```

#### <a name="apidoc.element.fs.extra.stat"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>stat (path, callback)](#apidoc.element.fs.extra.stat)
- description and source-code
```javascript
stat = function (path, callback) {
  callback = makeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.stat(pathModule._makeLong(path), req);
}
```
- example usage
```shell
...
, os
;

      if (!err && !(opts.replace || opts.overwrite)) {
return cb(new Error("File " + dst + " exists."));
      }

      fs.stat(src, function (err, stat) {
if (err) {
  return cb(err);
}

is = fs.createReadStream(src);
os = fs.createWriteStream(dst);
...
```

#### <a name="apidoc.element.fs.extra.statSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>statSync (path)](#apidoc.element.fs.extra.statSync)
- description and source-code
```javascript
statSync = function (path) {
  nullCheck(path);
  binding.stat(pathModule._makeLong(path), statValues);
  return statsFromValues();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.symlink"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>symlink (target, path, type_, callback_)](#apidoc.element.fs.extra.symlink)
- description and source-code
```javascript
symlink = function (target, path, type_, callback_) {
  var type = (typeof type_ === 'string' ? type_ : null);
  var callback = makeCallback(arguments[arguments.length - 1]);

  if (!nullCheck(target, callback)) return;
  if (!nullCheck(path, callback)) return;

  var req = new FSReqWrap();
  req.oncomplete = callback;

  binding.symlink(preprocessSymlinkDestination(target, type, path),
                  pathModule._makeLong(path),
                  type,
                  req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.symlinkSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>symlinkSync (target, path, type)](#apidoc.element.fs.extra.symlinkSync)
- description and source-code
```javascript
symlinkSync = function (target, path, type) {
  type = (typeof type === 'string' ? type : null);

  nullCheck(target);
  nullCheck(path);

  return binding.symlink(preprocessSymlinkDestination(target, type, path),
                         pathModule._makeLong(path),
                         type);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.touch"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>touch ()](#apidoc.element.fs.extra.touch)
- description and source-code
```javascript
function touch() {
  console.log('fs.touch() is deprecated. Please use fs.createFile().')
  fs.createFile.apply(null, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.touchSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>touchSync ()](#apidoc.element.fs.extra.touchSync)
- description and source-code
```javascript
function touchSync() {
  console.log('fs.touchSync() is deprecated. Please use fs.createFileSync().')
  fs.createFileSync.apply(null, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.truncate"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>truncate (path, len, callback)](#apidoc.element.fs.extra.truncate)
- description and source-code
```javascript
truncate = function (path, len, callback) {
  if (typeof path === 'number') {
    return fs.ftruncate(path, len, callback);
  }
  if (typeof len === 'function') {
    callback = len;
    len = 0;
  } else if (len === undefined) {
    len = 0;
  }

  callback = maybeCallback(callback);
  fs.open(path, 'r+', function(er, fd) {
    if (er) return callback(er);
    var req = new FSReqWrap();
    req.oncomplete = function oncomplete(er) {
      fs.close(fd, function(er2) {
        callback(er || er2);
      });
    };
    binding.ftruncate(fd, len, req);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.truncateSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>truncateSync (path, len)](#apidoc.element.fs.extra.truncateSync)
- description and source-code
```javascript
truncateSync = function (path, len) {
  if (typeof path === 'number') {
    // legacy
    return fs.ftruncateSync(path, len);
  }
  if (len === undefined) {
    len = 0;
  }
  // allow error to be thrown, but still close fd.
  var fd = fs.openSync(path, 'r+');
  var ret;

  try {
    ret = fs.ftruncateSync(fd, len);
  } finally {
    fs.closeSync(fd);
  }
  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.unlink"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>unlink (path, callback)](#apidoc.element.fs.extra.unlink)
- description and source-code
```javascript
unlink = function (path, callback) {
  callback = makeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.unlink(pathModule._makeLong(path), req);
}
```
- example usage
```shell
...
  if (!err) {
    return cb(null);
  }
  fsCopy(src, dst, function(err) {
    if (!err) {
      // TODO
      // should we revert the copy if the unlink fails?
      fs.unlink(src, cb);
    } else {
      cb(err);
    }
  });
}

cb = cb || noop;
...
```

#### <a name="apidoc.element.fs.extra.unlinkSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>unlinkSync (path)](#apidoc.element.fs.extra.unlinkSync)
- description and source-code
```javascript
unlinkSync = function (path) {
  nullCheck(path);
  return binding.unlink(pathModule._makeLong(path));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.unwatchFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>unwatchFile (filename, listener)](#apidoc.element.fs.extra.unwatchFile)
- description and source-code
```javascript
unwatchFile = function (filename, listener) {
  nullCheck(filename);
  filename = pathModule.resolve(filename);
  var stat = statWatchers.get(filename);

  if (stat === undefined) return;

  if (typeof listener === 'function') {
    stat.removeListener('change', listener);
  } else {
    stat.removeAllListeners('change');
  }

  if (stat.listenerCount('change') === 0) {
    stat.stop();
    statWatchers.delete(filename);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.utimes"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>utimes (path, atime, mtime, callback)](#apidoc.element.fs.extra.utimes)
- description and source-code
```javascript
utimes = function (path, atime, mtime, callback) {
  callback = makeCallback(callback);
  if (!nullCheck(path, callback)) return;
  var req = new FSReqWrap();
  req.oncomplete = callback;
  binding.utimes(pathModule._makeLong(path),
                 toUnixTimestamp(atime),
                 toUnixTimestamp(mtime),
                 req);
}
```
- example usage
```shell
...

      is.pipe(os);
      os.on('close', function (err) {
        if (err) {
          return cb(err);
        }

        fs.utimes(dst, stat.atime, stat.mtime, cb);
      });
    });
  }

  cb = cb || noop;
  fs.stat(dst, copyHelper);
}
...
```

#### <a name="apidoc.element.fs.extra.utimesSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>utimesSync (path, atime, mtime)](#apidoc.element.fs.extra.utimesSync)
- description and source-code
```javascript
utimesSync = function (path, atime, mtime) {
  nullCheck(path);
  atime = toUnixTimestamp(atime);
  mtime = toUnixTimestamp(mtime);
  binding.utimes(pathModule._makeLong(path), atime, mtime);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.walk"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>walk (path, opts)](#apidoc.element.fs.extra.walk)
- description and source-code
```javascript
walk = function (path, opts) {
  return new Walker(path, opts, false);
}
```
- example usage
```shell
...

fs.walk
===

See <https://github.com/coolaj86/node-walk>

'''javascript
var walker = fs.walk(dir)
;

// file, files, directory, directories
walker.on("file", function (root, stat, next) {
var filepath = path.join(root, stat.name)
  ;
...
```

#### <a name="apidoc.element.fs.extra.watch"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>watch (filename, options, listener)](#apidoc.element.fs.extra.watch)
- description and source-code
```javascript
watch = function (filename, options, listener) {
  nullCheck(filename);

  options = options || {};
  if (typeof options === 'function') {
    listener = options;
    options = {};
  } else if (typeof options === 'string') {
    options = {encoding: options};
  }
  if (typeof options !== 'object')
    throw new TypeError('"options" must be a string or an object');

  if (options.persistent === undefined) options.persistent = true;
  if (options.recursive === undefined) options.recursive = false;

  const watcher = new FSWatcher();
  watcher.start(filename,
                options.persistent,
                options.recursive,
                options.encoding);

  if (listener) {
    watcher.addListener('change', listener);
  }

  return watcher;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.watchFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>watchFile (filename, options, listener)](#apidoc.element.fs.extra.watchFile)
- description and source-code
```javascript
watchFile = function (filename, options, listener) {
  nullCheck(filename);
  filename = pathModule.resolve(filename);
  var stat;

  var defaults = {
    // Poll interval in milliseconds. 5007 is what libev used to use. It's
    // a little on the slow side but let's stick with it for now to keep
    // behavioral changes to a minimum.
    interval: 5007,
    persistent: true
  };

  if (options !== null && typeof options === 'object') {
    options = util._extend(defaults, options);
  } else {
    listener = options;
    options = defaults;
  }

  if (typeof listener !== 'function') {
    throw new Error('"watchFile()" requires a listener function');
  }

  stat = statWatchers.get(filename);

  if (stat === undefined) {
    stat = new StatWatcher();
    stat.start(filename, options.persistent, options.interval);
    statWatchers.set(filename, stat);
  }

  stat.addListener('change', listener);
  return stat;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.write"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>write (fd, buffer, offset, length, position, callback)](#apidoc.element.fs.extra.write)
- description and source-code
```javascript
write = function (fd, buffer, offset, length, position, callback) {
  function wrapper(err, written) {
    // Retain a reference to buffer so that it can't be GC'ed too soon.
    callback(err, written || 0, buffer);
  }

  var req = new FSReqWrap();
  req.oncomplete = wrapper;

  if (buffer instanceof Buffer) {
    // if no position is passed then assume null
    if (typeof position === 'function') {
      callback = position;
      position = null;
    }
    callback = maybeCallback(callback);
    return binding.writeBuffer(fd, buffer, offset, length, position, req);
  }

  if (typeof buffer !== 'string')
    buffer += '';
  if (typeof position !== 'function') {
    if (typeof offset === 'function') {
      position = offset;
      offset = null;
    } else {
      position = length;
    }
    length = 'utf8';
  }
  callback = maybeCallback(position);
  return binding.writeString(fd, buffer, offset, length, req);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeFile (path, data, options, callback_)](#apidoc.element.fs.extra.writeFile)
- description and source-code
```javascript
writeFile = function (path, data, options, callback_) {
  var callback = maybeCallback(arguments[arguments.length - 1]);

  if (!options || typeof options === 'function') {
    options = { encoding: 'utf8', mode: 0o666, flag: 'w' };
  } else if (typeof options === 'string') {
    options = { encoding: options, mode: 0o666, flag: 'w' };
  } else if (typeof options !== 'object') {
    throwOptionsError(options);
  }

  assertEncoding(options.encoding);

  var flag = options.flag || 'w';

  if (isFd(path)) {
    writeFd(path, true);
    return;
  }

  fs.open(path, flag, options.mode, function(openErr, fd) {
    if (openErr) {
      callback(openErr);
    } else {
      writeFd(fd, false);
    }
  });

  function writeFd(fd, isUserFd) {
    var buffer = (data instanceof Buffer) ?
        data : Buffer.from('' + data, options.encoding || 'utf8');
    var position = /a/.test(flag) ? null : 0;

    writeAll(fd, isUserFd, buffer, 0, buffer.length, position, callback);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeFileSync (path, data, options)](#apidoc.element.fs.extra.writeFileSync)
- description and source-code
```javascript
writeFileSync = function (path, data, options) {
  if (!options) {
    options = { encoding: 'utf8', mode: 0o666, flag: 'w' };
  } else if (typeof options === 'string') {
    options = { encoding: options, mode: 0o666, flag: 'w' };
  } else if (typeof options !== 'object') {
    throwOptionsError(options);
  }

  assertEncoding(options.encoding);

  var flag = options.flag || 'w';
  var isUserFd = isFd(path); // file descriptor ownership
  var fd = isUserFd ? path : fs.openSync(path, flag, options.mode);

  if (!(data instanceof Buffer)) {
    data = Buffer.from('' + data, options.encoding || 'utf8');
  }
  var offset = 0;
  var length = data.length;
  var position = /a/.test(flag) ? null : 0;
  try {
    while (length > 0) {
      var written = fs.writeSync(fd, data, offset, length, position);
      offset += written;
      length -= written;
      if (position !== null) {
        position += written;
      }
    }
  } finally {
    if (!isUserFd) fs.closeSync(fd);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeJSON"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeJSON (file, obj, callback)](#apidoc.element.fs.extra.writeJSON)
- description and source-code
```javascript
writeJSON = function (file, obj, callback) {
  var str = '';
  try {
    str = JSON.stringify(obj, null, module.exports.spaces);
  } catch (err) {
    callback(err, null);
  }
  fs.writeFile(file, str, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeJSONFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeJSONFile (file, obj, callback)](#apidoc.element.fs.extra.writeJSONFile)
- description and source-code
```javascript
writeJSONFile = function (file, obj, callback) {
  var str = '';
  try {
    str = JSON.stringify(obj, null, module.exports.spaces);
  } catch (err) {
    callback(err, null);
  }
  fs.writeFile(file, str, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeJSONFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeJSONFileSync (file, obj)](#apidoc.element.fs.extra.writeJSONFileSync)
- description and source-code
```javascript
writeJSONFileSync = function (file, obj) {
  var str = JSON.stringify(obj, null, module.exports.spaces);
  return fs.writeFileSync(file, str); //not sure if fs.writeFileSync returns anything, but just in case
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeJSONSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeJSONSync (file, obj)](#apidoc.element.fs.extra.writeJSONSync)
- description and source-code
```javascript
writeJSONSync = function (file, obj) {
  var str = JSON.stringify(obj, null, module.exports.spaces);
  return fs.writeFileSync(file, str); //not sure if fs.writeFileSync returns anything, but just in case
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeJson"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeJson (file, obj, callback)](#apidoc.element.fs.extra.writeJson)
- description and source-code
```javascript
writeJson = function (file, obj, callback) {
  var str = '';
  try {
    str = JSON.stringify(obj, null, module.exports.spaces);
  } catch (err) {
    callback(err, null);
  }
  fs.writeFile(file, str, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeJsonFile"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeJsonFile (file, obj, callback)](#apidoc.element.fs.extra.writeJsonFile)
- description and source-code
```javascript
writeJsonFile = function (file, obj, callback) {
  var str = '';
  try {
    str = JSON.stringify(obj, null, module.exports.spaces);
  } catch (err) {
    callback(err, null);
  }
  fs.writeFile(file, str, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeJsonFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeJsonFileSync (file, obj)](#apidoc.element.fs.extra.writeJsonFileSync)
- description and source-code
```javascript
writeJsonFileSync = function (file, obj) {
  var str = JSON.stringify(obj, null, module.exports.spaces);
  return fs.writeFileSync(file, str); //not sure if fs.writeFileSync returns anything, but just in case
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeJsonSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeJsonSync (file, obj)](#apidoc.element.fs.extra.writeJsonSync)
- description and source-code
```javascript
writeJsonSync = function (file, obj) {
  var str = JSON.stringify(obj, null, module.exports.spaces);
  return fs.writeFileSync(file, str); //not sure if fs.writeFileSync returns anything, but just in case
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.writeSync"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>writeSync (fd, buffer, offset, length, position)](#apidoc.element.fs.extra.writeSync)
- description and source-code
```javascript
writeSync = function (fd, buffer, offset, length, position) {
  if (buffer instanceof Buffer) {
    if (position === undefined)
      position = null;
    return binding.writeBuffer(fd, buffer, offset, length, position);
  }
  if (typeof buffer !== 'string')
    buffer += '';
  if (offset === undefined)
    offset = null;
  return binding.writeString(fd, buffer, offset, length, position);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs.extra.ReadStream"></a>[module fs.extra.ReadStream](#apidoc.module.fs.extra.ReadStream)

#### <a name="apidoc.element.fs.extra.ReadStream.ReadStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>ReadStream (path, options)](#apidoc.element.fs.extra.ReadStream.ReadStream)
- description and source-code
```javascript
function ReadStream(path, options) {
  if (!(this instanceof ReadStream))
    return new ReadStream(path, options);

  if (options === undefined)
    options = {};
  else if (typeof options === 'string')
    options = { encoding: options };
  else if (options === null || typeof options !== 'object')
    throw new TypeError('"options" argument must be a string or an object');

  // a little bit bigger buffer and water marks by default
  options = Object.create(options);
  if (options.highWaterMark === undefined)
    options.highWaterMark = 64 * 1024;

  Readable.call(this, options);

  this.path = path;
  this.fd = options.fd === undefined ? null : options.fd;
  this.flags = options.flags === undefined ? 'r' : options.flags;
  this.mode = options.mode === undefined ? 0o666 : options.mode;

  this.start = options.start;
  this.end = options.end;
  this.autoClose = options.autoClose === undefined ? true : options.autoClose;
  this.pos = undefined;
  this.bytesRead = 0;

  if (this.start !== undefined) {
    if (typeof this.start !== 'number') {
      throw new TypeError('"start" option must be a Number');
    }
    if (this.end === undefined) {
      this.end = Infinity;
    } else if (typeof this.end !== 'number') {
      throw new TypeError('"end" option must be a Number');
    }

    if (this.start > this.end) {
      throw new Error('"start" option must be <= "end" option');
    }

    this.pos = this.start;
  }

  if (typeof this.fd !== 'number')
    this.open();

  this.on('end', function() {
    if (this.autoClose) {
      this.destroy();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.ReadStream.super_"></a>[function <span class="apidocSignatureSpan">fs.extra.ReadStream.</span>super_ (options)](#apidoc.element.fs.extra.ReadStream.super_)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function')
    this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs.extra.ReadStream.prototype"></a>[module fs.extra.ReadStream.prototype](#apidoc.module.fs.extra.ReadStream.prototype)

#### <a name="apidoc.element.fs.extra.ReadStream.prototype._read"></a>[function <span class="apidocSignatureSpan">fs.extra.ReadStream.prototype.</span>_read (n)](#apidoc.element.fs.extra.ReadStream.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  if (typeof this.fd !== 'number')
    return this.once('open', function() {
      this._read(n);
    });

  if (this.destroyed)
    return;

  if (!pool || pool.length - pool.used < kMinPoolSpace) {
    // discard the old pool.
    allocNewPool(this._readableState.highWaterMark);
  }

  // Grab another reference to the pool in the case that while we're
  // in the thread pool another read() finishes up the pool, and
  // allocates a new one.
  var thisPool = pool;
  var toRead = Math.min(pool.length - pool.used, n);
  var start = pool.used;

  if (this.pos !== undefined)
    toRead = Math.min(this.end - this.pos + 1, toRead);

  // already read everything we were supposed to read!
  // treat as EOF.
  if (toRead <= 0)
    return this.push(null);

  // the actual read.
  var self = this;
  fs.read(this.fd, pool, pool.used, toRead, this.pos, onread);

  // move the pool positions, and internal position for reading.
  if (this.pos !== undefined)
    this.pos += toRead;
  pool.used += toRead;

  function onread(er, bytesRead) {
    if (er) {
      if (self.autoClose) {
        self.destroy();
      }
      self.emit('error', er);
    } else {
      var b = null;
      if (bytesRead > 0) {
        self.bytesRead += bytesRead;
        b = thisPool.slice(start, start + bytesRead);
      }

      self.push(b);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.ReadStream.prototype.close"></a>[function <span class="apidocSignatureSpan">fs.extra.ReadStream.prototype.</span>close (cb)](#apidoc.element.fs.extra.ReadStream.prototype.close)
- description and source-code
```javascript
close = function (cb) {
  var self = this;
  if (cb)
    this.once('close', cb);
  if (this.closed || typeof this.fd !== 'number') {
    if (typeof this.fd !== 'number') {
      this.once('open', close);
      return;
    }
    return process.nextTick(() => this.emit('close'));
  }
  this.closed = true;
  close();

  function close(fd) {
    fs.close(fd || self.fd, function(er) {
      if (er)
        self.emit('error', er);
      else
        self.emit('close');
    });
    self.fd = null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.ReadStream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">fs.extra.ReadStream.prototype.</span>destroy ()](#apidoc.element.fs.extra.ReadStream.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  if (this.destroyed)
    return;
  this.destroyed = true;
  this.close();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.ReadStream.prototype.open"></a>[function <span class="apidocSignatureSpan">fs.extra.ReadStream.prototype.</span>open ()](#apidoc.element.fs.extra.ReadStream.prototype.open)
- description and source-code
```javascript
open = function () {
  var self = this;
  fs.open(this.path, this.flags, this.mode, function(er, fd) {
    if (er) {
      if (self.autoClose) {
        self.destroy();
      }
      self.emit('error', er);
      return;
    }

    self.fd = fd;
    self.emit('open', fd);
    // start the flow of data.
    self.read();
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs.extra.Stats"></a>[module fs.extra.Stats](#apidoc.module.fs.extra.Stats)

#### <a name="apidoc.element.fs.extra.Stats.Stats"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.fs.extra.Stats.Stats)
- description and source-code
```javascript
function Stats( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec) {
  this.dev = dev;
  this.mode = mode;
  this.nlink = nlink;
  this.uid = uid;
  this.gid = gid;
  this.rdev = rdev;
  this.blksize = blksize;
  this.ino = ino;
  this.size = size;
  this.blocks = blocks;
  this.atime = new Date(atim_msec);
  this.mtime = new Date(mtim_msec);
  this.ctime = new Date(ctim_msec);
  this.birthtime = new Date(birthtim_msec);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs.extra.Stats.prototype"></a>[module fs.extra.Stats.prototype](#apidoc.module.fs.extra.Stats.prototype)

#### <a name="apidoc.element.fs.extra.Stats.prototype._checkModeProperty"></a>[function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>_checkModeProperty (property)](#apidoc.element.fs.extra.Stats.prototype._checkModeProperty)
- description and source-code
```javascript
_checkModeProperty = function (property) {
  return ((this.mode & constants.S_IFMT) === property);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.Stats.prototype.isBlockDevice"></a>[function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isBlockDevice ()](#apidoc.element.fs.extra.Stats.prototype.isBlockDevice)
- description and source-code
```javascript
isBlockDevice = function () {
  return this._checkModeProperty(constants.S_IFBLK);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.Stats.prototype.isCharacterDevice"></a>[function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isCharacterDevice ()](#apidoc.element.fs.extra.Stats.prototype.isCharacterDevice)
- description and source-code
```javascript
isCharacterDevice = function () {
  return this._checkModeProperty(constants.S_IFCHR);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.Stats.prototype.isDirectory"></a>[function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isDirectory ()](#apidoc.element.fs.extra.Stats.prototype.isDirectory)
- description and source-code
```javascript
isDirectory = function () {
  return this._checkModeProperty(constants.S_IFDIR);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.Stats.prototype.isFIFO"></a>[function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isFIFO ()](#apidoc.element.fs.extra.Stats.prototype.isFIFO)
- description and source-code
```javascript
isFIFO = function () {
  return this._checkModeProperty(constants.S_IFIFO);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.Stats.prototype.isFile"></a>[function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isFile ()](#apidoc.element.fs.extra.Stats.prototype.isFile)
- description and source-code
```javascript
isFile = function () {
  return this._checkModeProperty(constants.S_IFREG);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.Stats.prototype.isSocket"></a>[function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isSocket ()](#apidoc.element.fs.extra.Stats.prototype.isSocket)
- description and source-code
```javascript
isSocket = function () {
  return this._checkModeProperty(constants.S_IFSOCK);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.Stats.prototype.isSymbolicLink"></a>[function <span class="apidocSignatureSpan">fs.extra.Stats.prototype.</span>isSymbolicLink ()](#apidoc.element.fs.extra.Stats.prototype.isSymbolicLink)
- description and source-code
```javascript
isSymbolicLink = function () {
  return this._checkModeProperty(constants.S_IFLNK);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs.extra.WriteStream"></a>[module fs.extra.WriteStream](#apidoc.module.fs.extra.WriteStream)

#### <a name="apidoc.element.fs.extra.WriteStream.WriteStream"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>WriteStream (path, options)](#apidoc.element.fs.extra.WriteStream.WriteStream)
- description and source-code
```javascript
function WriteStream(path, options) {
  if (!(this instanceof WriteStream))
    return new WriteStream(path, options);

  if (options === undefined)
    options = {};
  else if (typeof options === 'string')
    options = { encoding: options };
  else if (options === null || typeof options !== 'object')
    throw new TypeError('"options" argument must be a string or an object');

  options = Object.create(options);

  Writable.call(this, options);

  this.path = path;
  this.fd = options.fd === undefined ? null : options.fd;
  this.flags = options.flags === undefined ? 'w' : options.flags;
  this.mode = options.mode === undefined ? 0o666 : options.mode;

  this.start = options.start;
  this.autoClose = options.autoClose === undefined ? true : !!options.autoClose;
  this.pos = undefined;
  this.bytesWritten = 0;

  if (this.start !== undefined) {
    if (typeof this.start !== 'number') {
      throw new TypeError('"start" option must be a Number');
    }
    if (this.start < 0) {
      throw new Error('"start" must be >= zero');
    }

    this.pos = this.start;
  }

  if (options.encoding)
    this.setDefaultEncoding(options.encoding);

  if (typeof this.fd !== 'number')
    this.open();

  // dispose on finish.
  this.once('finish', function() {
    if (this.autoClose) {
      this.close();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.WriteStream.super_"></a>[function <span class="apidocSignatureSpan">fs.extra.WriteStream.</span>super_ (options)](#apidoc.element.fs.extra.WriteStream.super_)
- description and source-code
```javascript
function Writable(options) {
  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!(realHasInstance.call(Writable, this)) &&
      !(this instanceof Stream.Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function')
      this._write = options.write;

    if (typeof options.writev === 'function')
      this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs.extra.WriteStream.prototype"></a>[module fs.extra.WriteStream.prototype](#apidoc.module.fs.extra.WriteStream.prototype)

#### <a name="apidoc.element.fs.extra.WriteStream.prototype._write"></a>[function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>_write (data, encoding, cb)](#apidoc.element.fs.extra.WriteStream.prototype._write)
- description and source-code
```javascript
_write = function (data, encoding, cb) {
  if (!(data instanceof Buffer))
    return this.emit('error', new Error('Invalid data'));

  if (typeof this.fd !== 'number')
    return this.once('open', function() {
      this._write(data, encoding, cb);
    });

  var self = this;
  fs.write(this.fd, data, 0, data.length, this.pos, function(er, bytes) {
    if (er) {
      if (self.autoClose) {
        self.destroy();
      }
      return cb(er);
    }
    self.bytesWritten += bytes;
    cb();
  });

  if (this.pos !== undefined)
    this.pos += data.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.WriteStream.prototype._writev"></a>[function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>_writev (data, cb)](#apidoc.element.fs.extra.WriteStream.prototype._writev)
- description and source-code
```javascript
_writev = function (data, cb) {
  if (typeof this.fd !== 'number')
    return this.once('open', function() {
      this._writev(data, cb);
    });

  const self = this;
  const len = data.length;
  const chunks = new Array(len);
  var size = 0;

  for (var i = 0; i < len; i++) {
    var chunk = data[i].chunk;

    chunks[i] = chunk;
    size += chunk.length;
  }

  writev(this.fd, chunks, this.pos, function(er, bytes) {
    if (er) {
      self.destroy();
      return cb(er);
    }
    self.bytesWritten += bytes;
    cb();
  });

  if (this.pos !== undefined)
    this.pos += size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.WriteStream.prototype.close"></a>[function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>close (cb)](#apidoc.element.fs.extra.WriteStream.prototype.close)
- description and source-code
```javascript
close = function (cb) {
  var self = this;
  if (cb)
    this.once('close', cb);
  if (this.closed || typeof this.fd !== 'number') {
    if (typeof this.fd !== 'number') {
      this.once('open', close);
      return;
    }
    return process.nextTick(() => this.emit('close'));
  }
  this.closed = true;
  close();

  function close(fd) {
    fs.close(fd || self.fd, function(er) {
      if (er)
        self.emit('error', er);
      else
        self.emit('close');
    });
    self.fd = null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.WriteStream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>destroy ()](#apidoc.element.fs.extra.WriteStream.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  if (this.destroyed)
    return;
  this.destroyed = true;
  this.close();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.WriteStream.prototype.destroySoon"></a>[function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>destroySoon (chunk, encoding, cb)](#apidoc.element.fs.extra.WriteStream.prototype.destroySoon)
- description and source-code
```javascript
destroySoon = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (chunk !== null && chunk !== undefined)
    this.write(chunk, encoding);

  // .end() fully uncorks
  if (state.corked) {
    state.corked = 1;
    this.uncork();
  }

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished)
    endWritable(this, state, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.WriteStream.prototype.open"></a>[function <span class="apidocSignatureSpan">fs.extra.WriteStream.prototype.</span>open ()](#apidoc.element.fs.extra.WriteStream.prototype.open)
- description and source-code
```javascript
open = function () {
  fs.open(this.path, this.flags, this.mode, function(er, fd) {
    if (er) {
      if (this.autoClose) {
        this.destroy();
      }
      this.emit('error', er);
      return;
    }

    this.fd = fd;
    this.emit('open', fd);
  }.bind(this));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs.extra.jsonfile"></a>[module fs.extra.jsonfile](#apidoc.module.fs.extra.jsonfile)

#### <a name="apidoc.element.fs.extra.jsonfile.readFile"></a>[function <span class="apidocSignatureSpan">fs.extra.jsonfile.</span>readFile (file, callback)](#apidoc.element.fs.extra.jsonfile.readFile)
- description and source-code
```javascript
readFile = function (file, callback) {
  fs.readFile(file, 'utf8', function(err, data) {
    if (err) return callback(err, null);

    try {
      var obj = JSON.parse(data);
      callback(null, obj);
    } catch (err2) {
      callback(err2, null);
    }
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.jsonfile.readFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.jsonfile.</span>readFileSync (file)](#apidoc.element.fs.extra.jsonfile.readFileSync)
- description and source-code
```javascript
readFileSync = function (file) {
  return JSON.parse(fs.readFileSync(file, 'utf8'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.jsonfile.writeFile"></a>[function <span class="apidocSignatureSpan">fs.extra.jsonfile.</span>writeFile (file, obj, callback)](#apidoc.element.fs.extra.jsonfile.writeFile)
- description and source-code
```javascript
writeFile = function (file, obj, callback) {
  var str = '';
  try {
    str = JSON.stringify(obj, null, module.exports.spaces);
  } catch (err) {
    callback(err, null);
  }
  fs.writeFile(file, str, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.jsonfile.writeFileSync"></a>[function <span class="apidocSignatureSpan">fs.extra.jsonfile.</span>writeFileSync (file, obj)](#apidoc.element.fs.extra.jsonfile.writeFileSync)
- description and source-code
```javascript
writeFileSync = function (file, obj) {
  var str = JSON.stringify(obj, null, module.exports.spaces);
  return fs.writeFileSync(file, str); //not sure if fs.writeFileSync returns anything, but just in case
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fs.extra.mkdirs"></a>[module fs.extra.mkdirs](#apidoc.module.fs.extra.mkdirs)

#### <a name="apidoc.element.fs.extra.mkdirs.mkdirs"></a>[function <span class="apidocSignatureSpan">fs.extra.</span>mkdirs (p, mode, f, made)](#apidoc.element.fs.extra.mkdirs.mkdirs)
- description and source-code
```javascript
function mkdirP(p, mode, f, made) {
    if (typeof mode === 'function' || mode === undefined) {
        f = mode;
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    var cb = f || function () {};
    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    fs.mkdir(p, mode, function (er) {
        if (!er) {
            made = made || p;
            return cb(null, made);
        }
        switch (er.code) {
            case 'ENOENT':
                mkdirP(path.dirname(p), mode, function (er, made) {
                    if (er) cb(er, made);
                    else mkdirP(p, mode, cb, made);
                });
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                fs.stat(p, function (er2, stat) {
                    // if the stat fails, then that's super weird.
                    // let the original error be the failure reason.
                    if (er2 || !stat.isDirectory()) cb(er, made)
                    else cb(null, made);
                });
                break;
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdirs.mkdirP"></a>[function <span class="apidocSignatureSpan">fs.extra.mkdirs.</span>mkdirP (p, mode, f, made)](#apidoc.element.fs.extra.mkdirs.mkdirP)
- description and source-code
```javascript
function mkdirP(p, mode, f, made) {
    if (typeof mode === 'function' || mode === undefined) {
        f = mode;
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    var cb = f || function () {};
    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    fs.mkdir(p, mode, function (er) {
        if (!er) {
            made = made || p;
            return cb(null, made);
        }
        switch (er.code) {
            case 'ENOENT':
                mkdirP(path.dirname(p), mode, function (er, made) {
                    if (er) cb(er, made);
                    else mkdirP(p, mode, cb, made);
                });
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                fs.stat(p, function (er2, stat) {
                    // if the stat fails, then that's super weird.
                    // let the original error be the failure reason.
                    if (er2 || !stat.isDirectory()) cb(er, made)
                    else cb(null, made);
                });
                break;
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fs.extra.mkdirs.mkdirp"></a>[function <span class="apidocSignatureSpan">fs.extra.mkdirs.</span>mkdirp (p, mode, f, made)](#apidoc.element.fs.extra.mkdirs.mkdirp)
- description and source-code
```javascript
function mkdirP(p, mode, f, made) {
    if (typeof mode === 'function' || mode === undefined) {
        f = mode;
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    var cb = f || function () {};
    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    fs.mkdir(p, mode, function (er) {
        if (!er) {
            made = made || p;
            return cb(null, made);
        }
        switch (er.code) {
            case 'ENOENT':
                mkdirP(path.dirname(p), mode, function (er, made) {
                    if (er) cb(er, made);
                    else mkdirP(p, mode, cb, made);
                });
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                fs.stat(p, function (er2, stat) {
                    // if the stat fails, then that's super weird.
                    // let the original error be the failure reason.
                    if (er2 || !stat.isDirectory()) cb(er, made)
                    else cb(null, made);
                });
                break;
        }
    });
}
```
- example usage
```shell
...

fs.mkdirRecursive
===

Included from <https://github.com/substack/node-mkdirp>

'''javascript
// fs.mkdirp(path, mode=(0777 & (~process.umask())), cb);

fs.mkdirp('/tmp/foo/bar/baz', function (err) {
if (err) {
  console.error(err);
} else {
  console.log('pow!')
}
...
```

#### <a name="apidoc.element.fs.extra.mkdirs.sync"></a>[function <span class="apidocSignatureSpan">fs.extra.mkdirs.</span>sync (p, mode, made)](#apidoc.element.fs.extra.mkdirs.sync)
- description and source-code
```javascript
function sync(p, mode, made) {
    if (mode === undefined) {
        mode = 0777 & (~process.umask());
    }
    if (!made) made = null;

    if (typeof mode === 'string') mode = parseInt(mode, 8);
    p = path.resolve(p);

    try {
        fs.mkdirSync(p, mode);
        made = made || p;
    }
    catch (err0) {
        switch (err0.code) {
            case 'ENOENT' :
                made = sync(path.dirname(p), mode, made);
                sync(p, mode, made);
                break;

            // In the case of any other error, just see if there's a dir
            // there already.  If so, then hooray!  If not, then something
            // is borked.
            default:
                var stat;
                try {
                    stat = fs.statSync(p);
                }
                catch (err1) {
                    throw err0;
                }
                if (!stat.isDirectory()) throw err0;
                break;
        }
    }

    return made;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
