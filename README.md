# npmdoc-electron-compile

#### basic api documentation for  [electron-compile (v6.4.0)](https://github.com/paulcbetts/electron-compile)  [![npm package](https://img.shields.io/npm/v/npmdoc-electron-compile.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electron-compile) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electron-compile.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electron-compile)

#### Electron supporting package to compile JS and CSS in Electron applications

[![NPM](https://nodei.co/npm/electron-compile.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/electron-compile)

- [https://npmdoc.github.io/node-npmdoc-electron-compile/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-electron-compile/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-compile/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-compile/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-electron-compile/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-electron-compile/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Paul Betts"
    },
    "bin": {
        "electron-compile": "lib/cli.js",
        "electron-packager-compile": "lib/packager-cli.js"
    },
    "bugs": {
        "url": "https://github.com/paulcbetts/electron-compile/issues"
    },
    "dependencies": {
        "@paulcbetts/mime-types": "^2.1.10",
        "@types/node": "^7.0.12",
        "btoa": "^1.1.2",
        "debug": "^2.5.1",
        "lru-cache": "^4.0.1",
        "mkdirp": "^0.5.1",
        "pify": "^2.3.0",
        "rimraf": "^2.5.4",
        "rxjs": "^5.1.1",
        "spawn-rx": "^2.0.3",
        "yargs": "^4.8.1"
    },
    "description": "Electron supporting package to compile JS and CSS in Electron applications",
    "devDependencies": {
        "asar": "^0.12.1",
        "babel-cli": "^6.11.4",
        "babel-eslint": "^6.1.2",
        "babel-plugin-array-includes": "^2.0.3",
        "babel-plugin-istanbul": "^4.0.0",
        "babel-plugin-transform-async-to-generator": "^6.8.0",
        "babel-preset-es2016-node5": "^1.1.2",
        "babel-preset-react": "^6.11.1",
        "babel-register": "^6.11.6",
        "chai": "^3.5.0",
        "chai-as-promised": "^5.3.0",
        "cheerio": "^0.20.0",
        "cross-env": "^3.2.4",
        "electron-compilers": "^5.8.0",
        "electron-packager": "^7.5.1",
        "electron-prebuilt": "^1.3.3",
        "esdoc": "^0.4.8",
        "esdoc-es7-plugin": "0.0.3",
        "esdoc-plugin-async-to-sync": "^0.5.0",
        "eslint": "^3.3.0",
        "istanbul": "^0.4.5",
        "mocha": "^3.0.2"
    },
    "directories": {},
    "dist": {
        "shasum": "c2670d8b512f41613ed37dea7a8b22548ca754ae",
        "tarball": "https://registry.npmjs.org/electron-compile/-/electron-compile-6.4.0.tgz"
    },
    "engines": {
        "node": ">= 5.0"
    },
    "gitHead": "7dffa22995c83a2def8f164d5ef486f46f57cc1a",
    "homepage": "https://github.com/paulcbetts/electron-compile",
    "keywords": [
        "electron"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "paulcbetts"
        }
    ],
    "name": "electron-compile",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/paulcbetts/electron-compile.git"
    },
    "scripts": {
        "compile": "cross-env NODE_ENV='production' git clean -xdf lib && babel -d lib/ src",
        "doc": "esdoc -c ./esdoc.json",
        "prepublish": "npm run compile",
        "start": "npm run compile && electron ./test-dist/electron-smoke-test.js",
        "test": "mocha --compilers js:babel-register test/*.js",
        "test-cov": "cross-env NODE_ENV='test' istanbul cover ./node_modules/mocha/bin/_mocha -- --compilers js:babel-register test/*.js"
    },
    "types": "types/index.d.ts",
    "version": "6.4.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
