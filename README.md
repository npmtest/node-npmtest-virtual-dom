# test coverage for  [virtual-dom (v2.1.1)](https://github.com/Matt-Esch/virtual-dom)  [![npm package](https://img.shields.io/npm/v/npmtest-virtual-dom.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-virtual-dom) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-virtual-dom.svg)](https://travis-ci.org/npmtest/node-npmtest-virtual-dom)
#### A batched diff-based DOM rendering strategy

[![NPM](https://nodei.co/npm/virtual-dom.png?downloads=true)](https://www.npmjs.com/package/virtual-dom)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-virtual-dom/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-virtual-dom/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-virtual-dom/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-virtual-dom/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-virtual-dom/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-virtual-dom/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-virtual-dom/tree/gh-pages/build)|

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-virtual-dom/build/screenCapture.buildCustomOrg.browser.coverage.html.png)](https://npmtest.github.io/node-npmtest-virtual-dom/build/coverage.html/index.html)

[![test-report](https://npmtest.github.io/node-npmtest-virtual-dom/build/screenCapture.buildCustomOrg.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmtest%252Fnode-npmtest-virtual-dom%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-virtual-dom/build/test-report.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-virtual-dom/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-virtual-dom%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-virtual-dom/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-virtual-dom/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-virtual-dom/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matt-Esch",
        "email": "matt@mattesch.info"
    },
    "bugs": {
        "url": "https://github.com/Matt-Esch/virtual-dom/issues",
        "email": "matt@mattesch.info"
    },
    "contributors": [
        {
            "name": "Matt-Esch"
        }
    ],
    "dependencies": {
        "browser-split": "0.0.1",
        "error": "^4.3.0",
        "ev-store": "^7.0.0",
        "global": "^4.3.0",
        "is-object": "^1.0.1",
        "next-tick": "^0.2.2",
        "x-is-array": "0.1.0",
        "x-is-string": "0.1.0"
    },
    "description": "A batched diff-based DOM rendering strategy",
    "devDependencies": {
        "browserify": "^9.0.7",
        "istanbul": "^0.3.13",
        "min-document": "^2.14.0",
        "opn": "^1.0.1",
        "run-browser": "^2.0.2",
        "tap-dot": "^1.0.0",
        "tap-spec": "^3.0.0",
        "tape": "^4.0.0",
        "zuul": "^2.1.1"
    },
    "directories": {},
    "dist": {
        "shasum": "80eda2d481b9ede0c049118cefcb4a05f21d1375",
        "tarball": "https://registry.npmjs.org/virtual-dom/-/virtual-dom-2.1.1.tgz"
    },
    "gitHead": "b57d21284dab9e96c5d33035c0530e2396d33b41",
    "homepage": "https://github.com/Matt-Esch/virtual-dom",
    "keywords": [
        "virtual",
        "dom",
        "vdom",
        "vtree",
        "diff",
        "patch",
        "browser"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "mattesch",
            "email": "matt@mattesch.info"
        }
    ],
    "name": "virtual-dom",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/Matt-Esch/virtual-dom.git"
    },
    "scripts": {
        "browser": "run-browser test/index.js",
        "cover": "istanbul cover --report html --print detail ./test/index.js",
        "dist": "browserify --standalone virtual-dom index.js > dist/virtual-dom.js",
        "dot": "node ./test/index.js | tap-dot",
        "phantom": "run-browser test/index.js -b | tap-spec",
        "release": "npm run release-patch",
        "release-major": "git checkout master && npm version major && git push origin master --tags && npm publish",
        "release-minor": "git checkout master && npm version minor && git push origin master --tags && npm publish",
        "release-patch": "git checkout master && npm version patch && git push origin master --tags && npm publish",
        "start": "node ./index.js",
        "test": "node ./test/index.js | tap-spec",
        "travis-test": "npm run phantom && npm run cover && istanbul report lcov && ((cat coverage/lcov.info | coveralls) || exit 0)",
        "view-cover": "istanbul report html && opn ./coverage/index.html"
    },
    "testling": {
        "files": "test/*.js",
        "browsers": [
            "ie/8..latest",
            "firefox/17..latest",
            "firefox/nightly",
            "chrome/22..latest",
            "chrome/canary",
            "opera/12..latest",
            "opera/next",
            "safari/5.1..latest",
            "ipad/6.0..latest",
            "iphone/6.0..latest",
            "android-browser/4.2..latest"
        ]
    },
    "version": "2.1.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
