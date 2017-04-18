# npmtest-redux-saga

#### test coverage for  [redux-saga (v0.14.6)](https://github.com/redux-saga/redux-saga#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-redux-saga.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-redux-saga) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-redux-saga.svg)](https://travis-ci.org/npmtest/node-npmtest-redux-saga)

#### Saga middleware for Redux to handle Side Effects

[![NPM](https://nodei.co/npm/redux-saga.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/redux-saga)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-redux-saga/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-redux-saga/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-redux-saga/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-redux-saga/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-redux-saga/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-redux-saga/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-redux-saga/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-redux-saga/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-redux-saga/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-redux-saga/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-redux-saga/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-redux-saga/build/test-report.html](https://npmtest.github.io/node-npmtest-redux-saga/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-redux-saga/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-redux-saga/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-redux-saga/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-redux-saga/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-redux-saga/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-redux-saga/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-redux-saga/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-redux-saga/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Yassine ELOUAFI"
    },
    "bugs": {
        "url": "https://github.com/redux-saga/redux-saga/issues"
    },
    "dependencies": {},
    "description": "Saga middleware for Redux to handle Side Effects",
    "devDependencies": {
        "babel-cli": "^6.1.18",
        "babel-core": "^6.14.0",
        "babel-eslint": "^6.0.3",
        "babel-loader": "^6.2.5",
        "babel-polyfill": "^6.7.4",
        "babel-preset-es2015": "^6.14.0",
        "babel-preset-react": "^6.11.1",
        "babel-preset-stage-2": "^6.13.0",
        "cross-env": "^1.0.8",
        "eslint": "^2.8.0",
        "express": "^4.13.3",
        "gitbook-cli": "1.0.1",
        "isomorphic-fetch": "^2.2.0",
        "lolex": "^1.5.2",
        "react": "^15.0.0",
        "react-dom": "^15.0.0",
        "react-redux": "^4.4.5",
        "redux": "^3.5.1",
        "redux-logger": "^2.6.1",
        "rimraf": "^2.4.3",
        "tap-spec": "^4.1.1",
        "tape": "^4.2.2",
        "typescript": "^1.8.10",
        "typescript-definition-tester": "0.0.4",
        "webpack": "1.13.0",
        "webpack-dev-middleware": "^1.4.0",
        "webpack-hot-middleware": "^2.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "bc409aa0edaa4a7234759041cc70da62f37c6f13",
        "tarball": "https://registry.npmjs.org/redux-saga/-/redux-saga-0.14.6.tgz"
    },
    "gitHead": "944eac74e20fa47e2a6ac927ce743f1e073dfdd2",
    "homepage": "https://github.com/redux-saga/redux-saga#readme",
    "jsnext:main": "es/index.js",
    "keywords": [
        "javascript",
        "redux",
        "middleware",
        "saga",
        "effects",
        "side effects"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "andarist"
        },
        {
            "name": "yelouafi"
        }
    ],
    "module": "es/index.js",
    "name": "redux-saga",
    "npmFileMap": [
        {
            "basePath": "/dist/",
            "files": [
                "*.js"
            ]
        }
    ],
    "npmName": "redux-saga",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/redux-saga/redux-saga.git"
    },
    "scripts": {
        "async": "cross-env BABEL_ENV=cjs node examples/async/server.js",
        "build": "rimraf dist es && npm run build:umd:dev && npm run build:umd:prod && npm run build:es",
        "build:es": "cross-env BABEL_ENV=es babel src --out-dir es",
        "build:umd:dev": "cross-env BABEL_ENV=cjs webpack src/index.js dist/redux-saga.js --config webpack.config.dev.js",
        "build:umd:prod": "cross-env BABEL_ENV=cjs webpack src/index.js dist/redux-saga.min.js --config webpack.config.prod.js",
        "cancellable-counter": "cross-env BABEL_ENV=cjs node examples/cancellable-counter/server.js",
        "check": "npm run lint && npm run test",
        "compile": "rimraf lib && cross-env BABEL_ENV=cjs babel -d lib/ src/",
        "counter": "cross-env BABEL_ENV=cjs node examples/counter/server.js",
        "docs:build": "npm run docs:prepare && gitbook build -g redux-saga/redux-saga",
        "docs:clean": "rimraf _book",
        "docs:prepare": "gitbook install",
        "docs:publish": "npm run docs:clean && npm run docs:build && cd _book && git init && git commit --allow-empty -m 'update book' && git checkout -b gh-pages && touch .nojekyll && git add . && git commit -am 'update book' && git push git@github.com:redux-saga/redux-saga gh-pages --force",
        "docs:watch": "npm run docs:prepare && gitbook serve",
        "lint": "eslint src",
        "prepublish": "npm run check && npm run compile && npm run build",
        "real-world": "npm --prefix examples/real-world install examples/real-world && cross-env BABEL_ENV=cjs node --require babel-register examples/real-world/server.js",
        "shop": "cross-env BABEL_ENV=cjs node examples/shopping-cart/server.js",
        "test": "cross-env BABEL_ENV=cjs babel-node test/index.js | tap-spec",
        "test-async": "cross-env BABEL_ENV=cjs babel-node examples/async/test/sagas.js | tap-spec",
        "test-counter": "cross-env BABEL_ENV=cjs babel-node examples/counter/test/sagas.js | tap-spec",
        "test-shop": "cross-env BABEL_ENV=cjs babel-node examples/shopping-cart/test/sagas.js | tap-spec"
    },
    "typings": "./index.d.ts",
    "version": "0.14.6"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
