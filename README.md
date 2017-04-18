# npmdoc-mz

#### api documentation for  [mz (v2.6.0)](https://github.com/normalize/mz#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-mz.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mz) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mz.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mz)

#### modernize node.js to current ECMAScript standards

[![NPM](https://nodei.co/npm/mz.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/mz)

- [https://npmdoc.github.io/node-npmdoc-mz/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-mz/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mz/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mz/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mz/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mz/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jonathan Ong",
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
            "name": "coderhaoxin"
        },
        {
            "name": "dead-horse"
        },
        {
            "name": "dead_horse"
        },
        {
            "name": "evancarroll"
        },
        {
            "name": "jongleberry"
        },
        {
            "name": "linusu"
        },
        {
            "name": "rstacruz"
        },
        {
            "name": "swatinem"
        }
    ],
    "name": "mz",
    "optionalDependencies": {},
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



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
