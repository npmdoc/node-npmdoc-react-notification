# npmdoc-react-notification

#### api documentation for  [react-notification (v6.6.1)](https://github.com/pburtchaell/react-notification)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-notification.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-notification) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-notification.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-notification)

#### Snackbar style notification component for React

[![NPM](https://nodei.co/npm/react-notification.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-notification)

- [https://npmdoc.github.io/node-npmdoc-react-notification/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-notification/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-notification/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-notification/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-notification/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-notification/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "react-notification",
    "version": "6.6.1",
    "description": "Snackbar style notification component for React",
    "main": "dist/index.js",
    "scripts": {
        "prepublish": "npm run build",
        "precommit": "echo 'Running pre-commit hooks...' && npm test",
        "prebuild": "npm test",
        "build": "'npm bin'/babel src -d dist",
        "pretest": "npm run lint",
        "test": "./bin/test.sh",
        "lint": "'npm bin'/eslint src/**/*.js test/**/*.js",
        "start": "node examples/server.js"
    },
    "pre-commit": [
        "precommit"
    ],
    "repository": {
        "type": "git",
        "url": "https+git://github.com/pburtchaell/react-notification"
    },
    "keywords": [
        "react",
        "component",
        "react-component",
        "components",
        "ui",
        "notify",
        "notification",
        "notification stack",
        "snackbar"
    ],
    "author": "Patrick Burtchaell <patrick@pburtchaell.com> (pburtchaell.com)",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/pburtchaell/react-notification/issues"
    },
    "homepage": "https://github.com/pburtchaell/react-notification",
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0"
    },
    "devDependencies": {
        "babel-cli": "^6.24.1",
        "babel-core": "^6.24.1",
        "babel-eslint": "^7.2.2",
        "babel-loader": "^6.4.1",
        "babel-plugin-transform-object-assign": "^6.22.0",
        "babel-preset-es2015": "^6.24.1",
        "babel-preset-react": "^6.24.1",
        "babel-preset-stage-0": "^6.24.1",
        "chai": "^3.5.0",
        "chai-enzyme": "^0.6.0",
        "cheerio": "^0.22.0",
        "enzyme": "^2.8.2",
        "eslint": "^3.10.2",
        "eslint-config-airbnb": "^13.0.0",
        "eslint-plugin-import": "^2.2.0",
        "eslint-plugin-jsx-a11y": "^2.2.3",
        "eslint-plugin-react": "^6.7.1",
        "express": "^4.15.2",
        "express-urlrewrite": "^1.2.0",
        "html-webpack-plugin": "^2.28.0",
        "immutable": "^3.8.1",
        "jsdom": "^9.12.0",
        "mocha": "^3.2.0",
        "pre-commit": "^1.2.2",
        "react": "^15.5.4",
        "react-dom": "^15.5.4",
        "react-test-renderer": "^15.5.4",
        "sinon": "^1.17.3",
        "webpack": "^1.12.14",
        "webpack-dev-middleware": "^1.10.1",
        "webpack-dev-server": "^1.14.1"
    },
    "dependencies": {
        "prop-types": "^15.5.8",
        "react-addons-test-utils": "^15.5.1"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
