# npmtest-neo4j

#### basic test coverage for  neo4j (v2.0.0-RC2)  [![npm package](https://img.shields.io/npm/v/npmtest-neo4j.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-neo4j) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-neo4j.svg)](https://travis-ci.org/npmtest/node-npmtest-neo4j)

#### Neo4j driver (REST API client) for Node.js

[![NPM](https://nodei.co/npm/neo4j.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/neo4j)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-neo4j/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-neo4j/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-neo4j/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-neo4j/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-neo4j/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-neo4j/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-neo4j/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-neo4j/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-neo4j/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-neo4j/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-neo4j/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-neo4j/build/test-report.html](https://npmtest.github.io/node-npmtest-neo4j/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-neo4j/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-neo4j/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-neo4j/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-neo4j/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-neo4j/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-neo4j/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-neo4j/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-neo4j/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "neo4j",
    "description": "Neo4j driver (REST API client) for Node.js",
    "version": "2.0.0-RC2",
    "author": "Aseem Kishore <aseem.kishore@gmail.com>",
    "contributors": [
        "Daniel Gasienica <daniel@gasienica.ch>",
        "Sergio Haro <sergio.haro.jr@gmail.com>"
    ],
    "main": "./lib-new/exports",
    "dependencies": {
        "request": "^2.27.0",
        "underscore": "1.7.x"
    },
    "devDependencies": {
        "chai": "^1.9.2",
        "coffee-script": "1.8.x",
        "coffeelint": "^1.9.7",
        "mocha": "^2.0.1",
        "streamline": "^0.10.16"
    },
    "engines": {
        "node": ">= 0.10"
    },
    "scripts": {
        "build": "coffee -m -c lib-new/",
        "clean": "rm -f lib-new/*.{js,map}",
        "lint": "git ls-files | grep coffee$ | grep -v '\\-old/' | xargs coffeelint",
        "prepublish": "npm run build",
        "postpublish": "npm run clean",
        "test": "mocha test-new"
    },
    "keywords": [
        "neo4j",
        "graph",
        "database",
        "driver",
        "client",
        "cypher"
    ],
    "license": "Apache-2.0",
    "repository": {
        "type": "git",
        "url": "https://github.com/thingdom/node-neo4j.git"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
