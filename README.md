# npmdoc-coveralls

#### basic api documentation for  [coveralls (v2.13.0)](https://github.com/nickmerwin/node-coveralls#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-coveralls.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-coveralls) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-coveralls.svg)](https://travis-ci.org/npmdoc/node-npmdoc-coveralls)

#### takes json-cov output into stdin and POSTs to coveralls.io

[![NPM](https://nodei.co/npm/coveralls.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/coveralls)

- [https://npmdoc.github.io/node-npmdoc-coveralls/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-coveralls/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-coveralls/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-coveralls/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-coveralls/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-coveralls/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Gregg Caines"
    },
    "bin": {
        "coveralls": "./bin/coveralls.js"
    },
    "bugs": {
        "url": "https://github.com/nickmerwin/node-coveralls/issues"
    },
    "contributors": [
        {
            "name": "Gregg Caines",
            "url": "http://caines.ca"
        },
        {
            "name": "Joshua Ma",
            "url": "http://joshma.com"
        },
        {
            "name": "Alan Gutierrez",
            "url": "http://www.prettyrobots.com/"
        },
        {
            "name": "Kir Belevich",
            "url": "https://github.com/svg"
        },
        {
            "name": "elliotcable",
            "url": "http://elliottcable.name/"
        },
        {
            "name": "Slotos",
            "url": "http://slotos.net"
        },
        {
            "name": "mattjmorrison",
            "url": "http://mattjmorrison.com"
        },
        {
            "name": "Arpad Borsos",
            "url": "http://swatinem.de/"
        },
        {
            "name": "Adam Moss",
            "url": "https://github.com/adam-moss"
        }
    ],
    "dependencies": {
        "js-yaml": "3.6.1",
        "lcov-parse": "0.0.10",
        "log-driver": "1.2.5",
        "minimist": "1.2.0",
        "request": "2.79.0"
    },
    "description": "takes json-cov output into stdin and POSTs to coveralls.io",
    "devDependencies": {
        "istanbul": "0.4.5",
        "jshint": "2.9.3",
        "mocha": "3.2.0",
        "mocha-lcov-reporter": "1.2.0",
        "should": "9.0.2",
        "sinon-restore": "1.0.1",
        "snyk": "1.23.3"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "df933876e8c6f478efb04f4d3ab70dc96b7e5a8e",
        "tarball": "https://registry.npmjs.org/coveralls/-/coveralls-2.13.0.tgz"
    },
    "engines": {
        "node": ">=0.8.6"
    },
    "gitHead": "28212004077299a871a6216273cce7a502e2ce67",
    "homepage": "https://github.com/nickmerwin/node-coveralls#readme",
    "keywords": [
        "coverage",
        "coveralls"
    ],
    "license": "BSD-2-Clause",
    "main": "index.js",
    "maintainers": [
        {
            "name": "cainus"
        },
        {
            "name": "nickmerwin"
        }
    ],
    "name": "coveralls",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/nickmerwin/node-coveralls.git"
    },
    "scripts": {
        "test": "snyk test && make test"
    },
    "version": "2.13.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
