# float-equal [![Build Status](https://travis-ci.org/sindresorhus/float-equal.svg?branch=master)](https://travis-ci.org/sindresorhus/float-equal)

> Check if two floats are almost equal

Due to [rounding errors](http://stackoverflow.com/questions/588004/is-floating-point-math-broken) you shouldn't compare floats directly. Instead this module takes an [upperbound](https://en.wikipedia.org/wiki/Machine_epsilon) for rounding errors into consideration.


## Install

```
$ npm install --save float-equal
```


## Usage

```js
var floatEqual = require('float-equal');

console.log(0.1 + 0.2 === 0.3);
//=> false

console.log(floatEqual(0.1 + 0.2, 0.3));
//=> true
```


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
