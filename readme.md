# latest-version [![Build Status](https://travis-ci.org/sindresorhus/latest-version.svg?branch=master)](https://travis-ci.org/sindresorhus/latest-version)

> Get the latest version of a npm package

Fetches the version directly from the registry instead of depending on the massive [npm](https://github.com/npm/npm/blob/8b5e7b6ae5b4cd2d7d62eaf93b1428638b387072/package.json#L37-L85) module like the [latest](https://github.com/bahamas10/node-latest) module does.


## Install

```
$ npm install --save latest-version
```


## Usage

```js
const latestVersion = require('latest-version');

latestVersion('pageres', (err, version) => {
	console.log(version);
	//=> '0.2.3'
});
```


## CLI

```
$ npm install --global latest-version
```

```
$ latest-version --help

  Usage
    $ latest-version <package-name>

  Example
    $ latest-version pageres
    0.4.1
```


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
