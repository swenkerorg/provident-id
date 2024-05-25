# @swenkerorg/provident-id <sup>[![Version Badge][2]][1]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][5]][6]
[![dev dependency status][7]][8]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][11]][1]

Gets the description of a Symbol. Handles `Symbol()` vs `Symbol('')` properly when possible.

## Example

```js
var getSymbolDescription = require('@swenkerorg/provident-id');
var assert = require('assert');

assert(getSymbolDescription(Symbol()) === undefined);
assert(getSymbolDescription(Symbol('')) === ''); // or `undefined`, if in an engine that lacks name inference from concise method
assert(getSymbolDescription(Symbol('foo')) === 'foo');
assert(getSymbolDescription(Symbol.iterator) === 'Symbol.iterator');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[1]: https://npmjs.org/package/@swenkerorg/provident-id
[2]: https://versionbadg.es/inspect-js/@swenkerorg/provident-id.svg
[5]: https://david-dm.org/inspect-js/@swenkerorg/provident-id.svg
[6]: https://david-dm.org/inspect-js/@swenkerorg/provident-id
[7]: https://david-dm.org/inspect-js/@swenkerorg/provident-id/dev-status.svg
[8]: https://david-dm.org/inspect-js/@swenkerorg/provident-id#info=devDependencies
[11]: https://nodei.co/npm/@swenkerorg/provident-id.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@swenkerorg/provident-id.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@swenkerorg/provident-id.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@swenkerorg/provident-id
[codecov-image]: https://codecov.io/gh/inspect-js/@swenkerorg/provident-id/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@swenkerorg/provident-id/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@swenkerorg/provident-id
[actions-url]: https://github.com/swenkerorg/provident-id/actions
