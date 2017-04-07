# api documentation for  [react-notification (v6.6.0)](https://github.com/pburtchaell/react-notification)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-notification.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-notification) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-notification.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-notification)
#### Snackbar style notification component for React

[![NPM](https://nodei.co/npm/react-notification.png?downloads=true)](https://www.npmjs.com/package/react-notification)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-notification/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-react-notification_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-notification/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-notification/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-notification/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Patrick Burtchaell",
        "email": "patrick@pburtchaell.com",
        "url": "pburtchaell.com"
    },
    "bugs": {
        "url": "https://github.com/pburtchaell/react-notification/issues"
    },
    "dependencies": {},
    "description": "Snackbar style notification component for React",
    "devDependencies": {
        "babel-cli": "^6.6.5",
        "babel-core": "^6.7.2",
        "babel-eslint": "^7.1.1",
        "babel-loader": "^6.2.4",
        "babel-plugin-transform-object-assign": "^6.8.0",
        "babel-preset-es2015": "^6.6.0",
        "babel-preset-react": "^6.5.0",
        "babel-preset-stage-0": "^6.5.0",
        "chai": "^3.5.0",
        "chai-enzyme": "^0.6.0",
        "cheerio": "^0.22.0",
        "enzyme": "^2.1.0",
        "eslint": "^3.10.2",
        "eslint-config-airbnb": "^13.0.0",
        "eslint-plugin-import": "^2.2.0",
        "eslint-plugin-jsx-a11y": "^2.2.3",
        "eslint-plugin-react": "^6.7.1",
        "express": "^4.13.4",
        "express-urlrewrite": "^1.2.0",
        "html-webpack-plugin": "^2.10.0",
        "immutable": "^3.8.1",
        "jsdom": "^9.8.3",
        "mocha": "^3.1.2",
        "pre-commit": "^1.1.3",
        "react": "^15.0.0",
        "react-addons-test-utils": "^15.0.0",
        "react-dom": "^15.0.0",
        "sinon": "^1.17.3",
        "webpack": "^1.12.14",
        "webpack-dev-middleware": "^1.5.1",
        "webpack-dev-server": "^1.14.1"
    },
    "directories": {},
    "dist": {
        "shasum": "791302e1522b0d2529daaab3b80839bcafd28fad",
        "tarball": "https://registry.npmjs.org/react-notification/-/react-notification-6.6.0.tgz"
    },
    "gitHead": "93154d5d868dbf98421676628056e423368cb0e8",
    "homepage": "https://github.com/pburtchaell/react-notification",
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
    "license": "MIT",
    "main": "dist/index.js",
    "maintainers": [
        {
            "name": "berkeleytrue",
            "email": "berkeley@r3dm.com"
        },
        {
            "name": "pburtchaell",
            "email": "patrick@pburtchaell.com"
        }
    ],
    "name": "react-notification",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0"
    },
    "pre-commit": [
        "precommit"
    ],
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "https+git://github.com/pburtchaell/react-notification"
    },
    "scripts": {
        "build": "'npm bin'/babel src -d dist",
        "lint": "'npm bin'/eslint src/**/*.js test/**/*.js",
        "prebuild": "npm test",
        "precommit": "echo 'Running pre-commit hooks...' && npm test",
        "prepublish": "npm run build",
        "pretest": "npm run lint",
        "start": "node examples/server.js",
        "test": "./bin/test.sh"
    },
    "version": "6.6.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-notification](#apidoc.module.react-notification)
1.  [function <span class="apidocSignatureSpan">react-notification.</span>Notification (props)](#apidoc.element.react-notification.Notification)
1.  [function <span class="apidocSignatureSpan">react-notification.</span>NotificationStack (props)](#apidoc.element.react-notification.NotificationStack)



# <a name="apidoc.module.react-notification"></a>[module react-notification](#apidoc.module.react-notification)

#### <a name="apidoc.element.react-notification.Notification"></a>[function <span class="apidocSignatureSpan">react-notification.</span>Notification (props)](#apidoc.element.react-notification.Notification)
- description and source-code
```javascript
function Notification(props) {
  _classCallCheck(this, Notification);

  var _this = _possibleConstructorReturn(this, (Notification.__proto__ || Object.getPrototypeOf(Notification)).call(this, props));

  _this.getBarStyle = _this.getBarStyle.bind(_this);
  _this.getActionStyle = _this.getActionStyle.bind(_this);
  _this.getTitleStyle = _this.getTitleStyle.bind(_this);
  _this.handleClick = _this.handleClick.bind(_this);

  if (props.onDismiss && props.isActive) {
    _this.dismissTimeout = setTimeout(props.onDismiss, props.dismissAfter);
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-notification.NotificationStack"></a>[function <span class="apidocSignatureSpan">react-notification.</span>NotificationStack (props)](#apidoc.element.react-notification.NotificationStack)
- description and source-code
```javascript
function NotificationStack(props) {
  return _react2.default.createElement(
    'div',
    { className: 'notification-list' },
    props.notifications.map(function (notification, index) {
      var isLast = index === 0 && props.notifications.length === 1;
      var dismissNow = isLast || !props.dismissInOrder;

      // Handle styles
      var barStyle = props.barStyleFactory(index, notification.barStyle);
      var activeBarStyle = props.activeBarStyleFactory(index, notification.activeBarStyle);

      // Allow onClick from notification stack or individual notifications
      var onClick = notification.onClick || props.onClick;
      var onDismiss = props.onDismiss;

      var dismissAfter = notification.dismissAfter;


      if (dismissAfter !== false) {
        if (dismissAfter == null) dismissAfter = props.dismissAfter;
        if (!dismissNow) dismissAfter += index * 1000;
      }

      return _react2.default.createElement(_stackedNotification2.default, _extends({}, notification, {
        key: notification.key,
        isLast: isLast,
        action: notification.action || props.action,
        dismissAfter: dismissAfter,
        onDismiss: onDismiss.bind(undefined, notification),
        onClick: onClick.bind(undefined, notification),
        activeBarStyle: activeBarStyle,
        barStyle: barStyle
      }));
    })
  );
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
