# api documentation for  [mz (v2.6.0)](https://github.com/normalize/mz#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-mz.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mz) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mz.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mz)
#### modernize node.js to current ECMAScript standards

[![NPM](https://nodei.co/npm/mz.png?downloads=true)](https://www.npmjs.com/package/mz)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mz/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mz_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mz/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mz/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mz/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jonathan Ong",
        "email": "me@jongleberry.com",
        "url": "http://jongleberry.com"
    },
    "bugs": {
        "url": "https://github.com/normalize/mz/issues"
    },
    "dependencies": {
        "any-promise": "^1.0.0",
        "object-assign": "^4.0.1",
        "thenify-all": "^1.0.0"
    },
    "description": "modernize node.js to current ECMAScript standards",
    "devDependencies": {
        "bluebird": "^3.0.0",
        "istanbul": "^0.4.0",
        "mocha": "^3.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "c8b8521d958df0a4f2768025db69c719ee4ef1ce",
        "tarball": "https://registry.npmjs.org/mz/-/mz-2.6.0.tgz"
    },
    "files": [
        "index.js",
        "child_process.js",
        "crypto.js",
        "dns.js",
        "fs.js",
        "readline.js",
        "zlib.js"
    ],
    "gitHead": "10bc91f7f0bb861cc940a078037be64cc166c144",
    "homepage": "https://github.com/normalize/mz#readme",
    "keywords": [
        "promisify",
        "promise",
        "thenify",
        "then",
        "es6"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "coderhaoxin",
            "email": "coderhaoxin@outlook.com"
        },
        {
            "name": "dead-horse",
            "email": "dead_horse@qq.com"
        },
        {
            "name": "dead_horse",
            "email": "dead_horse@qq.com"
        },
        {
            "name": "evancarroll",
            "email": "me@evancarroll.com"
        },
        {
            "name": "jongleberry",
            "email": "jonathanrichardong@gmail.com"
        },
        {
            "name": "linusu",
            "email": "linus@folkdatorn.se"
        },
        {
            "name": "rstacruz",
            "email": "dropbox@ricostacruz.com"
        },
        {
            "name": "swatinem",
            "email": "arpad.borsos@googlemail.com"
        }
    ],
    "name": "mz",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/normalize/mz.git"
    },
    "scripts": {
        "test": "mocha --reporter spec",
        "test-cov": "istanbul cover node_modules/mocha/bin/_mocha -- --reporter dot",
        "test-travis": "istanbul cover node_modules/mocha/bin/_mocha --report lcovonly -- --reporter dot"
    },
    "version": "2.6.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mz](#apidoc.module.mz)
