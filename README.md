# test coverage for  [generator-express (v2.15.0)](https://github.com/petecoop/generator-express)  [![npm package](https://img.shields.io/npm/v/npmtest-generator-express.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-generator-express) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-generator-express.svg)](https://travis-ci.org/npmtest/node-npmtest-generator-express)
#### A nodejs express generator for Yeoman

[![NPM](https://nodei.co/npm/generator-express.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/generator-express)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-generator-express/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-generator-express/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-generator-express/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-generator-express/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-generator-express/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-generator-express/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-generator-express/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-generator-express/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-generator-express/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-generator-express/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-generator-express/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-generator-express/build/test-report.html](https://npmtest.github.io/node-npmtest-generator-express/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-generator-express/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-generator-express/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-generator-express/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-generator-express/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-generator-express/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-generator-express/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-generator-express/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-generator-express/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "petecoop",
        "url": "http://petecoop.co.uk"
    },
    "bugs": {
        "url": "https://github.com/petecoop/generator-express/issues"
    },
    "contributors": [
        {
            "name": "nategood",
            "url": "http://nategood.com"
        }
    ],
    "dependencies": {
        "glob": "^7.0.0",
        "mkdirp": "^0.5.0",
        "underscore.string": "^3.0.3",
        "yeoman-generator": "^1.0.0"
    },
    "description": "A nodejs express generator for Yeoman",
    "devDependencies": {
        "mocha": "^2.1.0",
        "rimraf": "^2.3.2",
        "yeoman-assert": "^2.2.1",
        "yeoman-test": "^1.4.0"
    },
    "directories": {},
    "dist": {
        "shasum": "17d98cc590d7ba19cb6f348813adc88157e13303",
        "tarball": "https://registry.npmjs.org/generator-express/-/generator-express-2.15.0.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "gitHead": "c0dd893f80f7f68c7a1a86f908d9d0932db9d2bc",
    "homepage": "https://github.com/petecoop/generator-express",
    "keywords": [
        "yeoman-generator",
        "express",
        "scaffold"
    ],
    "licenses": [
        {
            "type": "MIT"
        }
    ],
    "main": "app/index.js",
    "maintainers": [
        {
            "name": "petecoop"
        }
    ],
    "name": "generator-express",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/petecoop/generator-express.git"
    },
    "scripts": {
        "test": "mocha",
        "test:generate": "npm link && npm run test:generate:basic && npm run test:generate:mvc",
        "test:generate:basic": "mkdir temp; cd temp && yo express --createDirectory true --dirname one --basic true --viewEngine handlebars --cssPreprocessor css --buildTool gulp && cd one && npm run test:coverage",
        "test:generate:mvc": "mkdir temp; cd temp && yo express --createDirectory true --dirname two --mvc true --viewEngine handlebars --cssPreprocessor css --database sqlite --buildTool gulp && cd two && npm run test:coverage"
    },
    "version": "2.15.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
