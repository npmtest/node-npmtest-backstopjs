# npmtest-backstopjs

#### basic test coverage for  backstopjs (v2.6.11)  [![npm package](https://img.shields.io/npm/v/npmtest-backstopjs.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-backstopjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-backstopjs.svg)](https://travis-ci.org/npmtest/node-npmtest-backstopjs)

#### BackstopJS: Catch CSS curveballs.

[![NPM](https://nodei.co/npm/backstopjs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/backstopjs)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-backstopjs/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-backstopjs/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-backstopjs/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-backstopjs/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-backstopjs/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-backstopjs/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-backstopjs/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-backstopjs/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-backstopjs/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-backstopjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-backstopjs/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-backstopjs/build/test-report.html](https://npmtest.github.io/node-npmtest-backstopjs/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-backstopjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-backstopjs/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-backstopjs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-backstopjs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-backstopjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-backstopjs/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-backstopjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-backstopjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "backstopjs",
    "version": "2.6.11",
    "description": "BackstopJS: Catch CSS curveballs.",
    "bin": {
        "backstop": "./cli/index.js"
    },
    "scripts": {
        "lint": "npm run lint-web && npm run lint-node",
        "lint-web": "eslint --env browser compare/*.js compare/**/*.js --fix",
        "lint-node": "eslint --env node core/*.js core/**/*.js cli/*.js cli/**/*.js capture/*.js capture/**/*.js --fix",
        "genConfig": "node ./cli/index.js genConfig",
        "reference": "node ./cli/index.js reference",
        "test": "node ./cli/index.js test",
        "openReport": "node ./cli/index.js openReport",
        "echo": "node ./cli/index.js echo",
        "unit-test": "mocha --reporter spec --recursive test/",
        "integration-test": "rm -rf newdir && mkdir newdir && cd newdir && node ../cli/index.js genConfig && node ../cli/index.js reference && node ../cli/index.js test && node -e \"require('../')('test')\""
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/garris/backstopjs.git"
    },
    "author": "https://github.com/garris/BackstopJS/graphs/contributors",
    "license": "MIT",
    "main": "core/runner.js",
    "devDependencies": {
        "assert": "^1.4.1",
        "eslint": "^3.3.0",
        "eslint-config-semistandard": "^7.0.0-beta.0",
        "eslint-config-standard": "^6.0.0",
        "eslint-plugin-promise": "^3.3.0",
        "eslint-plugin-standard": "^2.0.0",
        "mocha": "^1.21.5",
        "mockery": "^1.4.0"
    },
    "dependencies": {
        "casperjs": "^1.1.0-beta5",
        "chalk": "^1.1.3",
        "fs-extra": "^0.30.0",
        "junitwriter": "~0.3.1",
        "minimist": "^1.2.0",
        "node-resemble-js": "^0.2.0",
        "object-hash": "1.1.5",
        "open": "0.0.5",
        "os": "^0.1.1",
        "p-map": "^1.1.1",
        "phantomjs-prebuilt": "^2.1.7",
        "temp": "^0.8.3"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
