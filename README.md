
<img src="https://user-images.githubusercontent.com/98138701/173466440-2a051a17-b509-4ca6-9499-87bc3b2d0944.png" width="300px"/>

A little javascript library for checking argument values

[![Build](https://github.com/thiagodnf/check-arguments/actions/workflows/build.yml/badge.svg)](https://github.com/thiagodnf/check-arguments/actions/workflows/build.yml)
[![GitHub Release](https://img.shields.io/github/release/thiagodnf/check-arguments.svg)](https://github.com/thiagodnf/check-arguments/releases/latest)
[![GitHub contributors](https://img.shields.io/github/contributors/thiagodnf/check-arguments.svg)](https://github.com/thiagodnf/check-arguments/graphs/contributors)
[![GitHub stars](https://img.shields.io/github/stars/thiagodnf/check-arguments.svg)](https://github.com/thiagodnf/check-arguments)
[![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php)
[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)

## Why

It takes time to add explicit conditions to your functions to check arguments and throw errors. The purpose of this library is to assist developers on writing efficiently and reliably those conditions.

## How Do I Install It?

Via NPM:

```sh
npm i check-arguments --save
```

## How to I Use It?

Loading the library:

```js
const { check } = require("check-arguments");
```

Now you can use it on your functions:

```js
function foo(val){

    check(val).isString().isNotBlank();

    // The remaining source code
}
```

or
```js
function foo(a, b){

    check(a).isInt().isBetween(12, 20);
    check(b).isString();

    // The remaining source code
}
```

### Predicates

These are the list of predicates you may use

For `isNumber()`:

 - `isLessThan(max)`
 - `isLessThanOrEqualsTo(max)`
 - `isGreaterThan(min)`
 - `isGreaterThanOrEqualsTo(min)`
 - `isBetween(min, max)`
 - `inRange(min, max)`
 - `isPositive()`
 - `isNegative()`

For `isInt()`:

 - `isEven()`
 - `isOdd()`

For `isString()`:

 - `isNotBlank()`

For `isObject()`:

 - `hasKey()`
 - `isEmpty()`

## For Developers

Install the dependencies

```bash
npm install
```

Run the development enviroment

```bash
npm run dev
```

## Questions or Suggestions

Feel free to access the <a href="../../discussions">discussions tab</a> as you need

## Contribute

Contributions to the this project are very welcome! We can't do this alone! Feel free to fork this project, work on it and then make a pull request.

## License

Licensed under the [MIT license](LICENSE).

## Donate

I open-source almost everything I can, and I try to reply to everyone needing help using these projects. Obviously, this takes time. You can integrate and use these projects in your applications for free! You can even change the source code and redistribute (even resell it).

However, if you get some profit from this or just want to encourage me to continue creating stuff, reach out to me if you want to do it.

Thanks!

❤️