1.  [function <span class="apidocSignatureSpan">mz.</span>child_process.ChildProcess ()](#apidoc.element.mz.child_process.ChildProcess)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.Certificate ()](#apidoc.element.mz.crypto.Certificate)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.Cipher (cipher, password, options)](#apidoc.element.mz.crypto.Cipher)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.Cipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Cipheriv)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.Decipher (cipher, password, options)](#apidoc.element.mz.crypto.Decipher)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.Decipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Decipheriv)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.DiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.mz.crypto.DiffieHellman)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.Hash (algorithm, options)](#apidoc.element.mz.crypto.Hash)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.Hmac (hmac, key, options)](#apidoc.element.mz.crypto.Hmac)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.Sign (algorithm, options)](#apidoc.element.mz.crypto.Sign)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.Verify (algorithm, options)](#apidoc.element.mz.crypto.Verify)
1.  [function <span class="apidocSignatureSpan">mz.</span>crypto.getDiffieHellman (name)](#apidoc.element.mz.crypto.getDiffieHellman)
1.  [function <span class="apidocSignatureSpan">mz.</span>fs.ReadStream (path, options)](#apidoc.element.mz.fs.ReadStream)
1.  [function <span class="apidocSignatureSpan">mz.</span>fs.Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.mz.fs.Stats)
1.  [function <span class="apidocSignatureSpan">mz.</span>fs.WriteStream (path, options)](#apidoc.element.mz.fs.WriteStream)
1.  [function <span class="apidocSignatureSpan">mz.</span>readline.Interface (input, output, completer, terminal)](#apidoc.element.mz.readline.Interface)
1.  [function <span class="apidocSignatureSpan">mz.</span>zlib.Deflate (opts)](#apidoc.element.mz.zlib.Deflate)
1.  [function <span class="apidocSignatureSpan">mz.</span>zlib.DeflateRaw (opts)](#apidoc.element.mz.zlib.DeflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.</span>zlib.Gunzip (opts)](#apidoc.element.mz.zlib.Gunzip)
1.  [function <span class="apidocSignatureSpan">mz.</span>zlib.Gzip (opts)](#apidoc.element.mz.zlib.Gzip)
1.  [function <span class="apidocSignatureSpan">mz.</span>zlib.Inflate (opts)](#apidoc.element.mz.zlib.Inflate)
1.  [function <span class="apidocSignatureSpan">mz.</span>zlib.InflateRaw (opts)](#apidoc.element.mz.zlib.InflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.</span>zlib.Unzip (opts)](#apidoc.element.mz.zlib.Unzip)
1.  [function <span class="apidocSignatureSpan">mz.</span>zlib.Zlib ()](#apidoc.element.mz.zlib.Zlib)
1.  object <span class="apidocSignatureSpan">mz.</span>child_process
1.  object <span class="apidocSignatureSpan">mz.</span>child_process.ChildProcess.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.Certificate.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.Cipher.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.Cipheriv.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.Decipher.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.Decipheriv.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.DiffieHellman.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.Hash.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.Hmac.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.Sign.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.Verify.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>crypto.getDiffieHellman.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>dns
1.  object <span class="apidocSignatureSpan">mz.</span>fs
1.  object <span class="apidocSignatureSpan">mz.</span>fs.ReadStream.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>fs.Stats.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>fs.WriteStream.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>readline
1.  object <span class="apidocSignatureSpan">mz.</span>readline.Interface.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>zlib
1.  object <span class="apidocSignatureSpan">mz.</span>zlib.Deflate.super_.prototype
1.  object <span class="apidocSignatureSpan">mz.</span>zlib.Zlib.prototype

#### [module mz.child_process](#apidoc.module.mz.child_process)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>ChildProcess ()](#apidoc.element.mz.child_process.ChildProcess)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>_forkChild (fd)](#apidoc.element.mz.child_process._forkChild)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>exec ()](#apidoc.element.mz.child_process.exec)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>execFile ()](#apidoc.element.mz.child_process.execFile)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>execFileSync ()](#apidoc.element.mz.child_process.execFileSync)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>execSync (command)](#apidoc.element.mz.child_process.execSync)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>fork (modulePath)](#apidoc.element.mz.child_process.fork)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>spawn ()](#apidoc.element.mz.child_process.spawn)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>spawnSync ()](#apidoc.element.mz.child_process.spawnSync)

#### [module mz.child_process.ChildProcess](#apidoc.module.mz.child_process.ChildProcess)
1.  [function <span class="apidocSignatureSpan">mz.child_process.</span>ChildProcess ()](#apidoc.element.mz.child_process.ChildProcess.ChildProcess)
1.  [function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.</span>super_ ()](#apidoc.element.mz.child_process.ChildProcess.super_)

#### [module mz.child_process.ChildProcess.prototype](#apidoc.module.mz.child_process.ChildProcess.prototype)
1.  [function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.prototype.</span>kill (sig)](#apidoc.element.mz.child_process.ChildProcess.prototype.kill)
1.  [function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.prototype.</span>ref ()](#apidoc.element.mz.child_process.ChildProcess.prototype.ref)
1.  [function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.prototype.</span>spawn (options)](#apidoc.element.mz.child_process.ChildProcess.prototype.spawn)
1.  [function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.prototype.</span>unref ()](#apidoc.element.mz.child_process.ChildProcess.prototype.unref)

#### [module mz.crypto](#apidoc.module.mz.crypto)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Certificate ()](#apidoc.element.mz.crypto.Certificate)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Cipher (cipher, password, options)](#apidoc.element.mz.crypto.Cipher)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Cipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Cipheriv)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Decipher (cipher, password, options)](#apidoc.element.mz.crypto.Decipher)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Decipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Decipheriv)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>DiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.mz.crypto.DiffieHellman)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>DiffieHellmanGroup (name)](#apidoc.element.mz.crypto.DiffieHellmanGroup)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Hash (algorithm, options)](#apidoc.element.mz.crypto.Hash)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Hmac (hmac, key, options)](#apidoc.element.mz.crypto.Hmac)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Sign (algorithm, options)](#apidoc.element.mz.crypto.Sign)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Verify (algorithm, options)](#apidoc.element.mz.crypto.Verify)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>_toBuf (str, encoding)](#apidoc.element.mz.crypto._toBuf)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createCipher (cipher, password, options)](#apidoc.element.mz.crypto.createCipher)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createCipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.createCipheriv)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createDecipher (cipher, password, options)](#apidoc.element.mz.crypto.createDecipher)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createDecipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.createDecipheriv)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createDiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.mz.crypto.createDiffieHellman)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createDiffieHellmanGroup (name)](#apidoc.element.mz.crypto.createDiffieHellmanGroup)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createECDH (curve)](#apidoc.element.mz.crypto.createECDH)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createHash (algorithm, options)](#apidoc.element.mz.crypto.createHash)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createHmac (hmac, key, options)](#apidoc.element.mz.crypto.createHmac)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createSign (algorithm, options)](#apidoc.element.mz.crypto.createSign)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>createVerify (algorithm, options)](#apidoc.element.mz.crypto.createVerify)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>getCiphers ()](#apidoc.element.mz.crypto.getCiphers)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>getCurves ()](#apidoc.element.mz.crypto.getCurves)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>getDiffieHellman (name)](#apidoc.element.mz.crypto.getDiffieHellman)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>getHashes ()](#apidoc.element.mz.crypto.getHashes)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>pbkdf2 ()](#apidoc.element.mz.crypto.pbkdf2)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>pbkdf2Sync (password, salt, iterations, keylen, digest)](#apidoc.element.mz.crypto.pbkdf2Sync)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>privateDecrypt (options, buffer)](#apidoc.element.mz.crypto.privateDecrypt)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>privateEncrypt (options, buffer)](#apidoc.element.mz.crypto.privateEncrypt)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>prng ()](#apidoc.element.mz.crypto.prng)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>pseudoRandomBytes ()](#apidoc.element.mz.crypto.pseudoRandomBytes)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>publicDecrypt (options, buffer)](#apidoc.element.mz.crypto.publicDecrypt)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>publicEncrypt (options, buffer)](#apidoc.element.mz.crypto.publicEncrypt)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>randomBytes ()](#apidoc.element.mz.crypto.randomBytes)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>rng ()](#apidoc.element.mz.crypto.rng)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>setEngine (id, flags)](#apidoc.element.mz.crypto.setEngine)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>timingSafeEqual ()](#apidoc.element.mz.crypto.timingSafeEqual)
1.  object <span class="apidocSignatureSpan">mz.crypto.</span>constants
1.  string <span class="apidocSignatureSpan">mz.crypto.</span>DEFAULT_ENCODING

#### [module mz.crypto.Certificate](#apidoc.module.mz.crypto.Certificate)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Certificate ()](#apidoc.element.mz.crypto.Certificate.Certificate)

#### [module mz.crypto.Certificate.prototype](#apidoc.module.mz.crypto.Certificate.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Certificate.prototype.</span>exportChallenge (object, encoding)](#apidoc.element.mz.crypto.Certificate.prototype.exportChallenge)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Certificate.prototype.</span>exportPublicKey (object, encoding)](#apidoc.element.mz.crypto.Certificate.prototype.exportPublicKey)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Certificate.prototype.</span>verifySpkac (object)](#apidoc.element.mz.crypto.Certificate.prototype.verifySpkac)

#### [module mz.crypto.Cipher](#apidoc.module.mz.crypto.Cipher)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Cipher (cipher, password, options)](#apidoc.element.mz.crypto.Cipher.Cipher)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipher.</span>super_ (options)](#apidoc.element.mz.crypto.Cipher.super_)

#### [module mz.crypto.Cipher.prototype](#apidoc.module.mz.crypto.Cipher.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Cipher.prototype._flush)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Cipher.prototype._transform)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>final (outputEncoding)](#apidoc.element.mz.crypto.Cipher.prototype.final)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>getAuthTag ()](#apidoc.element.mz.crypto.Cipher.prototype.getAuthTag)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>setAAD (aadbuf)](#apidoc.element.mz.crypto.Cipher.prototype.setAAD)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.mz.crypto.Cipher.prototype.setAuthTag)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>setAutoPadding (ap)](#apidoc.element.mz.crypto.Cipher.prototype.setAutoPadding)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.mz.crypto.Cipher.prototype.update)

#### [module mz.crypto.Cipheriv](#apidoc.module.mz.crypto.Cipheriv)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Cipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Cipheriv.Cipheriv)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.</span>super_ (options)](#apidoc.element.mz.crypto.Cipheriv.super_)

#### [module mz.crypto.Cipheriv.prototype](#apidoc.module.mz.crypto.Cipheriv.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Cipheriv.prototype._flush)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Cipheriv.prototype._transform)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>final (outputEncoding)](#apidoc.element.mz.crypto.Cipheriv.prototype.final)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>getAuthTag ()](#apidoc.element.mz.crypto.Cipheriv.prototype.getAuthTag)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>setAAD (aadbuf)](#apidoc.element.mz.crypto.Cipheriv.prototype.setAAD)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.mz.crypto.Cipheriv.prototype.setAuthTag)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>setAutoPadding (ap)](#apidoc.element.mz.crypto.Cipheriv.prototype.setAutoPadding)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.mz.crypto.Cipheriv.prototype.update)

#### [module mz.crypto.Decipher](#apidoc.module.mz.crypto.Decipher)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Decipher (cipher, password, options)](#apidoc.element.mz.crypto.Decipher.Decipher)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.</span>super_ (options)](#apidoc.element.mz.crypto.Decipher.super_)

#### [module mz.crypto.Decipher.prototype](#apidoc.module.mz.crypto.Decipher.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Decipher.prototype._flush)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Decipher.prototype._transform)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>final (outputEncoding)](#apidoc.element.mz.crypto.Decipher.prototype.final)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>finaltol (outputEncoding)](#apidoc.element.mz.crypto.Decipher.prototype.finaltol)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>getAuthTag ()](#apidoc.element.mz.crypto.Decipher.prototype.getAuthTag)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>setAAD (aadbuf)](#apidoc.element.mz.crypto.Decipher.prototype.setAAD)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.mz.crypto.Decipher.prototype.setAuthTag)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>setAutoPadding (ap)](#apidoc.element.mz.crypto.Decipher.prototype.setAutoPadding)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.mz.crypto.Decipher.prototype.update)

#### [module mz.crypto.Decipheriv](#apidoc.module.mz.crypto.Decipheriv)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Decipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Decipheriv.Decipheriv)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.</span>super_ (options)](#apidoc.element.mz.crypto.Decipheriv.super_)

#### [module mz.crypto.Decipheriv.prototype](#apidoc.module.mz.crypto.Decipheriv.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Decipheriv.prototype._flush)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Decipheriv.prototype._transform)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>final (outputEncoding)](#apidoc.element.mz.crypto.Decipheriv.prototype.final)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>finaltol (outputEncoding)](#apidoc.element.mz.crypto.Decipheriv.prototype.finaltol)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>getAuthTag ()](#apidoc.element.mz.crypto.Decipheriv.prototype.getAuthTag)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>setAAD (aadbuf)](#apidoc.element.mz.crypto.Decipheriv.prototype.setAAD)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.mz.crypto.Decipheriv.prototype.setAuthTag)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>setAutoPadding (ap)](#apidoc.element.mz.crypto.Decipheriv.prototype.setAutoPadding)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.mz.crypto.Decipheriv.prototype.update)

#### [module mz.crypto.DiffieHellman](#apidoc.module.mz.crypto.DiffieHellman)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>DiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.mz.crypto.DiffieHellman.DiffieHellman)

#### [module mz.crypto.DiffieHellman.prototype](#apidoc.module.mz.crypto.DiffieHellman.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>computeSecret (key, inEnc, outEnc)](#apidoc.element.mz.crypto.DiffieHellman.prototype.computeSecret)
1.  [function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>generateKeys (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.generateKeys)
1.  [function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>getGenerator (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.getGenerator)
1.  [function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>getPrime (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.getPrime)
1.  [function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>getPrivateKey (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.getPrivateKey)
1.  [function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>getPublicKey (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.getPublicKey)
1.  [function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>setPrivateKey (key, encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.setPrivateKey)
1.  [function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>setPublicKey (key, encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.setPublicKey)

#### [module mz.crypto.Hash](#apidoc.module.mz.crypto.Hash)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Hash (algorithm, options)](#apidoc.element.mz.crypto.Hash.Hash)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hash.</span>super_ (options)](#apidoc.element.mz.crypto.Hash.super_)

#### [module mz.crypto.Hash.prototype](#apidoc.module.mz.crypto.Hash.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hash.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Hash.prototype._flush)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hash.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Hash.prototype._transform)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hash.prototype.</span>digest (outputEncoding)](#apidoc.element.mz.crypto.Hash.prototype.digest)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hash.prototype.</span>update (data, encoding)](#apidoc.element.mz.crypto.Hash.prototype.update)

#### [module mz.crypto.Hmac](#apidoc.module.mz.crypto.Hmac)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Hmac (hmac, key, options)](#apidoc.element.mz.crypto.Hmac.Hmac)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hmac.</span>super_ (options)](#apidoc.element.mz.crypto.Hmac.super_)

#### [module mz.crypto.Hmac.prototype](#apidoc.module.mz.crypto.Hmac.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hmac.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Hmac.prototype._flush)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hmac.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Hmac.prototype._transform)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hmac.prototype.</span>digest (outputEncoding)](#apidoc.element.mz.crypto.Hmac.prototype.digest)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Hmac.prototype.</span>update (data, encoding)](#apidoc.element.mz.crypto.Hmac.prototype.update)

#### [module mz.crypto.Sign](#apidoc.module.mz.crypto.Sign)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Sign (algorithm, options)](#apidoc.element.mz.crypto.Sign.Sign)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Sign.</span>super_ (options)](#apidoc.element.mz.crypto.Sign.super_)

#### [module mz.crypto.Sign.prototype](#apidoc.module.mz.crypto.Sign.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Sign.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.mz.crypto.Sign.prototype._write)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Sign.prototype.</span>sign (options, encoding)](#apidoc.element.mz.crypto.Sign.prototype.sign)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Sign.prototype.</span>update (data, encoding)](#apidoc.element.mz.crypto.Sign.prototype.update)

#### [module mz.crypto.Verify](#apidoc.module.mz.crypto.Verify)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>Verify (algorithm, options)](#apidoc.element.mz.crypto.Verify.Verify)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Verify.</span>super_ (options)](#apidoc.element.mz.crypto.Verify.super_)

#### [module mz.crypto.Verify.prototype](#apidoc.module.mz.crypto.Verify.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Verify.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.mz.crypto.Verify.prototype._write)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Verify.prototype.</span>update (data, encoding)](#apidoc.element.mz.crypto.Verify.prototype.update)
1.  [function <span class="apidocSignatureSpan">mz.crypto.Verify.prototype.</span>verify (object, signature, sigEncoding)](#apidoc.element.mz.crypto.Verify.prototype.verify)

#### [module mz.crypto.getDiffieHellman](#apidoc.module.mz.crypto.getDiffieHellman)
1.  [function <span class="apidocSignatureSpan">mz.crypto.</span>getDiffieHellman (name)](#apidoc.element.mz.crypto.getDiffieHellman.getDiffieHellman)

#### [module mz.crypto.getDiffieHellman.prototype](#apidoc.module.mz.crypto.getDiffieHellman.prototype)
1.  [function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>computeSecret (key, inEnc, outEnc)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.computeSecret)
1.  [function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>generateKeys (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.generateKeys)
1.  [function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>getGenerator (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.getGenerator)
1.  [function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>getPrime (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.getPrime)
1.  [function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>getPrivateKey (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.getPrivateKey)
1.  [function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>getPublicKey (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.getPublicKey)

#### [module mz.dns](#apidoc.module.mz.dns)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>getServers ()](#apidoc.element.mz.dns.getServers)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>lookup ()](#apidoc.element.mz.dns.lookup)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>lookupService (host, port, callback)](#apidoc.element.mz.dns.lookupService)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolve ()](#apidoc.element.mz.dns.resolve)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolve4 ()](#apidoc.element.mz.dns.resolve4)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolve6 ()](#apidoc.element.mz.dns.resolve6)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolveCname ()](#apidoc.element.mz.dns.resolveCname)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolveMx ()](#apidoc.element.mz.dns.resolveMx)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolveNaptr (name, callback)](#apidoc.element.mz.dns.resolveNaptr)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolveNs ()](#apidoc.element.mz.dns.resolveNs)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolvePtr (name, callback)](#apidoc.element.mz.dns.resolvePtr)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolveSoa (name, callback)](#apidoc.element.mz.dns.resolveSoa)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolveSrv ()](#apidoc.element.mz.dns.resolveSrv)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>resolveTxt ()](#apidoc.element.mz.dns.resolveTxt)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>reverse ()](#apidoc.element.mz.dns.reverse)
1.  [function <span class="apidocSignatureSpan">mz.dns.</span>setServers (servers)](#apidoc.element.mz.dns.setServers)
1.  number <span class="apidocSignatureSpan">mz.dns.</span>ADDRCONFIG
1.  number <span class="apidocSignatureSpan">mz.dns.</span>V4MAPPED
1.  string <span class="apidocSignatureSpan">mz.dns.</span>ADDRGETNETWORKPARAMS
1.  string <span class="apidocSignatureSpan">mz.dns.</span>BADFAMILY
1.  string <span class="apidocSignatureSpan">mz.dns.</span>BADFLAGS
1.  string <span class="apidocSignatureSpan">mz.dns.</span>BADHINTS
1.  string <span class="apidocSignatureSpan">mz.dns.</span>BADNAME
1.  string <span class="apidocSignatureSpan">mz.dns.</span>BADQUERY
1.  string <span class="apidocSignatureSpan">mz.dns.</span>BADRESP
1.  string <span class="apidocSignatureSpan">mz.dns.</span>BADSTR
1.  string <span class="apidocSignatureSpan">mz.dns.</span>CANCELLED
1.  string <span class="apidocSignatureSpan">mz.dns.</span>CONNREFUSED
1.  string <span class="apidocSignatureSpan">mz.dns.</span>DESTRUCTION
1.  string <span class="apidocSignatureSpan">mz.dns.</span>EOF
1.  string <span class="apidocSignatureSpan">mz.dns.</span>FILE
1.  string <span class="apidocSignatureSpan">mz.dns.</span>FORMERR
1.  string <span class="apidocSignatureSpan">mz.dns.</span>LOADIPHLPAPI
1.  string <span class="apidocSignatureSpan">mz.dns.</span>NODATA
1.  string <span class="apidocSignatureSpan">mz.dns.</span>NOMEM
1.  string <span class="apidocSignatureSpan">mz.dns.</span>NONAME
1.  string <span class="apidocSignatureSpan">mz.dns.</span>NOTFOUND
1.  string <span class="apidocSignatureSpan">mz.dns.</span>NOTIMP
1.  string <span class="apidocSignatureSpan">mz.dns.</span>NOTINITIALIZED
1.  string <span class="apidocSignatureSpan">mz.dns.</span>REFUSED
1.  string <span class="apidocSignatureSpan">mz.dns.</span>SERVFAIL
1.  string <span class="apidocSignatureSpan">mz.dns.</span>TIMEOUT

#### [module mz.fs](#apidoc.module.mz.fs)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>FileReadStream (path, options)](#apidoc.element.mz.fs.FileReadStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>FileWriteStream (path, options)](#apidoc.element.mz.fs.FileWriteStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>ReadStream (path, options)](#apidoc.element.mz.fs.ReadStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.mz.fs.Stats)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>WriteStream (path, options)](#apidoc.element.mz.fs.WriteStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>_toUnixTimestamp (time)](#apidoc.element.mz.fs._toUnixTimestamp)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>access ()](#apidoc.element.mz.fs.access)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>accessSync (path, mode)](#apidoc.element.mz.fs.accessSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>appendFile ()](#apidoc.element.mz.fs.appendFile)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>appendFileSync (path, data, options)](#apidoc.element.mz.fs.appendFileSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>chmod ()](#apidoc.element.mz.fs.chmod)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>chmodSync (path, mode)](#apidoc.element.mz.fs.chmodSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>chown ()](#apidoc.element.mz.fs.chown)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>chownSync (path, uid, gid)](#apidoc.element.mz.fs.chownSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>close ()](#apidoc.element.mz.fs.close)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>closeSync (fd)](#apidoc.element.mz.fs.closeSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>createReadStream (path, options)](#apidoc.element.mz.fs.createReadStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>createWriteStream (path, options)](#apidoc.element.mz.fs.createWriteStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>exists (filename, callback)](#apidoc.element.mz.fs.exists)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>existsSync (path)](#apidoc.element.mz.fs.existsSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fchmod ()](#apidoc.element.mz.fs.fchmod)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fchmodSync (fd, mode)](#apidoc.element.mz.fs.fchmodSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fchown ()](#apidoc.element.mz.fs.fchown)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fchownSync (fd, uid, gid)](#apidoc.element.mz.fs.fchownSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fdatasync ()](#apidoc.element.mz.fs.fdatasync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fdatasyncSync (fd)](#apidoc.element.mz.fs.fdatasyncSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fstat ()](#apidoc.element.mz.fs.fstat)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fstatSync (fd)](#apidoc.element.mz.fs.fstatSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fsync ()](#apidoc.element.mz.fs.fsync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>fsyncSync (fd)](#apidoc.element.mz.fs.fsyncSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>ftruncate ()](#apidoc.element.mz.fs.ftruncate)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>ftruncateSync (fd, len)](#apidoc.element.mz.fs.ftruncateSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>futimes ()](#apidoc.element.mz.fs.futimes)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>futimesSync (fd, atime, mtime)](#apidoc.element.mz.fs.futimesSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>link ()](#apidoc.element.mz.fs.link)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>linkSync (existingPath, newPath)](#apidoc.element.mz.fs.linkSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>lstat ()](#apidoc.element.mz.fs.lstat)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>lstatSync (path)](#apidoc.element.mz.fs.lstatSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>mkdir ()](#apidoc.element.mz.fs.mkdir)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>mkdirSync (path, mode)](#apidoc.element.mz.fs.mkdirSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>mkdtemp ()](#apidoc.element.mz.fs.mkdtemp)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>mkdtempSync (prefix, options)](#apidoc.element.mz.fs.mkdtempSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>open ()](#apidoc.element.mz.fs.open)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>openSync (path, flags, mode)](#apidoc.element.mz.fs.openSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>read ()](#apidoc.element.mz.fs.read)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>readFile ()](#apidoc.element.mz.fs.readFile)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>readFileSync (path, options)](#apidoc.element.mz.fs.readFileSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>readSync (fd, buffer, offset, length, position)](#apidoc.element.mz.fs.readSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>readdir ()](#apidoc.element.mz.fs.readdir)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>readdirSync (path, options)](#apidoc.element.mz.fs.readdirSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>readlink ()](#apidoc.element.mz.fs.readlink)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>readlinkSync (path, options)](#apidoc.element.mz.fs.readlinkSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>realpath ()](#apidoc.element.mz.fs.realpath)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>realpathSync (p, options)](#apidoc.element.mz.fs.realpathSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>rename ()](#apidoc.element.mz.fs.rename)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>renameSync (oldPath, newPath)](#apidoc.element.mz.fs.renameSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>rmdir ()](#apidoc.element.mz.fs.rmdir)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>rmdirSync (path)](#apidoc.element.mz.fs.rmdirSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>stat ()](#apidoc.element.mz.fs.stat)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>statSync (path)](#apidoc.element.mz.fs.statSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>symlink ()](#apidoc.element.mz.fs.symlink)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>symlinkSync (target, path, type)](#apidoc.element.mz.fs.symlinkSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>truncate ()](#apidoc.element.mz.fs.truncate)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>truncateSync (path, len)](#apidoc.element.mz.fs.truncateSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>unlink ()](#apidoc.element.mz.fs.unlink)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>unlinkSync (path)](#apidoc.element.mz.fs.unlinkSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>unwatchFile (filename, listener)](#apidoc.element.mz.fs.unwatchFile)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>utimes ()](#apidoc.element.mz.fs.utimes)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>utimesSync (path, atime, mtime)](#apidoc.element.mz.fs.utimesSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>watch (filename, options, listener)](#apidoc.element.mz.fs.watch)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>watchFile (filename, options, listener)](#apidoc.element.mz.fs.watchFile)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>write ()](#apidoc.element.mz.fs.write)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>writeFile ()](#apidoc.element.mz.fs.writeFile)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>writeFileSync (path, data, options)](#apidoc.element.mz.fs.writeFileSync)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>writeSync (fd, buffer, offset, length, position)](#apidoc.element.mz.fs.writeSync)
1.  number <span class="apidocSignatureSpan">mz.fs.</span>F_OK
1.  number <span class="apidocSignatureSpan">mz.fs.</span>R_OK
1.  number <span class="apidocSignatureSpan">mz.fs.</span>W_OK
1.  number <span class="apidocSignatureSpan">mz.fs.</span>X_OK
1.  object <span class="apidocSignatureSpan">mz.fs.</span>constants

#### [module mz.fs.ReadStream](#apidoc.module.mz.fs.ReadStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>ReadStream (path, options)](#apidoc.element.mz.fs.ReadStream.ReadStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.ReadStream.</span>super_ (options)](#apidoc.element.mz.fs.ReadStream.super_)

#### [module mz.fs.ReadStream.prototype](#apidoc.module.mz.fs.ReadStream.prototype)
1.  [function <span class="apidocSignatureSpan">mz.fs.ReadStream.prototype.</span>_read (n)](#apidoc.element.mz.fs.ReadStream.prototype._read)
1.  [function <span class="apidocSignatureSpan">mz.fs.ReadStream.prototype.</span>close (cb)](#apidoc.element.mz.fs.ReadStream.prototype.close)
1.  [function <span class="apidocSignatureSpan">mz.fs.ReadStream.prototype.</span>destroy ()](#apidoc.element.mz.fs.ReadStream.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">mz.fs.ReadStream.prototype.</span>open ()](#apidoc.element.mz.fs.ReadStream.prototype.open)

#### [module mz.fs.Stats](#apidoc.module.mz.fs.Stats)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.mz.fs.Stats.Stats)

#### [module mz.fs.Stats.prototype](#apidoc.module.mz.fs.Stats.prototype)
1.  [function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>_checkModeProperty (property)](#apidoc.element.mz.fs.Stats.prototype._checkModeProperty)
1.  [function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isBlockDevice ()](#apidoc.element.mz.fs.Stats.prototype.isBlockDevice)
1.  [function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isCharacterDevice ()](#apidoc.element.mz.fs.Stats.prototype.isCharacterDevice)
1.  [function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isDirectory ()](#apidoc.element.mz.fs.Stats.prototype.isDirectory)
1.  [function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isFIFO ()](#apidoc.element.mz.fs.Stats.prototype.isFIFO)
1.  [function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isFile ()](#apidoc.element.mz.fs.Stats.prototype.isFile)
1.  [function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isSocket ()](#apidoc.element.mz.fs.Stats.prototype.isSocket)
1.  [function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isSymbolicLink ()](#apidoc.element.mz.fs.Stats.prototype.isSymbolicLink)

#### [module mz.fs.WriteStream](#apidoc.module.mz.fs.WriteStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.</span>WriteStream (path, options)](#apidoc.element.mz.fs.WriteStream.WriteStream)
1.  [function <span class="apidocSignatureSpan">mz.fs.WriteStream.</span>super_ (options)](#apidoc.element.mz.fs.WriteStream.super_)

#### [module mz.fs.WriteStream.prototype](#apidoc.module.mz.fs.WriteStream.prototype)
1.  [function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>_write (data, encoding, cb)](#apidoc.element.mz.fs.WriteStream.prototype._write)
1.  [function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>_writev (data, cb)](#apidoc.element.mz.fs.WriteStream.prototype._writev)
1.  [function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>close (cb)](#apidoc.element.mz.fs.WriteStream.prototype.close)
1.  [function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>destroy ()](#apidoc.element.mz.fs.WriteStream.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>destroySoon (chunk, encoding, cb)](#apidoc.element.mz.fs.WriteStream.prototype.destroySoon)
1.  [function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>open ()](#apidoc.element.mz.fs.WriteStream.prototype.open)

#### [module mz.readline](#apidoc.module.mz.readline)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>Interface (input, output, completer, terminal)](#apidoc.element.mz.readline.Interface)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>clearLine (stream, dir)](#apidoc.element.mz.readline.clearLine)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>clearScreenDown (stream)](#apidoc.element.mz.readline.clearScreenDown)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>codePointAt ()](#apidoc.element.mz.readline.codePointAt)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>createInterface (input, output, completer, terminal)](#apidoc.element.mz.readline.createInterface)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>cursorTo (stream, x, y)](#apidoc.element.mz.readline.cursorTo)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>emitKeypressEvents (stream, iface)](#apidoc.element.mz.readline.emitKeypressEvents)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>getStringWidth ()](#apidoc.element.mz.readline.getStringWidth)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>isFullWidthCodePoint ()](#apidoc.element.mz.readline.isFullWidthCodePoint)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>moveCursor (stream, dx, dy)](#apidoc.element.mz.readline.moveCursor)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>stripVTControlCharacters ()](#apidoc.element.mz.readline.stripVTControlCharacters)

#### [module mz.readline.Interface](#apidoc.module.mz.readline.Interface)
1.  [function <span class="apidocSignatureSpan">mz.readline.</span>Interface (input, output, completer, terminal)](#apidoc.element.mz.readline.Interface.Interface)

#### [module mz.readline.Interface.prototype](#apidoc.module.mz.readline.Interface.prototype)
1.  [function <span class="apidocSignatureSpan">mz.readline.Interface.prototype.</span>question (question, callback)](#apidoc.element.mz.readline.Interface.prototype.question)

#### [module mz.zlib](#apidoc.module.mz.zlib)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Deflate (opts)](#apidoc.element.mz.zlib.Deflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>DeflateRaw (opts)](#apidoc.element.mz.zlib.DeflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Gunzip (opts)](#apidoc.element.mz.zlib.Gunzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Gzip (opts)](#apidoc.element.mz.zlib.Gzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Inflate (opts)](#apidoc.element.mz.zlib.Inflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>InflateRaw (opts)](#apidoc.element.mz.zlib.InflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Unzip (opts)](#apidoc.element.mz.zlib.Unzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Zlib ()](#apidoc.element.mz.zlib.Zlib)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>createDeflate (o)](#apidoc.element.mz.zlib.createDeflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>createDeflateRaw (o)](#apidoc.element.mz.zlib.createDeflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>createGunzip (o)](#apidoc.element.mz.zlib.createGunzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>createGzip (o)](#apidoc.element.mz.zlib.createGzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>createInflate (o)](#apidoc.element.mz.zlib.createInflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>createInflateRaw (o)](#apidoc.element.mz.zlib.createInflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>createUnzip (o)](#apidoc.element.mz.zlib.createUnzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>deflate ()](#apidoc.element.mz.zlib.deflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>deflateRaw ()](#apidoc.element.mz.zlib.deflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>deflateRawSync (buffer, opts)](#apidoc.element.mz.zlib.deflateRawSync)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>deflateSync (buffer, opts)](#apidoc.element.mz.zlib.deflateSync)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>gunzip ()](#apidoc.element.mz.zlib.gunzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>gunzipSync (buffer, opts)](#apidoc.element.mz.zlib.gunzipSync)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>gzip ()](#apidoc.element.mz.zlib.gzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>gzipSync (buffer, opts)](#apidoc.element.mz.zlib.gzipSync)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>inflate ()](#apidoc.element.mz.zlib.inflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>inflateRaw ()](#apidoc.element.mz.zlib.inflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>inflateRawSync (buffer, opts)](#apidoc.element.mz.zlib.inflateRawSync)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>inflateSync (buffer, opts)](#apidoc.element.mz.zlib.inflateSync)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>unzip ()](#apidoc.element.mz.zlib.unzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>unzipSync (buffer, opts)](#apidoc.element.mz.zlib.unzipSync)
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>ZLIB_VERNUM
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_BEST_COMPRESSION
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_BEST_SPEED
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_BLOCK
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_BUF_ERROR
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_DATA_ERROR
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_DEFAULT_CHUNK
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_DEFAULT_COMPRESSION
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_DEFAULT_LEVEL
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_DEFAULT_MEMLEVEL
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_DEFAULT_STRATEGY
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_DEFAULT_WINDOWBITS
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_ERRNO
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_FILTERED
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_FINISH
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_FIXED
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_FULL_FLUSH
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_HUFFMAN_ONLY
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_MAX_CHUNK
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_MAX_LEVEL
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_MAX_MEMLEVEL
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_MAX_WINDOWBITS
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_MEM_ERROR
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_MIN_CHUNK
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_MIN_LEVEL
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_MIN_MEMLEVEL
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_MIN_WINDOWBITS
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_NEED_DICT
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_NO_COMPRESSION
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_NO_FLUSH
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_OK
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_PARTIAL_FLUSH
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_RLE
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_STREAM_END
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_STREAM_ERROR
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_SYNC_FLUSH
1.  number <span class="apidocSignatureSpan">mz.zlib.</span>Z_VERSION_ERROR
1.  object <span class="apidocSignatureSpan">mz.zlib.</span>codes
1.  string <span class="apidocSignatureSpan">mz.zlib.</span>ZLIB_VERSION

#### [module mz.zlib.Deflate](#apidoc.module.mz.zlib.Deflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Deflate (opts)](#apidoc.element.mz.zlib.Deflate.Deflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Deflate.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Deflate.super_)

#### [module mz.zlib.Deflate.super_.prototype](#apidoc.module.mz.zlib.Deflate.super_.prototype)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>_flush (callback)](#apidoc.element.mz.zlib.Deflate.super_.prototype._flush)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>_processChunk (chunk, flushFlag, cb)](#apidoc.element.mz.zlib.Deflate.super_.prototype._processChunk)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.mz.zlib.Deflate.super_.prototype._transform)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>close (callback)](#apidoc.element.mz.zlib.Deflate.super_.prototype.close)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>flush (kind, callback)](#apidoc.element.mz.zlib.Deflate.super_.prototype.flush)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>params (level, strategy, callback)](#apidoc.element.mz.zlib.Deflate.super_.prototype.params)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>reset ()](#apidoc.element.mz.zlib.Deflate.super_.prototype.reset)

#### [module mz.zlib.DeflateRaw](#apidoc.module.mz.zlib.DeflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>DeflateRaw (opts)](#apidoc.element.mz.zlib.DeflateRaw.DeflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.DeflateRaw.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.DeflateRaw.super_)

#### [module mz.zlib.Gunzip](#apidoc.module.mz.zlib.Gunzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Gunzip (opts)](#apidoc.element.mz.zlib.Gunzip.Gunzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Gunzip.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Gunzip.super_)

#### [module mz.zlib.Gzip](#apidoc.module.mz.zlib.Gzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Gzip (opts)](#apidoc.element.mz.zlib.Gzip.Gzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Gzip.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Gzip.super_)

#### [module mz.zlib.Inflate](#apidoc.module.mz.zlib.Inflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Inflate (opts)](#apidoc.element.mz.zlib.Inflate.Inflate)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Inflate.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Inflate.super_)

#### [module mz.zlib.InflateRaw](#apidoc.module.mz.zlib.InflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>InflateRaw (opts)](#apidoc.element.mz.zlib.InflateRaw.InflateRaw)
1.  [function <span class="apidocSignatureSpan">mz.zlib.InflateRaw.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.InflateRaw.super_)

#### [module mz.zlib.Unzip](#apidoc.module.mz.zlib.Unzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Unzip (opts)](#apidoc.element.mz.zlib.Unzip.Unzip)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Unzip.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Unzip.super_)

#### [module mz.zlib.Zlib](#apidoc.module.mz.zlib.Zlib)
1.  [function <span class="apidocSignatureSpan">mz.zlib.</span>Zlib ()](#apidoc.element.mz.zlib.Zlib.Zlib)

#### [module mz.zlib.Zlib.prototype](#apidoc.module.mz.zlib.Zlib.prototype)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>close ()](#apidoc.element.mz.zlib.Zlib.prototype.close)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>init ()](#apidoc.element.mz.zlib.Zlib.prototype.init)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>params ()](#apidoc.element.mz.zlib.Zlib.prototype.params)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>reset ()](#apidoc.element.mz.zlib.Zlib.prototype.reset)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>write ()](#apidoc.element.mz.zlib.Zlib.prototype.write)
1.  [function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>writeSync ()](#apidoc.element.mz.zlib.Zlib.prototype.writeSync)



# <a name="apidoc.module.mz"></a>[module mz](#apidoc.module.mz)

#### <a name="apidoc.element.mz.child_process.ChildProcess"></a>[function <span class="apidocSignatureSpan">mz.</span>child_process.ChildProcess ()](#apidoc.element.mz.child_process.ChildProcess)
- description and source-code
```javascript
function ChildProcess() {
  EventEmitter.call(this);

  var self = this;

  this._closesNeeded = 1;
  this._closesGot = 0;
  this.connected = false;

  this.signalCode = null;
  this.exitCode = null;
  this.killed = false;
  this.spawnfile = null;

  this._handle = new Process();
  this._handle.owner = this;

  this._handle.onexit = function(exitCode, signalCode) {
    //
    // follow 0.4.x behaviour:
    //
    // - normally terminated processes don't touch this.signalCode
    // - signaled processes don't touch this.exitCode
    //
    // new in 0.9.x:
    //
    // - spawn failures are reported with exitCode < 0
    //
    var syscall = self.spawnfile ? 'spawn ' + self.spawnfile : 'spawn';
    var err = (exitCode < 0) ? errnoException(exitCode, syscall) : null;

    if (signalCode) {
      self.signalCode = signalCode;
    } else {
      self.exitCode = exitCode;
    }

    if (self.stdin) {
      self.stdin.destroy();
    }

    self._handle.close();
    self._handle = null;

    if (exitCode < 0) {
      if (self.spawnfile)
        err.path = self.spawnfile;

      err.spawnargs = self.spawnargs.slice(1);
      self.emit('error', err);
    } else {
      self.emit('exit', self.exitCode, self.signalCode);
    }

    // if any of the stdio streams have not been touched,
    // then pull all the data through so that it can get the
    // eof and emit a 'close' event.
    // Do it on nextTick so that the user has one last chance
    // to consume the output, if for example they only want to
    // start reading the data once the process exits.
    process.nextTick(flushStdio, self);

    maybeClose(self);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Certificate"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.Certificate ()](#apidoc.element.mz.crypto.Certificate)
- description and source-code
```javascript
function Certificate() {
  if (!(this instanceof Certificate))
    return new Certificate();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.Cipher (cipher, password, options)](#apidoc.element.mz.crypto.Cipher)
- description and source-code
```javascript
function Cipher(cipher, password, options) {
  if (!(this instanceof Cipher))
    return new Cipher(cipher, password, options);
  this._handle = new binding.CipherBase(true);

  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.Cipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Cipheriv)
- description and source-code
```javascript
function Cipheriv(cipher, key, iv, options) {
  if (!(this instanceof Cipheriv))
    return new Cipheriv(cipher, key, iv, options);
  this._handle = new binding.CipherBase(true);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.Decipher (cipher, password, options)](#apidoc.element.mz.crypto.Decipher)
- description and source-code
```javascript
function Decipher(cipher, password, options) {
  if (!(this instanceof Decipher))
    return new Decipher(cipher, password, options);

  this._handle = new binding.CipherBase(false);
  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.Decipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Decipheriv)
- description and source-code
```javascript
function Decipheriv(cipher, key, iv, options) {
  if (!(this instanceof Decipheriv))
    return new Decipheriv(cipher, key, iv, options);

  this._handle = new binding.CipherBase(false);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellman"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.DiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.mz.crypto.DiffieHellman)
- description and source-code
```javascript
function DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding) {
  if (!(this instanceof DiffieHellman))
    return new DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding);

  if (!(sizeOrKey instanceof Buffer) &&
      typeof sizeOrKey !== 'number' &&
      typeof sizeOrKey !== 'string')
    throw new TypeError('First argument should be number, string or Buffer');

  if (keyEncoding) {
    if (typeof keyEncoding !== 'string' ||
        (!Buffer.isEncoding(keyEncoding) && keyEncoding !== 'buffer')) {
      genEncoding = generator;
      generator = keyEncoding;
      keyEncoding = false;
    }
  }

  keyEncoding = keyEncoding || exports.DEFAULT_ENCODING;
  genEncoding = genEncoding || exports.DEFAULT_ENCODING;

  if (typeof sizeOrKey !== 'number')
    sizeOrKey = toBuf(sizeOrKey, keyEncoding);

  if (!generator)
    generator = DH_GENERATOR;
  else if (typeof generator !== 'number')
    generator = toBuf(generator, genEncoding);

  this._handle = new binding.DiffieHellman(sizeOrKey, generator);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hash"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.Hash (algorithm, options)](#apidoc.element.mz.crypto.Hash)
- description and source-code
```javascript
function Hash(algorithm, options) {
  if (!(this instanceof Hash))
    return new Hash(algorithm, options);
  this._handle = new binding.Hash(algorithm);
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hmac"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.Hmac (hmac, key, options)](#apidoc.element.mz.crypto.Hmac)
- description and source-code
```javascript
function Hmac(hmac, key, options) {
  if (!(this instanceof Hmac))
    return new Hmac(hmac, key, options);
  this._handle = new binding.Hmac();
  this._handle.init(hmac, toBuf(key));
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Sign"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.Sign (algorithm, options)](#apidoc.element.mz.crypto.Sign)
- description and source-code
```javascript
function Sign(algorithm, options) {
  if (!(this instanceof Sign))
    return new Sign(algorithm, options);
  this._handle = new binding.Sign();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Verify"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.Verify (algorithm, options)](#apidoc.element.mz.crypto.Verify)
- description and source-code
```javascript
function Verify(algorithm, options) {
  if (!(this instanceof Verify))
    return new Verify(algorithm, options);

  this._handle = new binding.Verify();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getDiffieHellman"></a>[function <span class="apidocSignatureSpan">mz.</span>crypto.getDiffieHellman (name)](#apidoc.element.mz.crypto.getDiffieHellman)
- description and source-code
```javascript
function DiffieHellmanGroup(name) {
  if (!(this instanceof DiffieHellmanGroup))
    return new DiffieHellmanGroup(name);
  this._handle = new binding.DiffieHellmanGroup(name);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.ReadStream"></a>[function <span class="apidocSignatureSpan">mz.</span>fs.ReadStream (path, options)](#apidoc.element.mz.fs.ReadStream)
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

#### <a name="apidoc.element.mz.fs.Stats"></a>[function <span class="apidocSignatureSpan">mz.</span>fs.Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.mz.fs.Stats)
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

#### <a name="apidoc.element.mz.fs.WriteStream"></a>[function <span class="apidocSignatureSpan">mz.</span>fs.WriteStream (path, options)](#apidoc.element.mz.fs.WriteStream)
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

#### <a name="apidoc.element.mz.readline.Interface"></a>[function <span class="apidocSignatureSpan">mz.</span>readline.Interface (input, output, completer, terminal)](#apidoc.element.mz.readline.Interface)
- description and source-code
```javascript
function InterfaceAsPromised(input, output, completer, terminal) {
  if (arguments.length === 1) {
    var options = input

    if (typeof options.completer === 'function') {
      options = objectAssign({}, options, {
        completer: wrapCompleter(options.completer)
      })
    }

    Interface.call(this, options)
  } else {
    if (typeof completer === 'function') {
      completer = wrapCompleter(completer)
    }

    Interface.call(this, input, output, completer, terminal)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Deflate"></a>[function <span class="apidocSignatureSpan">mz.</span>zlib.Deflate (opts)](#apidoc.element.mz.zlib.Deflate)
- description and source-code
```javascript
function Deflate(opts) {
  if (!(this instanceof Deflate)) return new Deflate(opts);
  Zlib.call(this, opts, binding.DEFLATE);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.DeflateRaw"></a>[function <span class="apidocSignatureSpan">mz.</span>zlib.DeflateRaw (opts)](#apidoc.element.mz.zlib.DeflateRaw)
- description and source-code
```javascript
function DeflateRaw(opts) {
  if (!(this instanceof DeflateRaw)) return new DeflateRaw(opts);
  Zlib.call(this, opts, binding.DEFLATERAW);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Gunzip"></a>[function <span class="apidocSignatureSpan">mz.</span>zlib.Gunzip (opts)](#apidoc.element.mz.zlib.Gunzip)
- description and source-code
```javascript
function Gunzip(opts) {
  if (!(this instanceof Gunzip)) return new Gunzip(opts);
  Zlib.call(this, opts, binding.GUNZIP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Gzip"></a>[function <span class="apidocSignatureSpan">mz.</span>zlib.Gzip (opts)](#apidoc.element.mz.zlib.Gzip)
- description and source-code
```javascript
function Gzip(opts) {
  if (!(this instanceof Gzip)) return new Gzip(opts);
  Zlib.call(this, opts, binding.GZIP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Inflate"></a>[function <span class="apidocSignatureSpan">mz.</span>zlib.Inflate (opts)](#apidoc.element.mz.zlib.Inflate)
- description and source-code
```javascript
function Inflate(opts) {
  if (!(this instanceof Inflate)) return new Inflate(opts);
  Zlib.call(this, opts, binding.INFLATE);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.InflateRaw"></a>[function <span class="apidocSignatureSpan">mz.</span>zlib.InflateRaw (opts)](#apidoc.element.mz.zlib.InflateRaw)
- description and source-code
```javascript
function InflateRaw(opts) {
  if (!(this instanceof InflateRaw)) return new InflateRaw(opts);
  Zlib.call(this, opts, binding.INFLATERAW);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Unzip"></a>[function <span class="apidocSignatureSpan">mz.</span>zlib.Unzip (opts)](#apidoc.element.mz.zlib.Unzip)
- description and source-code
```javascript
function Unzip(opts) {
  if (!(this instanceof Unzip)) return new Unzip(opts);
  Zlib.call(this, opts, binding.UNZIP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Zlib"></a>[function <span class="apidocSignatureSpan">mz.</span>zlib.Zlib ()](#apidoc.element.mz.zlib.Zlib)
- description and source-code
```javascript
function Zlib() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.child_process"></a>[module mz.child_process](#apidoc.module.mz.child_process)

#### <a name="apidoc.element.mz.child_process.ChildProcess"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>ChildProcess ()](#apidoc.element.mz.child_process.ChildProcess)
- description and source-code
```javascript
function ChildProcess() {
  EventEmitter.call(this);

  var self = this;

  this._closesNeeded = 1;
  this._closesGot = 0;
  this.connected = false;

  this.signalCode = null;
  this.exitCode = null;
  this.killed = false;
  this.spawnfile = null;

  this._handle = new Process();
  this._handle.owner = this;

  this._handle.onexit = function(exitCode, signalCode) {
    //
    // follow 0.4.x behaviour:
    //
    // - normally terminated processes don't touch this.signalCode
    // - signaled processes don't touch this.exitCode
    //
    // new in 0.9.x:
    //
    // - spawn failures are reported with exitCode < 0
    //
    var syscall = self.spawnfile ? 'spawn ' + self.spawnfile : 'spawn';
    var err = (exitCode < 0) ? errnoException(exitCode, syscall) : null;

    if (signalCode) {
      self.signalCode = signalCode;
    } else {
      self.exitCode = exitCode;
    }

    if (self.stdin) {
      self.stdin.destroy();
    }

    self._handle.close();
    self._handle = null;

    if (exitCode < 0) {
      if (self.spawnfile)
        err.path = self.spawnfile;

      err.spawnargs = self.spawnargs.slice(1);
      self.emit('error', err);
    } else {
      self.emit('exit', self.exitCode, self.signalCode);
    }

    // if any of the stdio streams have not been touched,
    // then pull all the data through so that it can get the
    // eof and emit a 'close' event.
    // Do it on nextTick so that the user has one last chance
    // to consume the output, if for example they only want to
    // start reading the data once the process exits.
    process.nextTick(flushStdio, self);

    maybeClose(self);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process._forkChild"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>_forkChild (fd)](#apidoc.element.mz.child_process._forkChild)
- description and source-code
```javascript
_forkChild = function (fd) {
  // set process.send()
  var p = new Pipe(true);
  p.open(fd);
  p.unref();
  const control = setupChannel(process, p);
  process.on('newListener', function(name) {
    if (name === 'message' || name === 'disconnect') control.ref();
  });
  process.on('removeListener', function(name) {
    if (name === 'message' || name === 'disconnect') control.unref();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.exec"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>exec ()](#apidoc.element.mz.child_process.exec)
- description and source-code
```javascript
exec = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.execFile"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>execFile ()](#apidoc.element.mz.child_process.execFile)
- description and source-code
```javascript
execFile = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.execFileSync"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>execFileSync ()](#apidoc.element.mz.child_process.execFileSync)
- description and source-code
```javascript
function execFileSync() {
  var opts = normalizeSpawnArguments.apply(null, arguments);
  var inheritStderr = !opts.options.stdio;

  var ret = spawnSync(opts.file, opts.args.slice(1), opts.options);

  if (inheritStderr && ret.stderr)
    process.stderr.write(ret.stderr);

  var err = checkExecSyncError(ret);

  if (err)
    throw err;
  else
    return ret.stdout;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.execSync"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>execSync (command)](#apidoc.element.mz.child_process.execSync)
- description and source-code
```javascript
function execSync(command) {
  var opts = normalizeExecArgs.apply(null, arguments);
  var inheritStderr = !opts.options.stdio;

  var ret = spawnSync(opts.file, opts.options);
  ret.cmd = command;

  if (inheritStderr && ret.stderr)
    process.stderr.write(ret.stderr);

  var err = checkExecSyncError(ret);

  if (err)
    throw err;
  else
    return ret.stdout;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.fork"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>fork (modulePath)](#apidoc.element.mz.child_process.fork)
- description and source-code
```javascript
fork = function (modulePath) {

  // Get options and args arguments.
  var options, args, execArgv;
  if (Array.isArray(arguments[1])) {
    args = arguments[1];
    options = util._extend({}, arguments[2]);
  } else if (arguments[1] && typeof arguments[1] !== 'object') {
    throw new TypeError('Incorrect value of args option');
  } else {
    args = [];
    options = util._extend({}, arguments[1]);
  }

  // Prepare arguments for fork:
  execArgv = options.execArgv || process.execArgv;

  if (execArgv === process.execArgv && process._eval != null) {
    const index = execArgv.lastIndexOf(process._eval);
    if (index > 0) {
      // Remove the -e switch to avoid fork bombing ourselves.
      execArgv = execArgv.slice();
      execArgv.splice(index - 1, 2);
    }
  }

  args = execArgv.concat([modulePath], args);

  if (!Array.isArray(options.stdio)) {
    // Use a separate fd=3 for the IPC channel. Inherit stdin, stdout,
    // and stderr from the parent if silent isn't set.
    options.stdio = options.silent ? ['pipe', 'pipe', 'pipe', 'ipc'] :
        [0, 1, 2, 'ipc'];
  } else if (options.stdio.indexOf('ipc') === -1) {
    throw new TypeError('Forked processes must have an IPC channel');
  }

  options.execPath = options.execPath || process.execPath;

  return spawn(options.execPath, args, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.spawn"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>spawn ()](#apidoc.element.mz.child_process.spawn)
- description and source-code
```javascript
spawn = function () {
  var opts = normalizeSpawnArguments.apply(null, arguments);
  var options = opts.options;
  var child = new ChildProcess();

  debug('spawn', opts.args, options);

  child.spawn({
    file: opts.file,
    args: opts.args,
    cwd: options.cwd,
    windowsVerbatimArguments: !!options.windowsVerbatimArguments,
    detached: !!options.detached,
    envPairs: opts.envPairs,
    stdio: options.stdio,
    uid: options.uid,
    gid: options.gid
  });

  return child;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.spawnSync"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>spawnSync ()](#apidoc.element.mz.child_process.spawnSync)
- description and source-code
```javascript
function spawnSync() {
  var opts = normalizeSpawnArguments.apply(null, arguments);

  var options = opts.options;

  var i;

  debug('spawnSync', opts.args, options);

  options.file = opts.file;
  options.args = opts.args;
  options.envPairs = opts.envPairs;

  if (options.killSignal)
    options.killSignal = lookupSignal(options.killSignal);

  options.stdio = _validateStdio(options.stdio || 'pipe', true).stdio;

  if (options.input) {
    var stdin = options.stdio[0] = util._extend({}, options.stdio[0]);
    stdin.input = options.input;
  }

  // We may want to pass data in on any given fd, ensure it is a valid buffer
  for (i = 0; i < options.stdio.length; i++) {
    var input = options.stdio[i] && options.stdio[i].input;
    if (input != null) {
      var pipe = options.stdio[i] = util._extend({}, options.stdio[i]);
      if (Buffer.isBuffer(input))
        pipe.input = input;
      else if (typeof input === 'string')
        pipe.input = Buffer.from(input, options.encoding);
      else
        throw new TypeError(util.format(
            'stdio[%d] should be Buffer or string not %s',
            i,
            typeof input));
    }
  }

  var result = spawn_sync.spawn(options);

  if (result.output && options.encoding && options.encoding !== 'buffer') {
    for (i = 0; i < result.output.length; i++) {
      if (!result.output[i])
        continue;
      result.output[i] = result.output[i].toString(options.encoding);
    }
  }

  result.stdout = result.output && result.output[1];
  result.stderr = result.output && result.output[2];

  if (result.error) {
    result.error = errnoException(result.error, 'spawnSync ' + opts.file);
    result.error.path = opts.file;
    result.error.spawnargs = opts.args.slice(1);
  }

  util._extend(result, opts);

  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.child_process.ChildProcess"></a>[module mz.child_process.ChildProcess](#apidoc.module.mz.child_process.ChildProcess)

#### <a name="apidoc.element.mz.child_process.ChildProcess.ChildProcess"></a>[function <span class="apidocSignatureSpan">mz.child_process.</span>ChildProcess ()](#apidoc.element.mz.child_process.ChildProcess.ChildProcess)
- description and source-code
```javascript
function ChildProcess() {
  EventEmitter.call(this);

  var self = this;

  this._closesNeeded = 1;
  this._closesGot = 0;
  this.connected = false;

  this.signalCode = null;
  this.exitCode = null;
  this.killed = false;
  this.spawnfile = null;

  this._handle = new Process();
  this._handle.owner = this;

  this._handle.onexit = function(exitCode, signalCode) {
    //
    // follow 0.4.x behaviour:
    //
    // - normally terminated processes don't touch this.signalCode
    // - signaled processes don't touch this.exitCode
    //
    // new in 0.9.x:
    //
    // - spawn failures are reported with exitCode < 0
    //
    var syscall = self.spawnfile ? 'spawn ' + self.spawnfile : 'spawn';
    var err = (exitCode < 0) ? errnoException(exitCode, syscall) : null;

    if (signalCode) {
      self.signalCode = signalCode;
    } else {
      self.exitCode = exitCode;
    }

    if (self.stdin) {
      self.stdin.destroy();
    }

    self._handle.close();
    self._handle = null;

    if (exitCode < 0) {
      if (self.spawnfile)
        err.path = self.spawnfile;

      err.spawnargs = self.spawnargs.slice(1);
      self.emit('error', err);
    } else {
      self.emit('exit', self.exitCode, self.signalCode);
    }

    // if any of the stdio streams have not been touched,
    // then pull all the data through so that it can get the
    // eof and emit a 'close' event.
    // Do it on nextTick so that the user has one last chance
    // to consume the output, if for example they only want to
    // start reading the data once the process exits.
    process.nextTick(flushStdio, self);

    maybeClose(self);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.ChildProcess.super_"></a>[function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.</span>super_ ()](#apidoc.element.mz.child_process.ChildProcess.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.child_process.ChildProcess.prototype"></a>[module mz.child_process.ChildProcess.prototype](#apidoc.module.mz.child_process.ChildProcess.prototype)

#### <a name="apidoc.element.mz.child_process.ChildProcess.prototype.kill"></a>[function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.prototype.</span>kill (sig)](#apidoc.element.mz.child_process.ChildProcess.prototype.kill)
- description and source-code
```javascript
kill = function (sig) {
  var signal;

  if (sig === 0) {
    signal = 0;
  } else if (!sig) {
    signal = constants['SIGTERM'];
  } else {
    signal = constants[sig];
  }

  if (signal === undefined) {
    throw new Error('Unknown signal: ' + sig);
  }

  if (this._handle) {
    var err = this._handle.kill(signal);
    if (err === 0) {
<span class="apidocCodeCommentSpan">      /* Success. */
</span>      this.killed = true;
      return true;
    }
    if (err === uv.UV_ESRCH) {
      /* Already dead. */
    } else if (err === uv.UV_EINVAL || err === uv.UV_ENOSYS) {
      /* The underlying platform doesn't support this signal. */
      throw errnoException(err, 'kill');
    } else {
      /* Other error, almost certainly EPERM. */
      this.emit('error', errnoException(err, 'kill'));
    }
  }

  /* Kill didn't succeed. */
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.ChildProcess.prototype.ref"></a>[function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.prototype.</span>ref ()](#apidoc.element.mz.child_process.ChildProcess.prototype.ref)
- description and source-code
```javascript
ref = function () {
  if (this._handle) this._handle.ref();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.ChildProcess.prototype.spawn"></a>[function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.prototype.</span>spawn (options)](#apidoc.element.mz.child_process.ChildProcess.prototype.spawn)
- description and source-code
```javascript
spawn = function (options) {
  const self = this;
  var ipc;
  var ipcFd;
  var i;
  // If no 'stdio' option was given - use default
  var stdio = options.stdio || 'pipe';

  stdio = _validateStdio(stdio, false);

  ipc = stdio.ipc;
  ipcFd = stdio.ipcFd;
  stdio = options.stdio = stdio.stdio;

  if (ipc !== undefined) {
    // Let child process know about opened IPC channel
    options.envPairs = options.envPairs || [];
    options.envPairs.push('NODE_CHANNEL_FD=' + ipcFd);
  }

  this.spawnfile = options.file;
  this.spawnargs = options.args;

  var err = this._handle.spawn(options);

  // Run-time errors should emit an error, not throw an exception.
  if (err === uv.UV_EAGAIN ||
      err === uv.UV_EMFILE ||
      err === uv.UV_ENFILE ||
      err === uv.UV_ENOENT) {
    process.nextTick(onErrorNT, self, err);
    // There is no point in continuing when we've hit EMFILE or ENFILE
    // because we won't be able to set up the stdio file descriptors.
    // It's kind of silly that the de facto spec for ENOENT (the test suite)
    // mandates that stdio _is_ set up, even if there is no process on the
    // receiving end, but it is what it is.
    if (err !== uv.UV_ENOENT) return err;
  } else if (err) {
    // Close all opened fds on error
    for (i = 0; i < stdio.length; i++) {
      const stream = stdio[i];
      if (stream.type === 'pipe') {
        stream.handle.close();
      }
    }

    this._handle.close();
    this._handle = null;
    throw errnoException(err, 'spawn');
  }

  this.pid = this._handle.pid;

  for (i = 0; i < stdio.length; i++) {
    const stream = stdio[i];
    if (stream.type === 'ignore') continue;

    if (stream.ipc) {
      self._closesNeeded++;
      continue;
    }

    if (stream.handle) {
      // when i === 0 - we're dealing with stdin
      // (which is the only one writable pipe)
      stream.socket = createSocket(self.pid !== 0 ?
          stream.handle : null, i > 0);

      if (i > 0 && self.pid !== 0) {
        self._closesNeeded++;
        stream.socket.on('close', function() {
          maybeClose(self);
        });
      }
    }
  }

  this.stdin = stdio.length >= 1 && stdio[0].socket !== undefined ?
      stdio[0].socket : null;
  this.stdout = stdio.length >= 2 && stdio[1].socket !== undefined ?
      stdio[1].socket : null;
  this.stderr = stdio.length >= 3 && stdio[2].socket !== undefined ?
      stdio[2].socket : null;

  this.stdio = stdio.map(function(stdio) {
    return stdio.socket === undefined ? null : stdio.socket;
  });

  // Add .send() method and start listening for IPC data
  if (ipc !== undefined) setupChannel(this, ipc);

  return err;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.child_process.ChildProcess.prototype.unref"></a>[function <span class="apidocSignatureSpan">mz.child_process.ChildProcess.prototype.</span>unref ()](#apidoc.element.mz.child_process.ChildProcess.prototype.unref)
- description and source-code
```javascript
unref = function () {
  if (this._handle) this._handle.unref();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto"></a>[module mz.crypto](#apidoc.module.mz.crypto)

#### <a name="apidoc.element.mz.crypto.Certificate"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Certificate ()](#apidoc.element.mz.crypto.Certificate)
- description and source-code
```javascript
function Certificate() {
  if (!(this instanceof Certificate))
    return new Certificate();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Cipher (cipher, password, options)](#apidoc.element.mz.crypto.Cipher)
- description and source-code
```javascript
function Cipher(cipher, password, options) {
  if (!(this instanceof Cipher))
    return new Cipher(cipher, password, options);
  this._handle = new binding.CipherBase(true);

  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Cipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Cipheriv)
- description and source-code
```javascript
function Cipheriv(cipher, key, iv, options) {
  if (!(this instanceof Cipheriv))
    return new Cipheriv(cipher, key, iv, options);
  this._handle = new binding.CipherBase(true);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Decipher (cipher, password, options)](#apidoc.element.mz.crypto.Decipher)
- description and source-code
```javascript
function Decipher(cipher, password, options) {
  if (!(this instanceof Decipher))
    return new Decipher(cipher, password, options);

  this._handle = new binding.CipherBase(false);
  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Decipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Decipheriv)
- description and source-code
```javascript
function Decipheriv(cipher, key, iv, options) {
  if (!(this instanceof Decipheriv))
    return new Decipheriv(cipher, key, iv, options);

  this._handle = new binding.CipherBase(false);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellman"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>DiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.mz.crypto.DiffieHellman)
- description and source-code
```javascript
function DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding) {
  if (!(this instanceof DiffieHellman))
    return new DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding);

  if (!(sizeOrKey instanceof Buffer) &&
      typeof sizeOrKey !== 'number' &&
      typeof sizeOrKey !== 'string')
    throw new TypeError('First argument should be number, string or Buffer');

  if (keyEncoding) {
    if (typeof keyEncoding !== 'string' ||
        (!Buffer.isEncoding(keyEncoding) && keyEncoding !== 'buffer')) {
      genEncoding = generator;
      generator = keyEncoding;
      keyEncoding = false;
    }
  }

  keyEncoding = keyEncoding || exports.DEFAULT_ENCODING;
  genEncoding = genEncoding || exports.DEFAULT_ENCODING;

  if (typeof sizeOrKey !== 'number')
    sizeOrKey = toBuf(sizeOrKey, keyEncoding);

  if (!generator)
    generator = DH_GENERATOR;
  else if (typeof generator !== 'number')
    generator = toBuf(generator, genEncoding);

  this._handle = new binding.DiffieHellman(sizeOrKey, generator);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellmanGroup"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>DiffieHellmanGroup (name)](#apidoc.element.mz.crypto.DiffieHellmanGroup)
- description and source-code
```javascript
function DiffieHellmanGroup(name) {
  if (!(this instanceof DiffieHellmanGroup))
    return new DiffieHellmanGroup(name);
  this._handle = new binding.DiffieHellmanGroup(name);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hash"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Hash (algorithm, options)](#apidoc.element.mz.crypto.Hash)
- description and source-code
```javascript
function Hash(algorithm, options) {
  if (!(this instanceof Hash))
    return new Hash(algorithm, options);
  this._handle = new binding.Hash(algorithm);
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hmac"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Hmac (hmac, key, options)](#apidoc.element.mz.crypto.Hmac)
- description and source-code
```javascript
function Hmac(hmac, key, options) {
  if (!(this instanceof Hmac))
    return new Hmac(hmac, key, options);
  this._handle = new binding.Hmac();
  this._handle.init(hmac, toBuf(key));
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Sign"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Sign (algorithm, options)](#apidoc.element.mz.crypto.Sign)
- description and source-code
```javascript
function Sign(algorithm, options) {
  if (!(this instanceof Sign))
    return new Sign(algorithm, options);
  this._handle = new binding.Sign();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Verify"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Verify (algorithm, options)](#apidoc.element.mz.crypto.Verify)
- description and source-code
```javascript
function Verify(algorithm, options) {
  if (!(this instanceof Verify))
    return new Verify(algorithm, options);

  this._handle = new binding.Verify();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto._toBuf"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>_toBuf (str, encoding)](#apidoc.element.mz.crypto._toBuf)
- description and source-code
```javascript
function toBuf(str, encoding) {
  if (typeof str === 'string') {
    if (encoding === 'buffer' || !encoding)
      encoding = 'utf8';
    return Buffer.from(str, encoding);
  }
  return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createCipher"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createCipher (cipher, password, options)](#apidoc.element.mz.crypto.createCipher)
- description and source-code
```javascript
function Cipher(cipher, password, options) {
  if (!(this instanceof Cipher))
    return new Cipher(cipher, password, options);
  this._handle = new binding.CipherBase(true);

  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createCipheriv"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createCipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.createCipheriv)
- description and source-code
```javascript
function Cipheriv(cipher, key, iv, options) {
  if (!(this instanceof Cipheriv))
    return new Cipheriv(cipher, key, iv, options);
  this._handle = new binding.CipherBase(true);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createDecipher"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createDecipher (cipher, password, options)](#apidoc.element.mz.crypto.createDecipher)
- description and source-code
```javascript
function Decipher(cipher, password, options) {
  if (!(this instanceof Decipher))
    return new Decipher(cipher, password, options);

  this._handle = new binding.CipherBase(false);
  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createDecipheriv"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createDecipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.createDecipheriv)
- description and source-code
```javascript
function Decipheriv(cipher, key, iv, options) {
  if (!(this instanceof Decipheriv))
    return new Decipheriv(cipher, key, iv, options);

  this._handle = new binding.CipherBase(false);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createDiffieHellman"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createDiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.mz.crypto.createDiffieHellman)
- description and source-code
```javascript
function DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding) {
  if (!(this instanceof DiffieHellman))
    return new DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding);

  if (!(sizeOrKey instanceof Buffer) &&
      typeof sizeOrKey !== 'number' &&
      typeof sizeOrKey !== 'string')
    throw new TypeError('First argument should be number, string or Buffer');

  if (keyEncoding) {
    if (typeof keyEncoding !== 'string' ||
        (!Buffer.isEncoding(keyEncoding) && keyEncoding !== 'buffer')) {
      genEncoding = generator;
      generator = keyEncoding;
      keyEncoding = false;
    }
  }

  keyEncoding = keyEncoding || exports.DEFAULT_ENCODING;
  genEncoding = genEncoding || exports.DEFAULT_ENCODING;

  if (typeof sizeOrKey !== 'number')
    sizeOrKey = toBuf(sizeOrKey, keyEncoding);

  if (!generator)
    generator = DH_GENERATOR;
  else if (typeof generator !== 'number')
    generator = toBuf(generator, genEncoding);

  this._handle = new binding.DiffieHellman(sizeOrKey, generator);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createDiffieHellmanGroup"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createDiffieHellmanGroup (name)](#apidoc.element.mz.crypto.createDiffieHellmanGroup)
- description and source-code
```javascript
function DiffieHellmanGroup(name) {
  if (!(this instanceof DiffieHellmanGroup))
    return new DiffieHellmanGroup(name);
  this._handle = new binding.DiffieHellmanGroup(name);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createECDH"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createECDH (curve)](#apidoc.element.mz.crypto.createECDH)
- description and source-code
```javascript
function createECDH(curve) {
  return new ECDH(curve);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createHash"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createHash (algorithm, options)](#apidoc.element.mz.crypto.createHash)
- description and source-code
```javascript
function Hash(algorithm, options) {
  if (!(this instanceof Hash))
    return new Hash(algorithm, options);
  this._handle = new binding.Hash(algorithm);
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createHmac"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createHmac (hmac, key, options)](#apidoc.element.mz.crypto.createHmac)
- description and source-code
```javascript
function Hmac(hmac, key, options) {
  if (!(this instanceof Hmac))
    return new Hmac(hmac, key, options);
  this._handle = new binding.Hmac();
  this._handle.init(hmac, toBuf(key));
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createSign"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createSign (algorithm, options)](#apidoc.element.mz.crypto.createSign)
- description and source-code
```javascript
function Sign(algorithm, options) {
  if (!(this instanceof Sign))
    return new Sign(algorithm, options);
  this._handle = new binding.Sign();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.createVerify"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>createVerify (algorithm, options)](#apidoc.element.mz.crypto.createVerify)
- description and source-code
```javascript
function Verify(algorithm, options) {
  if (!(this instanceof Verify))
    return new Verify(algorithm, options);

  this._handle = new binding.Verify();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getCiphers"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>getCiphers ()](#apidoc.element.mz.crypto.getCiphers)
- description and source-code
```javascript
() => {
  if (result === undefined)
    result = fn();
  return result.slice();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getCurves"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>getCurves ()](#apidoc.element.mz.crypto.getCurves)
- description and source-code
```javascript
() => {
  if (result === undefined)
    result = fn();
  return result.slice();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getDiffieHellman"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>getDiffieHellman (name)](#apidoc.element.mz.crypto.getDiffieHellman)
- description and source-code
```javascript
function DiffieHellmanGroup(name) {
  if (!(this instanceof DiffieHellmanGroup))
    return new DiffieHellmanGroup(name);
  this._handle = new binding.DiffieHellmanGroup(name);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getHashes"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>getHashes ()](#apidoc.element.mz.crypto.getHashes)
- description and source-code
```javascript
() => {
  if (result === undefined)
    result = fn();
  return result.slice();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.pbkdf2"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>pbkdf2 ()](#apidoc.element.mz.crypto.pbkdf2)
- description and source-code
```javascript
pbkdf2 = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.pbkdf2Sync"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>pbkdf2Sync (password, salt, iterations, keylen, digest)](#apidoc.element.mz.crypto.pbkdf2Sync)
- description and source-code
```javascript
pbkdf2Sync = function (password, salt, iterations, keylen, digest) {
  if (typeof digest === 'undefined') {
    digest = undefined;
    pbkdf2DeprecationWarning();
  }
  return pbkdf2(password, salt, iterations, keylen, digest);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.privateDecrypt"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>privateDecrypt (options, buffer)](#apidoc.element.mz.crypto.privateDecrypt)
- description and source-code
```javascript
privateDecrypt = function (options, buffer) {
  var key = options.key || options;
  var passphrase = options.passphrase || null;
  var padding = options.padding || defaultPadding;
  return method(toBuf(key), buffer, padding, passphrase);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.privateEncrypt"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>privateEncrypt (options, buffer)](#apidoc.element.mz.crypto.privateEncrypt)
- description and source-code
```javascript
privateEncrypt = function (options, buffer) {
  var key = options.key || options;
  var passphrase = options.passphrase || null;
  var padding = options.padding || defaultPadding;
  return method(toBuf(key), buffer, padding, passphrase);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.prng"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>prng ()](#apidoc.element.mz.crypto.prng)
- description and source-code
```javascript
function randomBytes() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.pseudoRandomBytes"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>pseudoRandomBytes ()](#apidoc.element.mz.crypto.pseudoRandomBytes)
- description and source-code
```javascript
function randomBytes() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.publicDecrypt"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>publicDecrypt (options, buffer)](#apidoc.element.mz.crypto.publicDecrypt)
- description and source-code
```javascript
publicDecrypt = function (options, buffer) {
  var key = options.key || options;
  var padding = options.padding || defaultPadding;
  var passphrase = options.passphrase || null;
  return method(toBuf(key), buffer, padding, passphrase);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.publicEncrypt"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>publicEncrypt (options, buffer)](#apidoc.element.mz.crypto.publicEncrypt)
- description and source-code
```javascript
publicEncrypt = function (options, buffer) {
  var key = options.key || options;
  var padding = options.padding || defaultPadding;
  var passphrase = options.passphrase || null;
  return method(toBuf(key), buffer, padding, passphrase);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.randomBytes"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>randomBytes ()](#apidoc.element.mz.crypto.randomBytes)
- description and source-code
```javascript
function randomBytes() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.rng"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>rng ()](#apidoc.element.mz.crypto.rng)
- description and source-code
```javascript
function randomBytes() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.setEngine"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>setEngine (id, flags)](#apidoc.element.mz.crypto.setEngine)
- description and source-code
```javascript
function setEngine(id, flags) {
  if (typeof id !== 'string')
    throw new TypeError('"id" argument should be a string');

  if (flags && typeof flags !== 'number')
    throw new TypeError('"flags" argument should be a number, if present');
  flags = flags >>> 0;

  // Use provided engine for everything by default
  if (flags === 0)
    flags = constants.ENGINE_METHOD_ALL;

  return binding.setEngine(id, flags);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.timingSafeEqual"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>timingSafeEqual ()](#apidoc.element.mz.crypto.timingSafeEqual)
- description and source-code
```javascript
function timingSafeEqual() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Certificate"></a>[module mz.crypto.Certificate](#apidoc.module.mz.crypto.Certificate)

#### <a name="apidoc.element.mz.crypto.Certificate.Certificate"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Certificate ()](#apidoc.element.mz.crypto.Certificate.Certificate)
- description and source-code
```javascript
function Certificate() {
  if (!(this instanceof Certificate))
    return new Certificate();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Certificate.prototype"></a>[module mz.crypto.Certificate.prototype](#apidoc.module.mz.crypto.Certificate.prototype)

#### <a name="apidoc.element.mz.crypto.Certificate.prototype.exportChallenge"></a>[function <span class="apidocSignatureSpan">mz.crypto.Certificate.prototype.</span>exportChallenge (object, encoding)](#apidoc.element.mz.crypto.Certificate.prototype.exportChallenge)
- description and source-code
```javascript
exportChallenge = function (object, encoding) {
  return binding.certExportChallenge(toBuf(object, encoding));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Certificate.prototype.exportPublicKey"></a>[function <span class="apidocSignatureSpan">mz.crypto.Certificate.prototype.</span>exportPublicKey (object, encoding)](#apidoc.element.mz.crypto.Certificate.prototype.exportPublicKey)
- description and source-code
```javascript
exportPublicKey = function (object, encoding) {
  return binding.certExportPublicKey(toBuf(object, encoding));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Certificate.prototype.verifySpkac"></a>[function <span class="apidocSignatureSpan">mz.crypto.Certificate.prototype.</span>verifySpkac (object)](#apidoc.element.mz.crypto.Certificate.prototype.verifySpkac)
- description and source-code
```javascript
verifySpkac = function (object) {
  return binding.certVerifySpkac(object);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Cipher"></a>[module mz.crypto.Cipher](#apidoc.module.mz.crypto.Cipher)

#### <a name="apidoc.element.mz.crypto.Cipher.Cipher"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Cipher (cipher, password, options)](#apidoc.element.mz.crypto.Cipher.Cipher)
- description and source-code
```javascript
function Cipher(cipher, password, options) {
  if (!(this instanceof Cipher))
    return new Cipher(cipher, password, options);
  this._handle = new binding.CipherBase(true);

  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher.super_"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipher.</span>super_ (options)](#apidoc.element.mz.crypto.Cipher.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Cipher.prototype"></a>[module mz.crypto.Cipher.prototype](#apidoc.module.mz.crypto.Cipher.prototype)

#### <a name="apidoc.element.mz.crypto.Cipher.prototype._flush"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Cipher.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  try {
    this.push(this._handle.final());
  } catch (e) {
    callback(e);
    return;
  }
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher.prototype._transform"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Cipher.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this.push(this._handle.update(chunk, encoding));
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher.prototype.final"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>final (outputEncoding)](#apidoc.element.mz.crypto.Cipher.prototype.final)
- description and source-code
```javascript
final = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher.prototype.getAuthTag"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>getAuthTag ()](#apidoc.element.mz.crypto.Cipher.prototype.getAuthTag)
- description and source-code
```javascript
getAuthTag = function () {
  return this._handle.getAuthTag();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher.prototype.setAAD"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>setAAD (aadbuf)](#apidoc.element.mz.crypto.Cipher.prototype.setAAD)
- description and source-code
```javascript
setAAD = function (aadbuf) {
  this._handle.setAAD(aadbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher.prototype.setAuthTag"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.mz.crypto.Cipher.prototype.setAuthTag)
- description and source-code
```javascript
setAuthTag = function (tagbuf) {
  this._handle.setAuthTag(tagbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher.prototype.setAutoPadding"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>setAutoPadding (ap)](#apidoc.element.mz.crypto.Cipher.prototype.setAutoPadding)
- description and source-code
```javascript
setAutoPadding = function (ap) {
  this._handle.setAutoPadding(ap);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipher.prototype.update"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipher.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.mz.crypto.Cipher.prototype.update)
- description and source-code
```javascript
update = function (data, inputEncoding, outputEncoding) {
  inputEncoding = inputEncoding || exports.DEFAULT_ENCODING;
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;

  var ret = this._handle.update(data, inputEncoding);

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.write(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Cipheriv"></a>[module mz.crypto.Cipheriv](#apidoc.module.mz.crypto.Cipheriv)

#### <a name="apidoc.element.mz.crypto.Cipheriv.Cipheriv"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Cipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Cipheriv.Cipheriv)
- description and source-code
```javascript
function Cipheriv(cipher, key, iv, options) {
  if (!(this instanceof Cipheriv))
    return new Cipheriv(cipher, key, iv, options);
  this._handle = new binding.CipherBase(true);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv.super_"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.</span>super_ (options)](#apidoc.element.mz.crypto.Cipheriv.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Cipheriv.prototype"></a>[module mz.crypto.Cipheriv.prototype](#apidoc.module.mz.crypto.Cipheriv.prototype)

#### <a name="apidoc.element.mz.crypto.Cipheriv.prototype._flush"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Cipheriv.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  try {
    this.push(this._handle.final());
  } catch (e) {
    callback(e);
    return;
  }
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv.prototype._transform"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Cipheriv.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this.push(this._handle.update(chunk, encoding));
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv.prototype.final"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>final (outputEncoding)](#apidoc.element.mz.crypto.Cipheriv.prototype.final)
- description and source-code
```javascript
final = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv.prototype.getAuthTag"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>getAuthTag ()](#apidoc.element.mz.crypto.Cipheriv.prototype.getAuthTag)
- description and source-code
```javascript
getAuthTag = function () {
  return this._handle.getAuthTag();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv.prototype.setAAD"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>setAAD (aadbuf)](#apidoc.element.mz.crypto.Cipheriv.prototype.setAAD)
- description and source-code
```javascript
setAAD = function (aadbuf) {
  this._handle.setAAD(aadbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv.prototype.setAuthTag"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.mz.crypto.Cipheriv.prototype.setAuthTag)
- description and source-code
```javascript
setAuthTag = function (tagbuf) {
  this._handle.setAuthTag(tagbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv.prototype.setAutoPadding"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>setAutoPadding (ap)](#apidoc.element.mz.crypto.Cipheriv.prototype.setAutoPadding)
- description and source-code
```javascript
setAutoPadding = function (ap) {
  this._handle.setAutoPadding(ap);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Cipheriv.prototype.update"></a>[function <span class="apidocSignatureSpan">mz.crypto.Cipheriv.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.mz.crypto.Cipheriv.prototype.update)
- description and source-code
```javascript
update = function (data, inputEncoding, outputEncoding) {
  inputEncoding = inputEncoding || exports.DEFAULT_ENCODING;
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;

  var ret = this._handle.update(data, inputEncoding);

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.write(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Decipher"></a>[module mz.crypto.Decipher](#apidoc.module.mz.crypto.Decipher)

#### <a name="apidoc.element.mz.crypto.Decipher.Decipher"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Decipher (cipher, password, options)](#apidoc.element.mz.crypto.Decipher.Decipher)
- description and source-code
```javascript
function Decipher(cipher, password, options) {
  if (!(this instanceof Decipher))
    return new Decipher(cipher, password, options);

  this._handle = new binding.CipherBase(false);
  this._handle.init(cipher, toBuf(password));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher.super_"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.</span>super_ (options)](#apidoc.element.mz.crypto.Decipher.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Decipher.prototype"></a>[module mz.crypto.Decipher.prototype](#apidoc.module.mz.crypto.Decipher.prototype)

#### <a name="apidoc.element.mz.crypto.Decipher.prototype._flush"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Decipher.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  try {
    this.push(this._handle.final());
  } catch (e) {
    callback(e);
    return;
  }
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher.prototype._transform"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Decipher.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this.push(this._handle.update(chunk, encoding));
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher.prototype.final"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>final (outputEncoding)](#apidoc.element.mz.crypto.Decipher.prototype.final)
- description and source-code
```javascript
final = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher.prototype.finaltol"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>finaltol (outputEncoding)](#apidoc.element.mz.crypto.Decipher.prototype.finaltol)
- description and source-code
```javascript
finaltol = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher.prototype.getAuthTag"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>getAuthTag ()](#apidoc.element.mz.crypto.Decipher.prototype.getAuthTag)
- description and source-code
```javascript
getAuthTag = function () {
  return this._handle.getAuthTag();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher.prototype.setAAD"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>setAAD (aadbuf)](#apidoc.element.mz.crypto.Decipher.prototype.setAAD)
- description and source-code
```javascript
setAAD = function (aadbuf) {
  this._handle.setAAD(aadbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher.prototype.setAuthTag"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.mz.crypto.Decipher.prototype.setAuthTag)
- description and source-code
```javascript
setAuthTag = function (tagbuf) {
  this._handle.setAuthTag(tagbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher.prototype.setAutoPadding"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>setAutoPadding (ap)](#apidoc.element.mz.crypto.Decipher.prototype.setAutoPadding)
- description and source-code
```javascript
setAutoPadding = function (ap) {
  this._handle.setAutoPadding(ap);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipher.prototype.update"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipher.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.mz.crypto.Decipher.prototype.update)
- description and source-code
```javascript
update = function (data, inputEncoding, outputEncoding) {
  inputEncoding = inputEncoding || exports.DEFAULT_ENCODING;
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;

  var ret = this._handle.update(data, inputEncoding);

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.write(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Decipheriv"></a>[module mz.crypto.Decipheriv](#apidoc.module.mz.crypto.Decipheriv)

#### <a name="apidoc.element.mz.crypto.Decipheriv.Decipheriv"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Decipheriv (cipher, key, iv, options)](#apidoc.element.mz.crypto.Decipheriv.Decipheriv)
- description and source-code
```javascript
function Decipheriv(cipher, key, iv, options) {
  if (!(this instanceof Decipheriv))
    return new Decipheriv(cipher, key, iv, options);

  this._handle = new binding.CipherBase(false);
  this._handle.initiv(cipher, toBuf(key), toBuf(iv));
  this._decoder = null;

  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv.super_"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.</span>super_ (options)](#apidoc.element.mz.crypto.Decipheriv.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Decipheriv.prototype"></a>[module mz.crypto.Decipheriv.prototype](#apidoc.module.mz.crypto.Decipheriv.prototype)

#### <a name="apidoc.element.mz.crypto.Decipheriv.prototype._flush"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Decipheriv.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  try {
    this.push(this._handle.final());
  } catch (e) {
    callback(e);
    return;
  }
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv.prototype._transform"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Decipheriv.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this.push(this._handle.update(chunk, encoding));
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv.prototype.final"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>final (outputEncoding)](#apidoc.element.mz.crypto.Decipheriv.prototype.final)
- description and source-code
```javascript
final = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv.prototype.finaltol"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>finaltol (outputEncoding)](#apidoc.element.mz.crypto.Decipheriv.prototype.finaltol)
- description and source-code
```javascript
finaltol = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  var ret = this._handle.final();

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.end(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv.prototype.getAuthTag"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>getAuthTag ()](#apidoc.element.mz.crypto.Decipheriv.prototype.getAuthTag)
- description and source-code
```javascript
getAuthTag = function () {
  return this._handle.getAuthTag();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv.prototype.setAAD"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>setAAD (aadbuf)](#apidoc.element.mz.crypto.Decipheriv.prototype.setAAD)
- description and source-code
```javascript
setAAD = function (aadbuf) {
  this._handle.setAAD(aadbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv.prototype.setAuthTag"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>setAuthTag (tagbuf)](#apidoc.element.mz.crypto.Decipheriv.prototype.setAuthTag)
- description and source-code
```javascript
setAuthTag = function (tagbuf) {
  this._handle.setAuthTag(tagbuf);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv.prototype.setAutoPadding"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>setAutoPadding (ap)](#apidoc.element.mz.crypto.Decipheriv.prototype.setAutoPadding)
- description and source-code
```javascript
setAutoPadding = function (ap) {
  this._handle.setAutoPadding(ap);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Decipheriv.prototype.update"></a>[function <span class="apidocSignatureSpan">mz.crypto.Decipheriv.prototype.</span>update (data, inputEncoding, outputEncoding)](#apidoc.element.mz.crypto.Decipheriv.prototype.update)
- description and source-code
```javascript
update = function (data, inputEncoding, outputEncoding) {
  inputEncoding = inputEncoding || exports.DEFAULT_ENCODING;
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;

  var ret = this._handle.update(data, inputEncoding);

  if (outputEncoding && outputEncoding !== 'buffer') {
    this._decoder = getDecoder(this._decoder, outputEncoding);
    ret = this._decoder.write(ret);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.DiffieHellman"></a>[module mz.crypto.DiffieHellman](#apidoc.module.mz.crypto.DiffieHellman)

#### <a name="apidoc.element.mz.crypto.DiffieHellman.DiffieHellman"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>DiffieHellman (sizeOrKey, keyEncoding, generator, genEncoding)](#apidoc.element.mz.crypto.DiffieHellman.DiffieHellman)
- description and source-code
```javascript
function DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding) {
  if (!(this instanceof DiffieHellman))
    return new DiffieHellman(sizeOrKey, keyEncoding, generator, genEncoding);

  if (!(sizeOrKey instanceof Buffer) &&
      typeof sizeOrKey !== 'number' &&
      typeof sizeOrKey !== 'string')
    throw new TypeError('First argument should be number, string or Buffer');

  if (keyEncoding) {
    if (typeof keyEncoding !== 'string' ||
        (!Buffer.isEncoding(keyEncoding) && keyEncoding !== 'buffer')) {
      genEncoding = generator;
      generator = keyEncoding;
      keyEncoding = false;
    }
  }

  keyEncoding = keyEncoding || exports.DEFAULT_ENCODING;
  genEncoding = genEncoding || exports.DEFAULT_ENCODING;

  if (typeof sizeOrKey !== 'number')
    sizeOrKey = toBuf(sizeOrKey, keyEncoding);

  if (!generator)
    generator = DH_GENERATOR;
  else if (typeof generator !== 'number')
    generator = toBuf(generator, genEncoding);

  this._handle = new binding.DiffieHellman(sizeOrKey, generator);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.DiffieHellman.prototype"></a>[module mz.crypto.DiffieHellman.prototype](#apidoc.module.mz.crypto.DiffieHellman.prototype)

#### <a name="apidoc.element.mz.crypto.DiffieHellman.prototype.computeSecret"></a>[function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>computeSecret (key, inEnc, outEnc)](#apidoc.element.mz.crypto.DiffieHellman.prototype.computeSecret)
- description and source-code
```javascript
function dhComputeSecret(key, inEnc, outEnc) {
  inEnc = inEnc || exports.DEFAULT_ENCODING;
  outEnc = outEnc || exports.DEFAULT_ENCODING;
  var ret = this._handle.computeSecret(toBuf(key, inEnc));
  if (outEnc && outEnc !== 'buffer')
    ret = ret.toString(outEnc);
  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellman.prototype.generateKeys"></a>[function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>generateKeys (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.generateKeys)
- description and source-code
```javascript
function dhGenerateKeys(encoding) {
  var keys = this._handle.generateKeys();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    keys = keys.toString(encoding);
  return keys;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellman.prototype.getGenerator"></a>[function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>getGenerator (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.getGenerator)
- description and source-code
```javascript
function dhGetGenerator(encoding) {
  var generator = this._handle.getGenerator();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    generator = generator.toString(encoding);
  return generator;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellman.prototype.getPrime"></a>[function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>getPrime (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.getPrime)
- description and source-code
```javascript
function dhGetPrime(encoding) {
  var prime = this._handle.getPrime();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    prime = prime.toString(encoding);
  return prime;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellman.prototype.getPrivateKey"></a>[function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>getPrivateKey (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.getPrivateKey)
- description and source-code
```javascript
function dhGetPrivateKey(encoding) {
  var key = this._handle.getPrivateKey();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    key = key.toString(encoding);
  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellman.prototype.getPublicKey"></a>[function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>getPublicKey (encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.getPublicKey)
- description and source-code
```javascript
function dhGetPublicKey(encoding) {
  var key = this._handle.getPublicKey();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    key = key.toString(encoding);
  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellman.prototype.setPrivateKey"></a>[function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>setPrivateKey (key, encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.setPrivateKey)
- description and source-code
```javascript
setPrivateKey = function (key, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.setPrivateKey(toBuf(key, encoding));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.DiffieHellman.prototype.setPublicKey"></a>[function <span class="apidocSignatureSpan">mz.crypto.DiffieHellman.prototype.</span>setPublicKey (key, encoding)](#apidoc.element.mz.crypto.DiffieHellman.prototype.setPublicKey)
- description and source-code
```javascript
setPublicKey = function (key, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.setPublicKey(toBuf(key, encoding));
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Hash"></a>[module mz.crypto.Hash](#apidoc.module.mz.crypto.Hash)

#### <a name="apidoc.element.mz.crypto.Hash.Hash"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Hash (algorithm, options)](#apidoc.element.mz.crypto.Hash.Hash)
- description and source-code
```javascript
function Hash(algorithm, options) {
  if (!(this instanceof Hash))
    return new Hash(algorithm, options);
  this._handle = new binding.Hash(algorithm);
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hash.super_"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hash.</span>super_ (options)](#apidoc.element.mz.crypto.Hash.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Hash.prototype"></a>[module mz.crypto.Hash.prototype](#apidoc.module.mz.crypto.Hash.prototype)

#### <a name="apidoc.element.mz.crypto.Hash.prototype._flush"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hash.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Hash.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  this.push(this._handle.digest());
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hash.prototype._transform"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hash.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Hash.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this._handle.update(chunk, encoding);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hash.prototype.digest"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hash.prototype.</span>digest (outputEncoding)](#apidoc.element.mz.crypto.Hash.prototype.digest)
- description and source-code
```javascript
digest = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  return this._handle.digest(outputEncoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hash.prototype.update"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hash.prototype.</span>update (data, encoding)](#apidoc.element.mz.crypto.Hash.prototype.update)
- description and source-code
```javascript
update = function (data, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.update(data, encoding);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Hmac"></a>[module mz.crypto.Hmac](#apidoc.module.mz.crypto.Hmac)

#### <a name="apidoc.element.mz.crypto.Hmac.Hmac"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Hmac (hmac, key, options)](#apidoc.element.mz.crypto.Hmac.Hmac)
- description and source-code
```javascript
function Hmac(hmac, key, options) {
  if (!(this instanceof Hmac))
    return new Hmac(hmac, key, options);
  this._handle = new binding.Hmac();
  this._handle.init(hmac, toBuf(key));
  LazyTransform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hmac.super_"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hmac.</span>super_ (options)](#apidoc.element.mz.crypto.Hmac.super_)
- description and source-code
```javascript
function LazyTransform(options) {
  this._options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Hmac.prototype"></a>[module mz.crypto.Hmac.prototype](#apidoc.module.mz.crypto.Hmac.prototype)

#### <a name="apidoc.element.mz.crypto.Hmac.prototype._flush"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hmac.prototype.</span>_flush (callback)](#apidoc.element.mz.crypto.Hmac.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  this.push(this._handle.digest());
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hmac.prototype._transform"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hmac.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.mz.crypto.Hmac.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
  this._handle.update(chunk, encoding);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hmac.prototype.digest"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hmac.prototype.</span>digest (outputEncoding)](#apidoc.element.mz.crypto.Hmac.prototype.digest)
- description and source-code
```javascript
digest = function (outputEncoding) {
  outputEncoding = outputEncoding || exports.DEFAULT_ENCODING;
  return this._handle.digest(outputEncoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Hmac.prototype.update"></a>[function <span class="apidocSignatureSpan">mz.crypto.Hmac.prototype.</span>update (data, encoding)](#apidoc.element.mz.crypto.Hmac.prototype.update)
- description and source-code
```javascript
update = function (data, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.update(data, encoding);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Sign"></a>[module mz.crypto.Sign](#apidoc.module.mz.crypto.Sign)

#### <a name="apidoc.element.mz.crypto.Sign.Sign"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Sign (algorithm, options)](#apidoc.element.mz.crypto.Sign.Sign)
- description and source-code
```javascript
function Sign(algorithm, options) {
  if (!(this instanceof Sign))
    return new Sign(algorithm, options);
  this._handle = new binding.Sign();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Sign.super_"></a>[function <span class="apidocSignatureSpan">mz.crypto.Sign.</span>super_ (options)](#apidoc.element.mz.crypto.Sign.super_)
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



# <a name="apidoc.module.mz.crypto.Sign.prototype"></a>[module mz.crypto.Sign.prototype](#apidoc.module.mz.crypto.Sign.prototype)

#### <a name="apidoc.element.mz.crypto.Sign.prototype._write"></a>[function <span class="apidocSignatureSpan">mz.crypto.Sign.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.mz.crypto.Sign.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, callback) {
  this._handle.update(chunk, encoding);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Sign.prototype.sign"></a>[function <span class="apidocSignatureSpan">mz.crypto.Sign.prototype.</span>sign (options, encoding)](#apidoc.element.mz.crypto.Sign.prototype.sign)
- description and source-code
```javascript
sign = function (options, encoding) {
  if (!options)
    throw new Error('No key provided to sign');

  var key = options.key || options;
  var passphrase = options.passphrase || null;
  var ret = this._handle.sign(toBuf(key), null, passphrase);

  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    ret = ret.toString(encoding);

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Sign.prototype.update"></a>[function <span class="apidocSignatureSpan">mz.crypto.Sign.prototype.</span>update (data, encoding)](#apidoc.element.mz.crypto.Sign.prototype.update)
- description and source-code
```javascript
update = function (data, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.update(data, encoding);
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.Verify"></a>[module mz.crypto.Verify](#apidoc.module.mz.crypto.Verify)

#### <a name="apidoc.element.mz.crypto.Verify.Verify"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>Verify (algorithm, options)](#apidoc.element.mz.crypto.Verify.Verify)
- description and source-code
```javascript
function Verify(algorithm, options) {
  if (!(this instanceof Verify))
    return new Verify(algorithm, options);

  this._handle = new binding.Verify();
  this._handle.init(algorithm);

  stream.Writable.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Verify.super_"></a>[function <span class="apidocSignatureSpan">mz.crypto.Verify.</span>super_ (options)](#apidoc.element.mz.crypto.Verify.super_)
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



# <a name="apidoc.module.mz.crypto.Verify.prototype"></a>[module mz.crypto.Verify.prototype](#apidoc.module.mz.crypto.Verify.prototype)

#### <a name="apidoc.element.mz.crypto.Verify.prototype._write"></a>[function <span class="apidocSignatureSpan">mz.crypto.Verify.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.mz.crypto.Verify.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, callback) {
  this._handle.update(chunk, encoding);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Verify.prototype.update"></a>[function <span class="apidocSignatureSpan">mz.crypto.Verify.prototype.</span>update (data, encoding)](#apidoc.element.mz.crypto.Verify.prototype.update)
- description and source-code
```javascript
update = function (data, encoding) {
  encoding = encoding || exports.DEFAULT_ENCODING;
  this._handle.update(data, encoding);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.Verify.prototype.verify"></a>[function <span class="apidocSignatureSpan">mz.crypto.Verify.prototype.</span>verify (object, signature, sigEncoding)](#apidoc.element.mz.crypto.Verify.prototype.verify)
- description and source-code
```javascript
verify = function (object, signature, sigEncoding) {
  sigEncoding = sigEncoding || exports.DEFAULT_ENCODING;
  return this._handle.verify(toBuf(object), toBuf(signature, sigEncoding));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.getDiffieHellman"></a>[module mz.crypto.getDiffieHellman](#apidoc.module.mz.crypto.getDiffieHellman)

#### <a name="apidoc.element.mz.crypto.getDiffieHellman.getDiffieHellman"></a>[function <span class="apidocSignatureSpan">mz.crypto.</span>getDiffieHellman (name)](#apidoc.element.mz.crypto.getDiffieHellman.getDiffieHellman)
- description and source-code
```javascript
function DiffieHellmanGroup(name) {
  if (!(this instanceof DiffieHellmanGroup))
    return new DiffieHellmanGroup(name);
  this._handle = new binding.DiffieHellmanGroup(name);
  Object.defineProperty(this, 'verifyError', {
    enumerable: true,
    value: this._handle.verifyError,
    writable: false
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.crypto.getDiffieHellman.prototype"></a>[module mz.crypto.getDiffieHellman.prototype](#apidoc.module.mz.crypto.getDiffieHellman.prototype)

#### <a name="apidoc.element.mz.crypto.getDiffieHellman.prototype.computeSecret"></a>[function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>computeSecret (key, inEnc, outEnc)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.computeSecret)
- description and source-code
```javascript
function dhComputeSecret(key, inEnc, outEnc) {
  inEnc = inEnc || exports.DEFAULT_ENCODING;
  outEnc = outEnc || exports.DEFAULT_ENCODING;
  var ret = this._handle.computeSecret(toBuf(key, inEnc));
  if (outEnc && outEnc !== 'buffer')
    ret = ret.toString(outEnc);
  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getDiffieHellman.prototype.generateKeys"></a>[function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>generateKeys (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.generateKeys)
- description and source-code
```javascript
function dhGenerateKeys(encoding) {
  var keys = this._handle.generateKeys();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    keys = keys.toString(encoding);
  return keys;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getDiffieHellman.prototype.getGenerator"></a>[function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>getGenerator (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.getGenerator)
- description and source-code
```javascript
function dhGetGenerator(encoding) {
  var generator = this._handle.getGenerator();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    generator = generator.toString(encoding);
  return generator;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getDiffieHellman.prototype.getPrime"></a>[function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>getPrime (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.getPrime)
- description and source-code
```javascript
function dhGetPrime(encoding) {
  var prime = this._handle.getPrime();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    prime = prime.toString(encoding);
  return prime;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getDiffieHellman.prototype.getPrivateKey"></a>[function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>getPrivateKey (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.getPrivateKey)
- description and source-code
```javascript
function dhGetPrivateKey(encoding) {
  var key = this._handle.getPrivateKey();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    key = key.toString(encoding);
  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.crypto.getDiffieHellman.prototype.getPublicKey"></a>[function <span class="apidocSignatureSpan">mz.crypto.getDiffieHellman.prototype.</span>getPublicKey (encoding)](#apidoc.element.mz.crypto.getDiffieHellman.prototype.getPublicKey)
- description and source-code
```javascript
function dhGetPublicKey(encoding) {
  var key = this._handle.getPublicKey();
  encoding = encoding || exports.DEFAULT_ENCODING;
  if (encoding && encoding !== 'buffer')
    key = key.toString(encoding);
  return key;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.dns"></a>[module mz.dns](#apidoc.module.mz.dns)

#### <a name="apidoc.element.mz.dns.getServers"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>getServers ()](#apidoc.element.mz.dns.getServers)
- description and source-code
```javascript
getServers = function () {
  return cares.getServers();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.lookup"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>lookup ()](#apidoc.element.mz.dns.lookup)
- description and source-code
```javascript
function lookup() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.lookupService"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>lookupService (host, port, callback)](#apidoc.element.mz.dns.lookupService)
- description and source-code
```javascript
lookupService = function (host, port, callback) {
  if (arguments.length !== 3)
    throw new Error('Invalid arguments');

  if (isIP(host) === 0)
    throw new TypeError('"host" argument needs to be a valid IP address');

  if (!isLegalPort(port))
    throw new TypeError('"port" should be >= 0 and < 65536, got "${port}"');

  if (typeof callback !== 'function')
    throw new TypeError('"callback" argument must be a function');

  port = +port;
  callback = makeAsync(callback);

  var req = new GetNameInfoReqWrap();
  req.callback = callback;
  req.host = host;
  req.port = port;
  req.oncomplete = onlookupservice;

  var err = cares.getnameinfo(req, host, port);
  if (err) throw errnoException(err, 'getnameinfo', host);

  callback.immediately = true;
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolve"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolve ()](#apidoc.element.mz.dns.resolve)
- description and source-code
```javascript
resolve = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolve4"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolve4 ()](#apidoc.element.mz.dns.resolve4)
- description and source-code
```javascript
function query() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolve6"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolve6 ()](#apidoc.element.mz.dns.resolve6)
- description and source-code
```javascript
function query() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolveCname"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolveCname ()](#apidoc.element.mz.dns.resolveCname)
- description and source-code
```javascript
function query() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolveMx"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolveMx ()](#apidoc.element.mz.dns.resolveMx)
- description and source-code
```javascript
function query() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolveNaptr"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolveNaptr (name, callback)](#apidoc.element.mz.dns.resolveNaptr)
- description and source-code
```javascript
function query(name, callback) {
  if (typeof name !== 'string') {
    throw new Error('"name" argument must be a string');
  } else if (typeof callback !== 'function') {
    throw new Error('"callback" argument must be a function');
  }

  callback = makeAsync(callback);
  var req = new QueryReqWrap();
  req.bindingName = bindingName;
  req.callback = callback;
  req.hostname = name;
  req.oncomplete = onresolve;
  var err = binding(req, name);
  if (err) throw errnoException(err, bindingName);
  callback.immediately = true;
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolveNs"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolveNs ()](#apidoc.element.mz.dns.resolveNs)
- description and source-code
```javascript
function query() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolvePtr"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolvePtr (name, callback)](#apidoc.element.mz.dns.resolvePtr)
- description and source-code
```javascript
function query(name, callback) {
  if (typeof name !== 'string') {
    throw new Error('"name" argument must be a string');
  } else if (typeof callback !== 'function') {
    throw new Error('"callback" argument must be a function');
  }

  callback = makeAsync(callback);
  var req = new QueryReqWrap();
  req.bindingName = bindingName;
  req.callback = callback;
  req.hostname = name;
  req.oncomplete = onresolve;
  var err = binding(req, name);
  if (err) throw errnoException(err, bindingName);
  callback.immediately = true;
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolveSoa"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolveSoa (name, callback)](#apidoc.element.mz.dns.resolveSoa)
- description and source-code
```javascript
function query(name, callback) {
  if (typeof name !== 'string') {
    throw new Error('"name" argument must be a string');
  } else if (typeof callback !== 'function') {
    throw new Error('"callback" argument must be a function');
  }

  callback = makeAsync(callback);
  var req = new QueryReqWrap();
  req.bindingName = bindingName;
  req.callback = callback;
  req.hostname = name;
  req.oncomplete = onresolve;
  var err = binding(req, name);
  if (err) throw errnoException(err, bindingName);
  callback.immediately = true;
  return req;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolveSrv"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolveSrv ()](#apidoc.element.mz.dns.resolveSrv)
- description and source-code
```javascript
function query() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.resolveTxt"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>resolveTxt ()](#apidoc.element.mz.dns.resolveTxt)
- description and source-code
```javascript
function query() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.reverse"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>reverse ()](#apidoc.element.mz.dns.reverse)
- description and source-code
```javascript
function query() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.dns.setServers"></a>[function <span class="apidocSignatureSpan">mz.dns.</span>setServers (servers)](#apidoc.element.mz.dns.setServers)
- description and source-code
```javascript
setServers = function (servers) {
  // cache the original servers because in the event of an error setting the
  // servers cares won't have any servers available for resolution
  const orig = cares.getServers();
  const newSet = [];

  servers.forEach((serv) => {
    var ipVersion = isIP(serv);
    if (ipVersion !== 0)
      return newSet.push([ipVersion, serv]);

    const match = serv.match(/\[(.*)\](?::\d+)?/);
    // we have an IPv6 in brackets
    if (match) {
      ipVersion = isIP(match[1]);
      if (ipVersion !== 0)
        return newSet.push([ipVersion, match[1]]);
    }

    const s = serv.split(/:\d+$/)[0];
    ipVersion = isIP(s);

    if (ipVersion !== 0)
      return newSet.push([ipVersion, s]);

    throw new Error('IP address is not properly formatted: ${serv}');
  });

  const errorNumber = cares.setServers(newSet);

  if (errorNumber !== 0) {
    // reset the servers to the old servers, because ares probably unset them
    cares.setServers(orig.join(','));

    var err = cares.strerror(errorNumber);
    throw new Error('c-ares failed to set servers: "${err}" [${servers}]');
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.fs"></a>[module mz.fs](#apidoc.module.mz.fs)

#### <a name="apidoc.element.mz.fs.FileReadStream"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>FileReadStream (path, options)](#apidoc.element.mz.fs.FileReadStream)
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

#### <a name="apidoc.element.mz.fs.FileWriteStream"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>FileWriteStream (path, options)](#apidoc.element.mz.fs.FileWriteStream)
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

#### <a name="apidoc.element.mz.fs.ReadStream"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>ReadStream (path, options)](#apidoc.element.mz.fs.ReadStream)
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

#### <a name="apidoc.element.mz.fs.Stats"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.mz.fs.Stats)
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

#### <a name="apidoc.element.mz.fs.WriteStream"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>WriteStream (path, options)](#apidoc.element.mz.fs.WriteStream)
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

#### <a name="apidoc.element.mz.fs._toUnixTimestamp"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>_toUnixTimestamp (time)](#apidoc.element.mz.fs._toUnixTimestamp)
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

#### <a name="apidoc.element.mz.fs.access"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>access ()](#apidoc.element.mz.fs.access)
- description and source-code
```javascript
access = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.accessSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>accessSync (path, mode)](#apidoc.element.mz.fs.accessSync)
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

#### <a name="apidoc.element.mz.fs.appendFile"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>appendFile ()](#apidoc.element.mz.fs.appendFile)
- description and source-code
```javascript
appendFile = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.appendFileSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>appendFileSync (path, data, options)](#apidoc.element.mz.fs.appendFileSync)
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

#### <a name="apidoc.element.mz.fs.chmod"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>chmod ()](#apidoc.element.mz.fs.chmod)
- description and source-code
```javascript
chmod = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.chmodSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>chmodSync (path, mode)](#apidoc.element.mz.fs.chmodSync)
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

#### <a name="apidoc.element.mz.fs.chown"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>chown ()](#apidoc.element.mz.fs.chown)
- description and source-code
```javascript
chown = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.chownSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>chownSync (path, uid, gid)](#apidoc.element.mz.fs.chownSync)
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

#### <a name="apidoc.element.mz.fs.close"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>close ()](#apidoc.element.mz.fs.close)
- description and source-code
```javascript
close = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.closeSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>closeSync (fd)](#apidoc.element.mz.fs.closeSync)
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

#### <a name="apidoc.element.mz.fs.createReadStream"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>createReadStream (path, options)](#apidoc.element.mz.fs.createReadStream)
- description and source-code
```javascript
createReadStream = function (path, options) {
  return new ReadStream(path, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.createWriteStream"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>createWriteStream (path, options)](#apidoc.element.mz.fs.createWriteStream)
- description and source-code
```javascript
createWriteStream = function (path, options) {
  return new WriteStream(path, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.exists"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>exists (filename, callback)](#apidoc.element.mz.fs.exists)
- description and source-code
```javascript
exists = function (filename, callback) {
  // callback
  if (typeof callback === 'function') {
    return fs.stat(filename, function (err) {
      callback(null, !err);
    })
  }
  // or promise
  return new Promise(function (resolve) {
    fs.stat(filename, function (err) {
      resolve(!err)
    })
  })
}
```
- example usage
```shell
...
'''

Then prefix the relevant 'require()'s with 'mz/':

'''js
var fs = require('mz/fs')

fs.exists(__filename).then(function (exists) {
  if (exists) // do something
})
'''

With ES2017, this will allow you to use async functions cleanly with node's core API:

'''js
...
```

#### <a name="apidoc.element.mz.fs.existsSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>existsSync (path)](#apidoc.element.mz.fs.existsSync)
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

#### <a name="apidoc.element.mz.fs.fchmod"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fchmod ()](#apidoc.element.mz.fs.fchmod)
- description and source-code
```javascript
fchmod = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.fchmodSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fchmodSync (fd, mode)](#apidoc.element.mz.fs.fchmodSync)
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

#### <a name="apidoc.element.mz.fs.fchown"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fchown ()](#apidoc.element.mz.fs.fchown)
- description and source-code
```javascript
fchown = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.fchownSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fchownSync (fd, uid, gid)](#apidoc.element.mz.fs.fchownSync)
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

#### <a name="apidoc.element.mz.fs.fdatasync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fdatasync ()](#apidoc.element.mz.fs.fdatasync)
- description and source-code
```javascript
fdatasync = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.fdatasyncSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fdatasyncSync (fd)](#apidoc.element.mz.fs.fdatasyncSync)
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

#### <a name="apidoc.element.mz.fs.fstat"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fstat ()](#apidoc.element.mz.fs.fstat)
- description and source-code
```javascript
fstat = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.fstatSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fstatSync (fd)](#apidoc.element.mz.fs.fstatSync)
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

#### <a name="apidoc.element.mz.fs.fsync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fsync ()](#apidoc.element.mz.fs.fsync)
- description and source-code
```javascript
fsync = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.fsyncSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>fsyncSync (fd)](#apidoc.element.mz.fs.fsyncSync)
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

#### <a name="apidoc.element.mz.fs.ftruncate"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>ftruncate ()](#apidoc.element.mz.fs.ftruncate)
- description and source-code
```javascript
ftruncate = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.ftruncateSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>ftruncateSync (fd, len)](#apidoc.element.mz.fs.ftruncateSync)
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

#### <a name="apidoc.element.mz.fs.futimes"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>futimes ()](#apidoc.element.mz.fs.futimes)
- description and source-code
```javascript
futimes = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.futimesSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>futimesSync (fd, atime, mtime)](#apidoc.element.mz.fs.futimesSync)
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

#### <a name="apidoc.element.mz.fs.link"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>link ()](#apidoc.element.mz.fs.link)
- description and source-code
```javascript
link = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.linkSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>linkSync (existingPath, newPath)](#apidoc.element.mz.fs.linkSync)
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

#### <a name="apidoc.element.mz.fs.lstat"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>lstat ()](#apidoc.element.mz.fs.lstat)
- description and source-code
```javascript
lstat = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.lstatSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>lstatSync (path)](#apidoc.element.mz.fs.lstatSync)
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

#### <a name="apidoc.element.mz.fs.mkdir"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>mkdir ()](#apidoc.element.mz.fs.mkdir)
- description and source-code
```javascript
mkdir = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.mkdirSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>mkdirSync (path, mode)](#apidoc.element.mz.fs.mkdirSync)
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

#### <a name="apidoc.element.mz.fs.mkdtemp"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>mkdtemp ()](#apidoc.element.mz.fs.mkdtemp)
- description and source-code
```javascript
mkdtemp = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.mkdtempSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>mkdtempSync (prefix, options)](#apidoc.element.mz.fs.mkdtempSync)
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

#### <a name="apidoc.element.mz.fs.open"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>open ()](#apidoc.element.mz.fs.open)
- description and source-code
```javascript
open = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.openSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>openSync (path, flags, mode)](#apidoc.element.mz.fs.openSync)
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

#### <a name="apidoc.element.mz.fs.read"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>read ()](#apidoc.element.mz.fs.read)
- description and source-code
```javascript
read = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.readFile"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>readFile ()](#apidoc.element.mz.fs.readFile)
- description and source-code
```javascript
readFile = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.readFileSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>readFileSync (path, options)](#apidoc.element.mz.fs.readFileSync)
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

#### <a name="apidoc.element.mz.fs.readSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>readSync (fd, buffer, offset, length, position)](#apidoc.element.mz.fs.readSync)
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

#### <a name="apidoc.element.mz.fs.readdir"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>readdir ()](#apidoc.element.mz.fs.readdir)
- description and source-code
```javascript
readdir = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.readdirSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>readdirSync (path, options)](#apidoc.element.mz.fs.readdirSync)
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

#### <a name="apidoc.element.mz.fs.readlink"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>readlink ()](#apidoc.element.mz.fs.readlink)
- description and source-code
```javascript
readlink = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.readlinkSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>readlinkSync (path, options)](#apidoc.element.mz.fs.readlinkSync)
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

#### <a name="apidoc.element.mz.fs.realpath"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>realpath ()](#apidoc.element.mz.fs.realpath)
- description and source-code
```javascript
function realpath() {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.realpathSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>realpathSync (p, options)](#apidoc.element.mz.fs.realpathSync)
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

#### <a name="apidoc.element.mz.fs.rename"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>rename ()](#apidoc.element.mz.fs.rename)
- description and source-code
```javascript
rename = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.renameSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>renameSync (oldPath, newPath)](#apidoc.element.mz.fs.renameSync)
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

#### <a name="apidoc.element.mz.fs.rmdir"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>rmdir ()](#apidoc.element.mz.fs.rmdir)
- description and source-code
```javascript
rmdir = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.rmdirSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>rmdirSync (path)](#apidoc.element.mz.fs.rmdirSync)
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

#### <a name="apidoc.element.mz.fs.stat"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>stat ()](#apidoc.element.mz.fs.stat)
- description and source-code
```javascript
stat = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.statSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>statSync (path)](#apidoc.element.mz.fs.statSync)
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

#### <a name="apidoc.element.mz.fs.symlink"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>symlink ()](#apidoc.element.mz.fs.symlink)
- description and source-code
```javascript
symlink = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.symlinkSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>symlinkSync (target, path, type)](#apidoc.element.mz.fs.symlinkSync)
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

#### <a name="apidoc.element.mz.fs.truncate"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>truncate ()](#apidoc.element.mz.fs.truncate)
- description and source-code
```javascript
truncate = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.truncateSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>truncateSync (path, len)](#apidoc.element.mz.fs.truncateSync)
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

#### <a name="apidoc.element.mz.fs.unlink"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>unlink ()](#apidoc.element.mz.fs.unlink)
- description and source-code
```javascript
unlink = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.unlinkSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>unlinkSync (path)](#apidoc.element.mz.fs.unlinkSync)
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

#### <a name="apidoc.element.mz.fs.unwatchFile"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>unwatchFile (filename, listener)](#apidoc.element.mz.fs.unwatchFile)
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

#### <a name="apidoc.element.mz.fs.utimes"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>utimes ()](#apidoc.element.mz.fs.utimes)
- description and source-code
```javascript
utimes = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.utimesSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>utimesSync (path, atime, mtime)](#apidoc.element.mz.fs.utimesSync)
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

#### <a name="apidoc.element.mz.fs.watch"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>watch (filename, options, listener)](#apidoc.element.mz.fs.watch)
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

#### <a name="apidoc.element.mz.fs.watchFile"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>watchFile (filename, options, listener)](#apidoc.element.mz.fs.watchFile)
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

#### <a name="apidoc.element.mz.fs.write"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>write ()](#apidoc.element.mz.fs.write)
- description and source-code
```javascript
write = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.writeFile"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>writeFile ()](#apidoc.element.mz.fs.writeFile)
- description and source-code
```javascript
writeFile = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.fs.writeFileSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>writeFileSync (path, data, options)](#apidoc.element.mz.fs.writeFileSync)
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

#### <a name="apidoc.element.mz.fs.writeSync"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>writeSync (fd, buffer, offset, length, position)](#apidoc.element.mz.fs.writeSync)
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



# <a name="apidoc.module.mz.fs.ReadStream"></a>[module mz.fs.ReadStream](#apidoc.module.mz.fs.ReadStream)

#### <a name="apidoc.element.mz.fs.ReadStream.ReadStream"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>ReadStream (path, options)](#apidoc.element.mz.fs.ReadStream.ReadStream)
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

#### <a name="apidoc.element.mz.fs.ReadStream.super_"></a>[function <span class="apidocSignatureSpan">mz.fs.ReadStream.</span>super_ (options)](#apidoc.element.mz.fs.ReadStream.super_)
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



# <a name="apidoc.module.mz.fs.ReadStream.prototype"></a>[module mz.fs.ReadStream.prototype](#apidoc.module.mz.fs.ReadStream.prototype)

#### <a name="apidoc.element.mz.fs.ReadStream.prototype._read"></a>[function <span class="apidocSignatureSpan">mz.fs.ReadStream.prototype.</span>_read (n)](#apidoc.element.mz.fs.ReadStream.prototype._read)
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

#### <a name="apidoc.element.mz.fs.ReadStream.prototype.close"></a>[function <span class="apidocSignatureSpan">mz.fs.ReadStream.prototype.</span>close (cb)](#apidoc.element.mz.fs.ReadStream.prototype.close)
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

#### <a name="apidoc.element.mz.fs.ReadStream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">mz.fs.ReadStream.prototype.</span>destroy ()](#apidoc.element.mz.fs.ReadStream.prototype.destroy)
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

#### <a name="apidoc.element.mz.fs.ReadStream.prototype.open"></a>[function <span class="apidocSignatureSpan">mz.fs.ReadStream.prototype.</span>open ()](#apidoc.element.mz.fs.ReadStream.prototype.open)
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



# <a name="apidoc.module.mz.fs.Stats"></a>[module mz.fs.Stats](#apidoc.module.mz.fs.Stats)

#### <a name="apidoc.element.mz.fs.Stats.Stats"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>Stats ( dev, mode, nlink, uid, gid, rdev, blksize, ino, size, blocks, atim_msec, mtim_msec, ctim_msec, birthtim_msec)](#apidoc.element.mz.fs.Stats.Stats)
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



# <a name="apidoc.module.mz.fs.Stats.prototype"></a>[module mz.fs.Stats.prototype](#apidoc.module.mz.fs.Stats.prototype)

#### <a name="apidoc.element.mz.fs.Stats.prototype._checkModeProperty"></a>[function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>_checkModeProperty (property)](#apidoc.element.mz.fs.Stats.prototype._checkModeProperty)
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

#### <a name="apidoc.element.mz.fs.Stats.prototype.isBlockDevice"></a>[function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isBlockDevice ()](#apidoc.element.mz.fs.Stats.prototype.isBlockDevice)
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

#### <a name="apidoc.element.mz.fs.Stats.prototype.isCharacterDevice"></a>[function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isCharacterDevice ()](#apidoc.element.mz.fs.Stats.prototype.isCharacterDevice)
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

#### <a name="apidoc.element.mz.fs.Stats.prototype.isDirectory"></a>[function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isDirectory ()](#apidoc.element.mz.fs.Stats.prototype.isDirectory)
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

#### <a name="apidoc.element.mz.fs.Stats.prototype.isFIFO"></a>[function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isFIFO ()](#apidoc.element.mz.fs.Stats.prototype.isFIFO)
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

#### <a name="apidoc.element.mz.fs.Stats.prototype.isFile"></a>[function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isFile ()](#apidoc.element.mz.fs.Stats.prototype.isFile)
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

#### <a name="apidoc.element.mz.fs.Stats.prototype.isSocket"></a>[function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isSocket ()](#apidoc.element.mz.fs.Stats.prototype.isSocket)
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

#### <a name="apidoc.element.mz.fs.Stats.prototype.isSymbolicLink"></a>[function <span class="apidocSignatureSpan">mz.fs.Stats.prototype.</span>isSymbolicLink ()](#apidoc.element.mz.fs.Stats.prototype.isSymbolicLink)
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



# <a name="apidoc.module.mz.fs.WriteStream"></a>[module mz.fs.WriteStream](#apidoc.module.mz.fs.WriteStream)

#### <a name="apidoc.element.mz.fs.WriteStream.WriteStream"></a>[function <span class="apidocSignatureSpan">mz.fs.</span>WriteStream (path, options)](#apidoc.element.mz.fs.WriteStream.WriteStream)
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

#### <a name="apidoc.element.mz.fs.WriteStream.super_"></a>[function <span class="apidocSignatureSpan">mz.fs.WriteStream.</span>super_ (options)](#apidoc.element.mz.fs.WriteStream.super_)
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



# <a name="apidoc.module.mz.fs.WriteStream.prototype"></a>[module mz.fs.WriteStream.prototype](#apidoc.module.mz.fs.WriteStream.prototype)

#### <a name="apidoc.element.mz.fs.WriteStream.prototype._write"></a>[function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>_write (data, encoding, cb)](#apidoc.element.mz.fs.WriteStream.prototype._write)
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

#### <a name="apidoc.element.mz.fs.WriteStream.prototype._writev"></a>[function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>_writev (data, cb)](#apidoc.element.mz.fs.WriteStream.prototype._writev)
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

#### <a name="apidoc.element.mz.fs.WriteStream.prototype.close"></a>[function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>close (cb)](#apidoc.element.mz.fs.WriteStream.prototype.close)
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

#### <a name="apidoc.element.mz.fs.WriteStream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>destroy ()](#apidoc.element.mz.fs.WriteStream.prototype.destroy)
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

#### <a name="apidoc.element.mz.fs.WriteStream.prototype.destroySoon"></a>[function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>destroySoon (chunk, encoding, cb)](#apidoc.element.mz.fs.WriteStream.prototype.destroySoon)
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

#### <a name="apidoc.element.mz.fs.WriteStream.prototype.open"></a>[function <span class="apidocSignatureSpan">mz.fs.WriteStream.prototype.</span>open ()](#apidoc.element.mz.fs.WriteStream.prototype.open)
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



# <a name="apidoc.module.mz.readline"></a>[module mz.readline](#apidoc.module.mz.readline)

#### <a name="apidoc.element.mz.readline.Interface"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>Interface (input, output, completer, terminal)](#apidoc.element.mz.readline.Interface)
- description and source-code
```javascript
function InterfaceAsPromised(input, output, completer, terminal) {
  if (arguments.length === 1) {
    var options = input

    if (typeof options.completer === 'function') {
      options = objectAssign({}, options, {
        completer: wrapCompleter(options.completer)
      })
    }

    Interface.call(this, options)
  } else {
    if (typeof completer === 'function') {
      completer = wrapCompleter(completer)
    }

    Interface.call(this, input, output, completer, terminal)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.clearLine"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>clearLine (stream, dir)](#apidoc.element.mz.readline.clearLine)
- description and source-code
```javascript
function clearLine(stream, dir) {
  if (stream === null || stream === undefined)
    return;

  if (dir < 0) {
    // to the beginning
    stream.write('\x1b[1K');
  } else if (dir > 0) {
    // to the end
    stream.write('\x1b[0K');
  } else {
    // entire line
    stream.write('\x1b[2K');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.clearScreenDown"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>clearScreenDown (stream)](#apidoc.element.mz.readline.clearScreenDown)
- description and source-code
```javascript
function clearScreenDown(stream) {
  if (stream === null || stream === undefined)
    return;

  stream.write('\x1b[0J');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.codePointAt"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>codePointAt ()](#apidoc.element.mz.readline.codePointAt)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.createInterface"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>createInterface (input, output, completer, terminal)](#apidoc.element.mz.readline.createInterface)
- description and source-code
```javascript
createInterface = function (input, output, completer, terminal) {
  if (arguments.length === 1) {
    return new InterfaceAsPromised(input)
  }

  return new InterfaceAsPromised(input, output, completer, terminal)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.cursorTo"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>cursorTo (stream, x, y)](#apidoc.element.mz.readline.cursorTo)
- description and source-code
```javascript
function cursorTo(stream, x, y) {
  if (stream === null || stream === undefined)
    return;

  if (typeof x !== 'number' && typeof y !== 'number')
    return;

  if (typeof x !== 'number')
    throw new Error('Can\'t set cursor row without also setting it\'s column');

  if (typeof y !== 'number') {
    stream.write('\x1b[' + (x + 1) + 'G');
  } else {
    stream.write('\x1b[' + (y + 1) + ';' + (x + 1) + 'H');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.emitKeypressEvents"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>emitKeypressEvents (stream, iface)](#apidoc.element.mz.readline.emitKeypressEvents)
- description and source-code
```javascript
function emitKeypressEvents(stream, iface) {
  if (stream[KEYPRESS_DECODER]) return;
  var StringDecoder = require('string_decoder').StringDecoder; // lazy load
  stream[KEYPRESS_DECODER] = new StringDecoder('utf8');

  stream[ESCAPE_DECODER] = emitKeys(stream);
  stream[ESCAPE_DECODER].next();

  const escapeCodeTimeout = () => stream[ESCAPE_DECODER].next('');
  let timeoutId;

  function onData(b) {
    if (stream.listenerCount('keypress') > 0) {
      var r = stream[KEYPRESS_DECODER].write(b);
      if (r) {
        clearTimeout(timeoutId);

        if (iface) {
          iface._sawKeyPress = r.length === 1;
        }

        for (var i = 0; i < r.length; i++) {
          if (r[i] === '\t' && typeof r[i + 1] === 'string' && iface) {
            iface.isCompletionEnabled = false;
          }

          try {
            stream[ESCAPE_DECODER].next(r[i]);
            // Escape letter at the tail position
            if (r[i] === '\x1b' && i + 1 === r.length) {
              timeoutId = setTimeout(escapeCodeTimeout, ESCAPE_CODE_TIMEOUT);
            }
          } catch (err) {
            // if the generator throws (it could happen in the 'keypress'
            // event), we need to restart it.
            stream[ESCAPE_DECODER] = emitKeys(stream);
            stream[ESCAPE_DECODER].next();
            throw err;
          } finally {
            if (iface) {
              iface.isCompletionEnabled = true;
            }
          }
        }
      }
    } else {
      // Nobody's watching anyway
      stream.removeListener('data', onData);
      stream.on('newListener', onNewListener);
    }
  }

  function onNewListener(event) {
    if (event === 'keypress') {
      stream.on('data', onData);
      stream.removeListener('newListener', onNewListener);
    }
  }

  if (stream.listenerCount('keypress') > 0) {
    stream.on('data', onData);
  } else {
    stream.on('newListener', onNewListener);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.getStringWidth"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>getStringWidth ()](#apidoc.element.mz.readline.getStringWidth)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.isFullWidthCodePoint"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>isFullWidthCodePoint ()](#apidoc.element.mz.readline.isFullWidthCodePoint)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.moveCursor"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>moveCursor (stream, dx, dy)](#apidoc.element.mz.readline.moveCursor)
- description and source-code
```javascript
function moveCursor(stream, dx, dy) {
  if (stream === null || stream === undefined)
    return;

  if (dx < 0) {
    stream.write('\x1b[' + (-dx) + 'D');
  } else if (dx > 0) {
    stream.write('\x1b[' + dx + 'C');
  }

  if (dy < 0) {
    stream.write('\x1b[' + (-dy) + 'A');
  } else if (dy > 0) {
    stream.write('\x1b[' + dy + 'B');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.readline.stripVTControlCharacters"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>stripVTControlCharacters ()](#apidoc.element.mz.readline.stripVTControlCharacters)
- description and source-code
```javascript
function deprecated() {
  warned = exports.printDeprecationMessage(msg, warned, deprecated);
  if (new.target) {
    return Reflect.construct(fn, arguments, new.target);
  }
  return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.readline.Interface"></a>[module mz.readline.Interface](#apidoc.module.mz.readline.Interface)

#### <a name="apidoc.element.mz.readline.Interface.Interface"></a>[function <span class="apidocSignatureSpan">mz.readline.</span>Interface (input, output, completer, terminal)](#apidoc.element.mz.readline.Interface.Interface)
- description and source-code
```javascript
function InterfaceAsPromised(input, output, completer, terminal) {
  if (arguments.length === 1) {
    var options = input

    if (typeof options.completer === 'function') {
      options = objectAssign({}, options, {
        completer: wrapCompleter(options.completer)
      })
    }

    Interface.call(this, options)
  } else {
    if (typeof completer === 'function') {
      completer = wrapCompleter(completer)
    }

    Interface.call(this, input, output, completer, terminal)
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.readline.Interface.prototype"></a>[module mz.readline.Interface.prototype](#apidoc.module.mz.readline.Interface.prototype)

#### <a name="apidoc.element.mz.readline.Interface.prototype.question"></a>[function <span class="apidocSignatureSpan">mz.readline.Interface.prototype.</span>question (question, callback)](#apidoc.element.mz.readline.Interface.prototype.question)
- description and source-code
```javascript
question = function (question, callback) {
  if (typeof callback === 'function') {
    return Interface.prototype.question.call(this, question, callback)
  }

  var self = this
  return new Promise(function (resolve) {
    Interface.prototype.question.call(self, question, resolve)
  })
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib"></a>[module mz.zlib](#apidoc.module.mz.zlib)

#### <a name="apidoc.element.mz.zlib.Deflate"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Deflate (opts)](#apidoc.element.mz.zlib.Deflate)
- description and source-code
```javascript
function Deflate(opts) {
  if (!(this instanceof Deflate)) return new Deflate(opts);
  Zlib.call(this, opts, binding.DEFLATE);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.DeflateRaw"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>DeflateRaw (opts)](#apidoc.element.mz.zlib.DeflateRaw)
- description and source-code
```javascript
function DeflateRaw(opts) {
  if (!(this instanceof DeflateRaw)) return new DeflateRaw(opts);
  Zlib.call(this, opts, binding.DEFLATERAW);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Gunzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Gunzip (opts)](#apidoc.element.mz.zlib.Gunzip)
- description and source-code
```javascript
function Gunzip(opts) {
  if (!(this instanceof Gunzip)) return new Gunzip(opts);
  Zlib.call(this, opts, binding.GUNZIP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Gzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Gzip (opts)](#apidoc.element.mz.zlib.Gzip)
- description and source-code
```javascript
function Gzip(opts) {
  if (!(this instanceof Gzip)) return new Gzip(opts);
  Zlib.call(this, opts, binding.GZIP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Inflate"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Inflate (opts)](#apidoc.element.mz.zlib.Inflate)
- description and source-code
```javascript
function Inflate(opts) {
  if (!(this instanceof Inflate)) return new Inflate(opts);
  Zlib.call(this, opts, binding.INFLATE);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.InflateRaw"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>InflateRaw (opts)](#apidoc.element.mz.zlib.InflateRaw)
- description and source-code
```javascript
function InflateRaw(opts) {
  if (!(this instanceof InflateRaw)) return new InflateRaw(opts);
  Zlib.call(this, opts, binding.INFLATERAW);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Unzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Unzip (opts)](#apidoc.element.mz.zlib.Unzip)
- description and source-code
```javascript
function Unzip(opts) {
  if (!(this instanceof Unzip)) return new Unzip(opts);
  Zlib.call(this, opts, binding.UNZIP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Zlib"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Zlib ()](#apidoc.element.mz.zlib.Zlib)
- description and source-code
```javascript
function Zlib() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.createDeflate"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>createDeflate (o)](#apidoc.element.mz.zlib.createDeflate)
- description and source-code
```javascript
createDeflate = function (o) {
  return new Deflate(o);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.createDeflateRaw"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>createDeflateRaw (o)](#apidoc.element.mz.zlib.createDeflateRaw)
- description and source-code
```javascript
createDeflateRaw = function (o) {
  return new DeflateRaw(o);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.createGunzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>createGunzip (o)](#apidoc.element.mz.zlib.createGunzip)
- description and source-code
```javascript
createGunzip = function (o) {
  return new Gunzip(o);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.createGzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>createGzip (o)](#apidoc.element.mz.zlib.createGzip)
- description and source-code
```javascript
createGzip = function (o) {
  return new Gzip(o);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.createInflate"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>createInflate (o)](#apidoc.element.mz.zlib.createInflate)
- description and source-code
```javascript
createInflate = function (o) {
  return new Inflate(o);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.createInflateRaw"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>createInflateRaw (o)](#apidoc.element.mz.zlib.createInflateRaw)
- description and source-code
```javascript
createInflateRaw = function (o) {
  return new InflateRaw(o);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.createUnzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>createUnzip (o)](#apidoc.element.mz.zlib.createUnzip)
- description and source-code
```javascript
createUnzip = function (o) {
  return new Unzip(o);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.deflate"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>deflate ()](#apidoc.element.mz.zlib.deflate)
- description and source-code
```javascript
deflate = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.deflateRaw"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>deflateRaw ()](#apidoc.element.mz.zlib.deflateRaw)
- description and source-code
```javascript
deflateRaw = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.deflateRawSync"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>deflateRawSync (buffer, opts)](#apidoc.element.mz.zlib.deflateRawSync)
- description and source-code
```javascript
deflateRawSync = function (buffer, opts) {
  return zlibBufferSync(new DeflateRaw(opts), buffer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.deflateSync"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>deflateSync (buffer, opts)](#apidoc.element.mz.zlib.deflateSync)
- description and source-code
```javascript
deflateSync = function (buffer, opts) {
  return zlibBufferSync(new Deflate(opts), buffer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.gunzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>gunzip ()](#apidoc.element.mz.zlib.gunzip)
- description and source-code
```javascript
gunzip = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.gunzipSync"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>gunzipSync (buffer, opts)](#apidoc.element.mz.zlib.gunzipSync)
- description and source-code
```javascript
gunzipSync = function (buffer, opts) {
  return zlibBufferSync(new Gunzip(opts), buffer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.gzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>gzip ()](#apidoc.element.mz.zlib.gzip)
- description and source-code
```javascript
gzip = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.gzipSync"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>gzipSync (buffer, opts)](#apidoc.element.mz.zlib.gzipSync)
- description and source-code
```javascript
gzipSync = function (buffer, opts) {
  return zlibBufferSync(new Gzip(opts), buffer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.inflate"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>inflate ()](#apidoc.element.mz.zlib.inflate)
- description and source-code
```javascript
inflate = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.inflateRaw"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>inflateRaw ()](#apidoc.element.mz.zlib.inflateRaw)
- description and source-code
```javascript
inflateRaw = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.inflateRawSync"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>inflateRawSync (buffer, opts)](#apidoc.element.mz.zlib.inflateRawSync)
- description and source-code
```javascript
inflateRawSync = function (buffer, opts) {
  return zlibBufferSync(new InflateRaw(opts), buffer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.inflateSync"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>inflateSync (buffer, opts)](#apidoc.element.mz.zlib.inflateSync)
- description and source-code
```javascript
inflateSync = function (buffer, opts) {
  return zlibBufferSync(new Inflate(opts), buffer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.unzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>unzip ()](#apidoc.element.mz.zlib.unzip)
- description and source-code
```javascript
unzip = function () {
var self = this
var len = arguments.length
var lastType = typeof arguments[len - 1]
if (lastType === "function") return $$__fn__$$.apply(self, arguments)
var args = new Array(len + 1)
for (var i = 0; i < len; ++i) args[i] = arguments[i]
var lastIndex = i
return new Promise(function (resolve, reject) {
args[lastIndex] = createCallback(resolve, reject)
$$__fn__$$.apply(self, args)
})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.unzipSync"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>unzipSync (buffer, opts)](#apidoc.element.mz.zlib.unzipSync)
- description and source-code
```javascript
unzipSync = function (buffer, opts) {
  return zlibBufferSync(new Unzip(opts), buffer);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.Deflate"></a>[module mz.zlib.Deflate](#apidoc.module.mz.zlib.Deflate)

#### <a name="apidoc.element.mz.zlib.Deflate.Deflate"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Deflate (opts)](#apidoc.element.mz.zlib.Deflate.Deflate)
- description and source-code
```javascript
function Deflate(opts) {
  if (!(this instanceof Deflate)) return new Deflate(opts);
  Zlib.call(this, opts, binding.DEFLATE);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Deflate.super_"></a>[function <span class="apidocSignatureSpan">mz.zlib.Deflate.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Deflate.super_)
- description and source-code
```javascript
function Zlib(opts, mode) {
  this._opts = opts = opts || {};
  this._chunkSize = opts.chunkSize || exports.Z_DEFAULT_CHUNK;

  Transform.call(this, opts);

  if (opts.flush && !isValidFlushFlag(opts.flush)) {
    throw new Error('Invalid flush flag: ' + opts.flush);
  }
  if (opts.finishFlush && !isValidFlushFlag(opts.finishFlush)) {
    throw new Error('Invalid flush flag: ' + opts.finishFlush);
  }

  this._flushFlag = opts.flush || binding.Z_NO_FLUSH;
  this._finishFlushFlag = typeof opts.finishFlush !== 'undefined' ?
    opts.finishFlush : binding.Z_FINISH;

  if (opts.chunkSize) {
    if (opts.chunkSize < exports.Z_MIN_CHUNK ||
        opts.chunkSize > exports.Z_MAX_CHUNK) {
      throw new Error('Invalid chunk size: ' + opts.chunkSize);
    }
  }

  if (opts.windowBits) {
    if (opts.windowBits < exports.Z_MIN_WINDOWBITS ||
        opts.windowBits > exports.Z_MAX_WINDOWBITS) {
      throw new Error('Invalid windowBits: ' + opts.windowBits);
    }
  }

  if (opts.level) {
    if (opts.level < exports.Z_MIN_LEVEL ||
        opts.level > exports.Z_MAX_LEVEL) {
      throw new Error('Invalid compression level: ' + opts.level);
    }
  }

  if (opts.memLevel) {
    if (opts.memLevel < exports.Z_MIN_MEMLEVEL ||
        opts.memLevel > exports.Z_MAX_MEMLEVEL) {
      throw new Error('Invalid memLevel: ' + opts.memLevel);
    }
  }

  if (opts.strategy) {
    if (opts.strategy != exports.Z_FILTERED &&
        opts.strategy != exports.Z_HUFFMAN_ONLY &&
        opts.strategy != exports.Z_RLE &&
        opts.strategy != exports.Z_FIXED &&
        opts.strategy != exports.Z_DEFAULT_STRATEGY) {
      throw new Error('Invalid strategy: ' + opts.strategy);
    }
  }

  if (opts.dictionary) {
    if (!(opts.dictionary instanceof Buffer)) {
      throw new Error('Invalid dictionary: it should be a Buffer instance');
    }
  }

  this._handle = new binding.Zlib(mode);

  var self = this;
  this._hadError = false;
  this._handle.onerror = function(message, errno) {
    // there is no way to cleanly recover.
    // continuing only obscures problems.
    _close(self);
    self._hadError = true;

    var error = new Error(message);
    error.errno = errno;
    error.code = exports.codes[errno];
    self.emit('error', error);
  };

  var level = exports.Z_DEFAULT_COMPRESSION;
  if (typeof opts.level === 'number') level = opts.level;

  var strategy = exports.Z_DEFAULT_STRATEGY;
  if (typeof opts.strategy === 'number') strategy = opts.strategy;

  this._handle.init(opts.windowBits || exports.Z_DEFAULT_WINDOWBITS,
                    level,
                    opts.memLevel || exports.Z_DEFAULT_MEMLEVEL,
                    strategy,
                    opts.dictionary);

  this._buffer = Buffer.allocUnsafe(this._chunkSize);
  this._offset = 0;
  this._level = level;
  this._strategy = strategy;

  this.once('end', this.close);

  Object.defineProperty(this, '_closed', {
    get: () => { return !this._handle; },
    configurable: true,
    enumerable: true
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.Deflate.super_.prototype"></a>[module mz.zlib.Deflate.super_.prototype](#apidoc.module.mz.zlib.Deflate.super_.prototype)

#### <a name="apidoc.element.mz.zlib.Deflate.super_.prototype._flush"></a>[function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>_flush (callback)](#apidoc.element.mz.zlib.Deflate.super_.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
  this._transform(Buffer.alloc(0), '', callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Deflate.super_.prototype._processChunk"></a>[function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>_processChunk (chunk, flushFlag, cb)](#apidoc.element.mz.zlib.Deflate.super_.prototype._processChunk)
- description and source-code
```javascript
_processChunk = function (chunk, flushFlag, cb) {
  var availInBefore = chunk && chunk.length;
  var availOutBefore = this._chunkSize - this._offset;
  var inOff = 0;

  var self = this;

  var async = typeof cb === 'function';

  if (!async) {
    var buffers = [];
    var nread = 0;

    var error;
    this.on('error', function(er) {
      error = er;
    });

    assert(this._handle, 'zlib binding closed');
    do {
      var res = this._handle.writeSync(flushFlag,
                                       chunk, // in
                                       inOff, // in_off
                                       availInBefore, // in_len
                                       this._buffer, // out
                                       this._offset, //out_off
                                       availOutBefore); // out_len
    } while (!this._hadError && callback(res[0], res[1]));

    if (this._hadError) {
      throw error;
    }

    if (nread >= kMaxLength) {
      _close(this);
      throw new RangeError(kRangeErrorMessage);
    }

    var buf = Buffer.concat(buffers, nread);
    _close(this);

    return buf;
  }

  assert(this._handle, 'zlib binding closed');
  var req = this._handle.write(flushFlag,
                               chunk, // in
                               inOff, // in_off
                               availInBefore, // in_len
                               this._buffer, // out
                               this._offset, //out_off
                               availOutBefore); // out_len

  req.buffer = chunk;
  req.callback = callback;

  function callback(availInAfter, availOutAfter) {
    // When the callback is used in an async write, the callback's
    // context is the 'req' object that was created. The req object
    // is === this._handle, and that's why it's important to null
    // out the values after they are done being used. 'this._handle'
    // can stay in memory longer than the callback and buffer are needed.
    if (this) {
      this.buffer = null;
      this.callback = null;
    }

    if (self._hadError)
      return;

    var have = availOutBefore - availOutAfter;
    assert(have >= 0, 'have should not go down');

    if (have > 0) {
      var out = self._buffer.slice(self._offset, self._offset + have);
      self._offset += have;
      // serve some output to the consumer.
      if (async) {
        self.push(out);
      } else {
        buffers.push(out);
        nread += out.length;
      }
    }

    // exhausted the output buffer, or used all the input create a new one.
    if (availOutAfter === 0 || self._offset >= self._chunkSize) {
      availOutBefore = self._chunkSize;
      self._offset = 0;
      self._buffer = Buffer.allocUnsafe(self._chunkSize);
    }

    if (availOutAfter === 0) {
      // Not actually done.  Need to reprocess.
      // Also, update the availInBefore to the availInAfter value,
      // so that if we have to hit it a third (fourth, etc.) time,
      // it'll have the correct byte counts.
      inOff += (availInBefore - availInAfter);
      availInBefore = availInAfter;

      if (!async)
        return true;

      var newReq = self._handle.write(flushFlag,
                                      chunk,
                                      inOff,
                                      availInBefore,
                                      self._buffer,
                                      self._offset,
                                      self._chunkSize);
      newReq.callback = callback; // this same function
      newReq.buffer = chunk;
      return;
    }

    if (!async)
      return false;

    // finished with the chunk.
    cb();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Deflate.super_.prototype._transform"></a>[function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.mz.zlib.Deflate.super_.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, cb) {
  var flushFlag;
  var ws = this._writableState;
  var ending = ws.ending || ws.ended;
  var last = ending && (!chunk || ws.length === chunk.length);

  if (chunk !== null && !(chunk instanceof Buffer))
    return cb(new Error('invalid input'));

  if (!this._handle)
    return cb(new Error('zlib binding closed'));

  // If it's the last chunk, or a final flush, we use the Z_FINISH flush flag
  // (or whatever flag was provided using opts.finishFlush).
  // If it's explicitly flushing at some other time, then we use
  // Z_FULL_FLUSH. Otherwise, use Z_NO_FLUSH for maximum compression
  // goodness.
  if (last)
    flushFlag = this._finishFlushFlag;
  else {
    flushFlag = this._flushFlag;
    // once we've flushed the last of the queue, stop flushing and
    // go back to the normal behavior.
    if (chunk.length >= ws.length) {
      this._flushFlag = this._opts.flush || binding.Z_NO_FLUSH;
    }
  }

  this._processChunk(chunk, flushFlag, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Deflate.super_.prototype.close"></a>[function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>close (callback)](#apidoc.element.mz.zlib.Deflate.super_.prototype.close)
- description and source-code
```javascript
close = function (callback) {
  _close(this, callback);
  process.nextTick(emitCloseNT, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Deflate.super_.prototype.flush"></a>[function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>flush (kind, callback)](#apidoc.element.mz.zlib.Deflate.super_.prototype.flush)
- description and source-code
```javascript
flush = function (kind, callback) {
  var ws = this._writableState;

  if (typeof kind === 'function' || (kind === undefined && !callback)) {
    callback = kind;
    kind = binding.Z_FULL_FLUSH;
  }

  if (ws.ended) {
    if (callback)
      process.nextTick(callback);
  } else if (ws.ending) {
    if (callback)
      this.once('end', callback);
  } else if (ws.needDrain) {
    if (callback) {
      this.once('drain', () => this.flush(kind, callback));
    }
  } else {
    this._flushFlag = kind;
    this.write(Buffer.alloc(0), '', callback);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Deflate.super_.prototype.params"></a>[function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>params (level, strategy, callback)](#apidoc.element.mz.zlib.Deflate.super_.prototype.params)
- description and source-code
```javascript
params = function (level, strategy, callback) {
  if (level < exports.Z_MIN_LEVEL ||
      level > exports.Z_MAX_LEVEL) {
    throw new RangeError('Invalid compression level: ' + level);
  }
  if (strategy != exports.Z_FILTERED &&
      strategy != exports.Z_HUFFMAN_ONLY &&
      strategy != exports.Z_RLE &&
      strategy != exports.Z_FIXED &&
      strategy != exports.Z_DEFAULT_STRATEGY) {
    throw new TypeError('Invalid strategy: ' + strategy);
  }

  if (this._level !== level || this._strategy !== strategy) {
    var self = this;
    this.flush(binding.Z_SYNC_FLUSH, function() {
      assert(self._handle, 'zlib binding closed');
      self._handle.params(level, strategy);
      if (!self._hadError) {
        self._level = level;
        self._strategy = strategy;
        if (callback) callback();
      }
    });
  } else {
    process.nextTick(callback);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Deflate.super_.prototype.reset"></a>[function <span class="apidocSignatureSpan">mz.zlib.Deflate.super_.prototype.</span>reset ()](#apidoc.element.mz.zlib.Deflate.super_.prototype.reset)
- description and source-code
```javascript
reset = function () {
  assert(this._handle, 'zlib binding closed');
  return this._handle.reset();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.DeflateRaw"></a>[module mz.zlib.DeflateRaw](#apidoc.module.mz.zlib.DeflateRaw)

#### <a name="apidoc.element.mz.zlib.DeflateRaw.DeflateRaw"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>DeflateRaw (opts)](#apidoc.element.mz.zlib.DeflateRaw.DeflateRaw)
- description and source-code
```javascript
function DeflateRaw(opts) {
  if (!(this instanceof DeflateRaw)) return new DeflateRaw(opts);
  Zlib.call(this, opts, binding.DEFLATERAW);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.DeflateRaw.super_"></a>[function <span class="apidocSignatureSpan">mz.zlib.DeflateRaw.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.DeflateRaw.super_)
- description and source-code
```javascript
function Zlib(opts, mode) {
  this._opts = opts = opts || {};
  this._chunkSize = opts.chunkSize || exports.Z_DEFAULT_CHUNK;

  Transform.call(this, opts);

  if (opts.flush && !isValidFlushFlag(opts.flush)) {
    throw new Error('Invalid flush flag: ' + opts.flush);
  }
  if (opts.finishFlush && !isValidFlushFlag(opts.finishFlush)) {
    throw new Error('Invalid flush flag: ' + opts.finishFlush);
  }

  this._flushFlag = opts.flush || binding.Z_NO_FLUSH;
  this._finishFlushFlag = typeof opts.finishFlush !== 'undefined' ?
    opts.finishFlush : binding.Z_FINISH;

  if (opts.chunkSize) {
    if (opts.chunkSize < exports.Z_MIN_CHUNK ||
        opts.chunkSize > exports.Z_MAX_CHUNK) {
      throw new Error('Invalid chunk size: ' + opts.chunkSize);
    }
  }

  if (opts.windowBits) {
    if (opts.windowBits < exports.Z_MIN_WINDOWBITS ||
        opts.windowBits > exports.Z_MAX_WINDOWBITS) {
      throw new Error('Invalid windowBits: ' + opts.windowBits);
    }
  }

  if (opts.level) {
    if (opts.level < exports.Z_MIN_LEVEL ||
        opts.level > exports.Z_MAX_LEVEL) {
      throw new Error('Invalid compression level: ' + opts.level);
    }
  }

  if (opts.memLevel) {
    if (opts.memLevel < exports.Z_MIN_MEMLEVEL ||
        opts.memLevel > exports.Z_MAX_MEMLEVEL) {
      throw new Error('Invalid memLevel: ' + opts.memLevel);
    }
  }

  if (opts.strategy) {
    if (opts.strategy != exports.Z_FILTERED &&
        opts.strategy != exports.Z_HUFFMAN_ONLY &&
        opts.strategy != exports.Z_RLE &&
        opts.strategy != exports.Z_FIXED &&
        opts.strategy != exports.Z_DEFAULT_STRATEGY) {
      throw new Error('Invalid strategy: ' + opts.strategy);
    }
  }

  if (opts.dictionary) {
    if (!(opts.dictionary instanceof Buffer)) {
      throw new Error('Invalid dictionary: it should be a Buffer instance');
    }
  }

  this._handle = new binding.Zlib(mode);

  var self = this;
  this._hadError = false;
  this._handle.onerror = function(message, errno) {
    // there is no way to cleanly recover.
    // continuing only obscures problems.
    _close(self);
    self._hadError = true;

    var error = new Error(message);
    error.errno = errno;
    error.code = exports.codes[errno];
    self.emit('error', error);
  };

  var level = exports.Z_DEFAULT_COMPRESSION;
  if (typeof opts.level === 'number') level = opts.level;

  var strategy = exports.Z_DEFAULT_STRATEGY;
  if (typeof opts.strategy === 'number') strategy = opts.strategy;

  this._handle.init(opts.windowBits || exports.Z_DEFAULT_WINDOWBITS,
                    level,
                    opts.memLevel || exports.Z_DEFAULT_MEMLEVEL,
                    strategy,
                    opts.dictionary);

  this._buffer = Buffer.allocUnsafe(this._chunkSize);
  this._offset = 0;
  this._level = level;
  this._strategy = strategy;

  this.once('end', this.close);

  Object.defineProperty(this, '_closed', {
    get: () => { return !this._handle; },
    configurable: true,
    enumerable: true
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.Gunzip"></a>[module mz.zlib.Gunzip](#apidoc.module.mz.zlib.Gunzip)

#### <a name="apidoc.element.mz.zlib.Gunzip.Gunzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Gunzip (opts)](#apidoc.element.mz.zlib.Gunzip.Gunzip)
- description and source-code
```javascript
function Gunzip(opts) {
  if (!(this instanceof Gunzip)) return new Gunzip(opts);
  Zlib.call(this, opts, binding.GUNZIP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Gunzip.super_"></a>[function <span class="apidocSignatureSpan">mz.zlib.Gunzip.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Gunzip.super_)
- description and source-code
```javascript
function Zlib(opts, mode) {
  this._opts = opts = opts || {};
  this._chunkSize = opts.chunkSize || exports.Z_DEFAULT_CHUNK;

  Transform.call(this, opts);

  if (opts.flush && !isValidFlushFlag(opts.flush)) {
    throw new Error('Invalid flush flag: ' + opts.flush);
  }
  if (opts.finishFlush && !isValidFlushFlag(opts.finishFlush)) {
    throw new Error('Invalid flush flag: ' + opts.finishFlush);
  }

  this._flushFlag = opts.flush || binding.Z_NO_FLUSH;
  this._finishFlushFlag = typeof opts.finishFlush !== 'undefined' ?
    opts.finishFlush : binding.Z_FINISH;

  if (opts.chunkSize) {
    if (opts.chunkSize < exports.Z_MIN_CHUNK ||
        opts.chunkSize > exports.Z_MAX_CHUNK) {
      throw new Error('Invalid chunk size: ' + opts.chunkSize);
    }
  }

  if (opts.windowBits) {
    if (opts.windowBits < exports.Z_MIN_WINDOWBITS ||
        opts.windowBits > exports.Z_MAX_WINDOWBITS) {
      throw new Error('Invalid windowBits: ' + opts.windowBits);
    }
  }

  if (opts.level) {
    if (opts.level < exports.Z_MIN_LEVEL ||
        opts.level > exports.Z_MAX_LEVEL) {
      throw new Error('Invalid compression level: ' + opts.level);
    }
  }

  if (opts.memLevel) {
    if (opts.memLevel < exports.Z_MIN_MEMLEVEL ||
        opts.memLevel > exports.Z_MAX_MEMLEVEL) {
      throw new Error('Invalid memLevel: ' + opts.memLevel);
    }
  }

  if (opts.strategy) {
    if (opts.strategy != exports.Z_FILTERED &&
        opts.strategy != exports.Z_HUFFMAN_ONLY &&
        opts.strategy != exports.Z_RLE &&
        opts.strategy != exports.Z_FIXED &&
        opts.strategy != exports.Z_DEFAULT_STRATEGY) {
      throw new Error('Invalid strategy: ' + opts.strategy);
    }
  }

  if (opts.dictionary) {
    if (!(opts.dictionary instanceof Buffer)) {
      throw new Error('Invalid dictionary: it should be a Buffer instance');
    }
  }

  this._handle = new binding.Zlib(mode);

  var self = this;
  this._hadError = false;
  this._handle.onerror = function(message, errno) {
    // there is no way to cleanly recover.
    // continuing only obscures problems.
    _close(self);
    self._hadError = true;

    var error = new Error(message);
    error.errno = errno;
    error.code = exports.codes[errno];
    self.emit('error', error);
  };

  var level = exports.Z_DEFAULT_COMPRESSION;
  if (typeof opts.level === 'number') level = opts.level;

  var strategy = exports.Z_DEFAULT_STRATEGY;
  if (typeof opts.strategy === 'number') strategy = opts.strategy;

  this._handle.init(opts.windowBits || exports.Z_DEFAULT_WINDOWBITS,
                    level,
                    opts.memLevel || exports.Z_DEFAULT_MEMLEVEL,
                    strategy,
                    opts.dictionary);

  this._buffer = Buffer.allocUnsafe(this._chunkSize);
  this._offset = 0;
  this._level = level;
  this._strategy = strategy;

  this.once('end', this.close);

  Object.defineProperty(this, '_closed', {
    get: () => { return !this._handle; },
    configurable: true,
    enumerable: true
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.Gzip"></a>[module mz.zlib.Gzip](#apidoc.module.mz.zlib.Gzip)

#### <a name="apidoc.element.mz.zlib.Gzip.Gzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Gzip (opts)](#apidoc.element.mz.zlib.Gzip.Gzip)
- description and source-code
```javascript
function Gzip(opts) {
  if (!(this instanceof Gzip)) return new Gzip(opts);
  Zlib.call(this, opts, binding.GZIP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Gzip.super_"></a>[function <span class="apidocSignatureSpan">mz.zlib.Gzip.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Gzip.super_)
- description and source-code
```javascript
function Zlib(opts, mode) {
  this._opts = opts = opts || {};
  this._chunkSize = opts.chunkSize || exports.Z_DEFAULT_CHUNK;

  Transform.call(this, opts);

  if (opts.flush && !isValidFlushFlag(opts.flush)) {
    throw new Error('Invalid flush flag: ' + opts.flush);
  }
  if (opts.finishFlush && !isValidFlushFlag(opts.finishFlush)) {
    throw new Error('Invalid flush flag: ' + opts.finishFlush);
  }

  this._flushFlag = opts.flush || binding.Z_NO_FLUSH;
  this._finishFlushFlag = typeof opts.finishFlush !== 'undefined' ?
    opts.finishFlush : binding.Z_FINISH;

  if (opts.chunkSize) {
    if (opts.chunkSize < exports.Z_MIN_CHUNK ||
        opts.chunkSize > exports.Z_MAX_CHUNK) {
      throw new Error('Invalid chunk size: ' + opts.chunkSize);
    }
  }

  if (opts.windowBits) {
    if (opts.windowBits < exports.Z_MIN_WINDOWBITS ||
        opts.windowBits > exports.Z_MAX_WINDOWBITS) {
      throw new Error('Invalid windowBits: ' + opts.windowBits);
    }
  }

  if (opts.level) {
    if (opts.level < exports.Z_MIN_LEVEL ||
        opts.level > exports.Z_MAX_LEVEL) {
      throw new Error('Invalid compression level: ' + opts.level);
    }
  }

  if (opts.memLevel) {
    if (opts.memLevel < exports.Z_MIN_MEMLEVEL ||
        opts.memLevel > exports.Z_MAX_MEMLEVEL) {
      throw new Error('Invalid memLevel: ' + opts.memLevel);
    }
  }

  if (opts.strategy) {
    if (opts.strategy != exports.Z_FILTERED &&
        opts.strategy != exports.Z_HUFFMAN_ONLY &&
        opts.strategy != exports.Z_RLE &&
        opts.strategy != exports.Z_FIXED &&
        opts.strategy != exports.Z_DEFAULT_STRATEGY) {
      throw new Error('Invalid strategy: ' + opts.strategy);
    }
  }

  if (opts.dictionary) {
    if (!(opts.dictionary instanceof Buffer)) {
      throw new Error('Invalid dictionary: it should be a Buffer instance');
    }
  }

  this._handle = new binding.Zlib(mode);

  var self = this;
  this._hadError = false;
  this._handle.onerror = function(message, errno) {
    // there is no way to cleanly recover.
    // continuing only obscures problems.
    _close(self);
    self._hadError = true;

    var error = new Error(message);
    error.errno = errno;
    error.code = exports.codes[errno];
    self.emit('error', error);
  };

  var level = exports.Z_DEFAULT_COMPRESSION;
  if (typeof opts.level === 'number') level = opts.level;

  var strategy = exports.Z_DEFAULT_STRATEGY;
  if (typeof opts.strategy === 'number') strategy = opts.strategy;

  this._handle.init(opts.windowBits || exports.Z_DEFAULT_WINDOWBITS,
                    level,
                    opts.memLevel || exports.Z_DEFAULT_MEMLEVEL,
                    strategy,
                    opts.dictionary);

  this._buffer = Buffer.allocUnsafe(this._chunkSize);
  this._offset = 0;
  this._level = level;
  this._strategy = strategy;

  this.once('end', this.close);

  Object.defineProperty(this, '_closed', {
    get: () => { return !this._handle; },
    configurable: true,
    enumerable: true
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.Inflate"></a>[module mz.zlib.Inflate](#apidoc.module.mz.zlib.Inflate)

#### <a name="apidoc.element.mz.zlib.Inflate.Inflate"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Inflate (opts)](#apidoc.element.mz.zlib.Inflate.Inflate)
- description and source-code
```javascript
function Inflate(opts) {
  if (!(this instanceof Inflate)) return new Inflate(opts);
  Zlib.call(this, opts, binding.INFLATE);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Inflate.super_"></a>[function <span class="apidocSignatureSpan">mz.zlib.Inflate.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Inflate.super_)
- description and source-code
```javascript
function Zlib(opts, mode) {
  this._opts = opts = opts || {};
  this._chunkSize = opts.chunkSize || exports.Z_DEFAULT_CHUNK;

  Transform.call(this, opts);

  if (opts.flush && !isValidFlushFlag(opts.flush)) {
    throw new Error('Invalid flush flag: ' + opts.flush);
  }
  if (opts.finishFlush && !isValidFlushFlag(opts.finishFlush)) {
    throw new Error('Invalid flush flag: ' + opts.finishFlush);
  }

  this._flushFlag = opts.flush || binding.Z_NO_FLUSH;
  this._finishFlushFlag = typeof opts.finishFlush !== 'undefined' ?
    opts.finishFlush : binding.Z_FINISH;

  if (opts.chunkSize) {
    if (opts.chunkSize < exports.Z_MIN_CHUNK ||
        opts.chunkSize > exports.Z_MAX_CHUNK) {
      throw new Error('Invalid chunk size: ' + opts.chunkSize);
    }
  }

  if (opts.windowBits) {
    if (opts.windowBits < exports.Z_MIN_WINDOWBITS ||
        opts.windowBits > exports.Z_MAX_WINDOWBITS) {
      throw new Error('Invalid windowBits: ' + opts.windowBits);
    }
  }

  if (opts.level) {
    if (opts.level < exports.Z_MIN_LEVEL ||
        opts.level > exports.Z_MAX_LEVEL) {
      throw new Error('Invalid compression level: ' + opts.level);
    }
  }

  if (opts.memLevel) {
    if (opts.memLevel < exports.Z_MIN_MEMLEVEL ||
        opts.memLevel > exports.Z_MAX_MEMLEVEL) {
      throw new Error('Invalid memLevel: ' + opts.memLevel);
    }
  }

  if (opts.strategy) {
    if (opts.strategy != exports.Z_FILTERED &&
        opts.strategy != exports.Z_HUFFMAN_ONLY &&
        opts.strategy != exports.Z_RLE &&
        opts.strategy != exports.Z_FIXED &&
        opts.strategy != exports.Z_DEFAULT_STRATEGY) {
      throw new Error('Invalid strategy: ' + opts.strategy);
    }
  }

  if (opts.dictionary) {
    if (!(opts.dictionary instanceof Buffer)) {
      throw new Error('Invalid dictionary: it should be a Buffer instance');
    }
  }

  this._handle = new binding.Zlib(mode);

  var self = this;
  this._hadError = false;
  this._handle.onerror = function(message, errno) {
    // there is no way to cleanly recover.
    // continuing only obscures problems.
    _close(self);
    self._hadError = true;

    var error = new Error(message);
    error.errno = errno;
    error.code = exports.codes[errno];
    self.emit('error', error);
  };

  var level = exports.Z_DEFAULT_COMPRESSION;
  if (typeof opts.level === 'number') level = opts.level;

  var strategy = exports.Z_DEFAULT_STRATEGY;
  if (typeof opts.strategy === 'number') strategy = opts.strategy;

  this._handle.init(opts.windowBits || exports.Z_DEFAULT_WINDOWBITS,
                    level,
                    opts.memLevel || exports.Z_DEFAULT_MEMLEVEL,
                    strategy,
                    opts.dictionary);

  this._buffer = Buffer.allocUnsafe(this._chunkSize);
  this._offset = 0;
  this._level = level;
  this._strategy = strategy;

  this.once('end', this.close);

  Object.defineProperty(this, '_closed', {
    get: () => { return !this._handle; },
    configurable: true,
    enumerable: true
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.InflateRaw"></a>[module mz.zlib.InflateRaw](#apidoc.module.mz.zlib.InflateRaw)

#### <a name="apidoc.element.mz.zlib.InflateRaw.InflateRaw"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>InflateRaw (opts)](#apidoc.element.mz.zlib.InflateRaw.InflateRaw)
- description and source-code
```javascript
function InflateRaw(opts) {
  if (!(this instanceof InflateRaw)) return new InflateRaw(opts);
  Zlib.call(this, opts, binding.INFLATERAW);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.InflateRaw.super_"></a>[function <span class="apidocSignatureSpan">mz.zlib.InflateRaw.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.InflateRaw.super_)
- description and source-code
```javascript
function Zlib(opts, mode) {
  this._opts = opts = opts || {};
  this._chunkSize = opts.chunkSize || exports.Z_DEFAULT_CHUNK;

  Transform.call(this, opts);

  if (opts.flush && !isValidFlushFlag(opts.flush)) {
    throw new Error('Invalid flush flag: ' + opts.flush);
  }
  if (opts.finishFlush && !isValidFlushFlag(opts.finishFlush)) {
    throw new Error('Invalid flush flag: ' + opts.finishFlush);
  }

  this._flushFlag = opts.flush || binding.Z_NO_FLUSH;
  this._finishFlushFlag = typeof opts.finishFlush !== 'undefined' ?
    opts.finishFlush : binding.Z_FINISH;

  if (opts.chunkSize) {
    if (opts.chunkSize < exports.Z_MIN_CHUNK ||
        opts.chunkSize > exports.Z_MAX_CHUNK) {
      throw new Error('Invalid chunk size: ' + opts.chunkSize);
    }
  }

  if (opts.windowBits) {
    if (opts.windowBits < exports.Z_MIN_WINDOWBITS ||
        opts.windowBits > exports.Z_MAX_WINDOWBITS) {
      throw new Error('Invalid windowBits: ' + opts.windowBits);
    }
  }

  if (opts.level) {
    if (opts.level < exports.Z_MIN_LEVEL ||
        opts.level > exports.Z_MAX_LEVEL) {
      throw new Error('Invalid compression level: ' + opts.level);
    }
  }

  if (opts.memLevel) {
    if (opts.memLevel < exports.Z_MIN_MEMLEVEL ||
        opts.memLevel > exports.Z_MAX_MEMLEVEL) {
      throw new Error('Invalid memLevel: ' + opts.memLevel);
    }
  }

  if (opts.strategy) {
    if (opts.strategy != exports.Z_FILTERED &&
        opts.strategy != exports.Z_HUFFMAN_ONLY &&
        opts.strategy != exports.Z_RLE &&
        opts.strategy != exports.Z_FIXED &&
        opts.strategy != exports.Z_DEFAULT_STRATEGY) {
      throw new Error('Invalid strategy: ' + opts.strategy);
    }
  }

  if (opts.dictionary) {
    if (!(opts.dictionary instanceof Buffer)) {
      throw new Error('Invalid dictionary: it should be a Buffer instance');
    }
  }

  this._handle = new binding.Zlib(mode);

  var self = this;
  this._hadError = false;
  this._handle.onerror = function(message, errno) {
    // there is no way to cleanly recover.
    // continuing only obscures problems.
    _close(self);
    self._hadError = true;

    var error = new Error(message);
    error.errno = errno;
    error.code = exports.codes[errno];
    self.emit('error', error);
  };

  var level = exports.Z_DEFAULT_COMPRESSION;
  if (typeof opts.level === 'number') level = opts.level;

  var strategy = exports.Z_DEFAULT_STRATEGY;
  if (typeof opts.strategy === 'number') strategy = opts.strategy;

  this._handle.init(opts.windowBits || exports.Z_DEFAULT_WINDOWBITS,
                    level,
                    opts.memLevel || exports.Z_DEFAULT_MEMLEVEL,
                    strategy,
                    opts.dictionary);

  this._buffer = Buffer.allocUnsafe(this._chunkSize);
  this._offset = 0;
  this._level = level;
  this._strategy = strategy;

  this.once('end', this.close);

  Object.defineProperty(this, '_closed', {
    get: () => { return !this._handle; },
    configurable: true,
    enumerable: true
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.Unzip"></a>[module mz.zlib.Unzip](#apidoc.module.mz.zlib.Unzip)

#### <a name="apidoc.element.mz.zlib.Unzip.Unzip"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Unzip (opts)](#apidoc.element.mz.zlib.Unzip.Unzip)
- description and source-code
```javascript
function Unzip(opts) {
  if (!(this instanceof Unzip)) return new Unzip(opts);
  Zlib.call(this, opts, binding.UNZIP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Unzip.super_"></a>[function <span class="apidocSignatureSpan">mz.zlib.Unzip.</span>super_ (opts, mode)](#apidoc.element.mz.zlib.Unzip.super_)
- description and source-code
```javascript
function Zlib(opts, mode) {
  this._opts = opts = opts || {};
  this._chunkSize = opts.chunkSize || exports.Z_DEFAULT_CHUNK;

  Transform.call(this, opts);

  if (opts.flush && !isValidFlushFlag(opts.flush)) {
    throw new Error('Invalid flush flag: ' + opts.flush);
  }
  if (opts.finishFlush && !isValidFlushFlag(opts.finishFlush)) {
    throw new Error('Invalid flush flag: ' + opts.finishFlush);
  }

  this._flushFlag = opts.flush || binding.Z_NO_FLUSH;
  this._finishFlushFlag = typeof opts.finishFlush !== 'undefined' ?
    opts.finishFlush : binding.Z_FINISH;

  if (opts.chunkSize) {
    if (opts.chunkSize < exports.Z_MIN_CHUNK ||
        opts.chunkSize > exports.Z_MAX_CHUNK) {
      throw new Error('Invalid chunk size: ' + opts.chunkSize);
    }
  }

  if (opts.windowBits) {
    if (opts.windowBits < exports.Z_MIN_WINDOWBITS ||
        opts.windowBits > exports.Z_MAX_WINDOWBITS) {
      throw new Error('Invalid windowBits: ' + opts.windowBits);
    }
  }

  if (opts.level) {
    if (opts.level < exports.Z_MIN_LEVEL ||
        opts.level > exports.Z_MAX_LEVEL) {
      throw new Error('Invalid compression level: ' + opts.level);
    }
  }

  if (opts.memLevel) {
    if (opts.memLevel < exports.Z_MIN_MEMLEVEL ||
        opts.memLevel > exports.Z_MAX_MEMLEVEL) {
      throw new Error('Invalid memLevel: ' + opts.memLevel);
    }
  }

  if (opts.strategy) {
    if (opts.strategy != exports.Z_FILTERED &&
        opts.strategy != exports.Z_HUFFMAN_ONLY &&
        opts.strategy != exports.Z_RLE &&
        opts.strategy != exports.Z_FIXED &&
        opts.strategy != exports.Z_DEFAULT_STRATEGY) {
      throw new Error('Invalid strategy: ' + opts.strategy);
    }
  }

  if (opts.dictionary) {
    if (!(opts.dictionary instanceof Buffer)) {
      throw new Error('Invalid dictionary: it should be a Buffer instance');
    }
  }

  this._handle = new binding.Zlib(mode);

  var self = this;
  this._hadError = false;
  this._handle.onerror = function(message, errno) {
    // there is no way to cleanly recover.
    // continuing only obscures problems.
    _close(self);
    self._hadError = true;

    var error = new Error(message);
    error.errno = errno;
    error.code = exports.codes[errno];
    self.emit('error', error);
  };

  var level = exports.Z_DEFAULT_COMPRESSION;
  if (typeof opts.level === 'number') level = opts.level;

  var strategy = exports.Z_DEFAULT_STRATEGY;
  if (typeof opts.strategy === 'number') strategy = opts.strategy;

  this._handle.init(opts.windowBits || exports.Z_DEFAULT_WINDOWBITS,
                    level,
                    opts.memLevel || exports.Z_DEFAULT_MEMLEVEL,
                    strategy,
                    opts.dictionary);

  this._buffer = Buffer.allocUnsafe(this._chunkSize);
  this._offset = 0;
  this._level = level;
  this._strategy = strategy;

  this.once('end', this.close);

  Object.defineProperty(this, '_closed', {
    get: () => { return !this._handle; },
    configurable: true,
    enumerable: true
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.Zlib"></a>[module mz.zlib.Zlib](#apidoc.module.mz.zlib.Zlib)

#### <a name="apidoc.element.mz.zlib.Zlib.Zlib"></a>[function <span class="apidocSignatureSpan">mz.zlib.</span>Zlib ()](#apidoc.element.mz.zlib.Zlib.Zlib)
- description and source-code
```javascript
function Zlib() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mz.zlib.Zlib.prototype"></a>[module mz.zlib.Zlib.prototype](#apidoc.module.mz.zlib.Zlib.prototype)

#### <a name="apidoc.element.mz.zlib.Zlib.prototype.close"></a>[function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>close ()](#apidoc.element.mz.zlib.Zlib.prototype.close)
- description and source-code
```javascript
function close() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Zlib.prototype.init"></a>[function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>init ()](#apidoc.element.mz.zlib.Zlib.prototype.init)
- description and source-code
```javascript
function init() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Zlib.prototype.params"></a>[function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>params ()](#apidoc.element.mz.zlib.Zlib.prototype.params)
- description and source-code
```javascript
function params() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Zlib.prototype.reset"></a>[function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>reset ()](#apidoc.element.mz.zlib.Zlib.prototype.reset)
- description and source-code
```javascript
function reset() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Zlib.prototype.write"></a>[function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>write ()](#apidoc.element.mz.zlib.Zlib.prototype.write)
- description and source-code
```javascript
function write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mz.zlib.Zlib.prototype.writeSync"></a>[function <span class="apidocSignatureSpan">mz.zlib.Zlib.prototype.</span>writeSync ()](#apidoc.element.mz.zlib.Zlib.prototype.writeSync)
- description and source-code
```javascript
function writeSync() { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
