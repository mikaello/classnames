# Changelog

## v2.3.0 / 2019-16.10

* Added alternate `list` version of classNames, which returns a list of classes instead of a single string. 

## v2.2.6 / 2018-06-08

* Fixed compatibility issue with usage in an es module environment

## v2.2.5 / 2016-05-02

* Improved performance of `dedupe` variant even further, thanks [Andres Suarez](https://github.com/zertosh)

## v2.2.4 / 2016-04-25

* Improved performance of `dedupe` variant by about 2x, thanks [Bartosz Gościński](https://github.com/bgoscinski)

## v2.2.3 / 2016-01-05

* Updated `bind` variant to use `[].join(' ')` as per the main script in 2.2.2

## v2.2.2 / 2016-01-04

* Switched from string concatenation to `[].join(' ')` for a slight performance gain in the main function.

## v2.2.1 / 2015-11-26

* Add deps parameter to the AMD module, fixes an issue using the Dojo loader, thanks [Chris Jordan](https://github.com/flipperkid)

## v2.2.0 / 2015-10-18

* added a new `bind` variant for use with [css-modules](https://github.com/css-modules/css-modules) and similar abstractions, thanks to [Kirill Yakovenko](https://github.com/blia)

## v2.1.5 / 2015-09-30

* reverted a new usage of `Object.keys` in `dedupe.js` that slipped through in the last release

## v2.1.4 / 2015-09-30

* new case added to benchmarks
* safer `hasOwnProperty` check
* AMD module is now named, so you can do the following:

```
define(["classnames"], function (classNames) {
  var style = classNames("foo", "bar");
  // ...
});
```

## v2.1.3 / 2015-07-02

* updated UMD wrapper to support AMD and CommonJS on the same pacge

## v2.1.2 / 2015-05-28

* added a proper UMD wrapper

## v2.1.1 / 2015-05-06

* minor performance improvement thanks to type caching
* improved benchmarking and results output

## v2.1.0 / 2015-05-05

* added alternate `dedupe` version of classNames, which is slower (10x) but ensures that if a class is added then overridden by a falsy value in a subsequent argument, it is excluded from the result.

## v2.0.0 / 2015-05-03

* performance improvement; switched to `Array.isArray` for type detection, which is much faster in modern browsers. A polyfill is now required for IE8 support, see the Readme for details.

## v1.2.2 / 2015-04-28

* license comment updates to simiplify certain build scenarios

## v1.2.1 / 2015-04-22

* added safe exporting for requireJS usage
* clarified Bower usage and instructions

## v1.2.0 / 2015-03-17

* added comprehensive support for array arguments, including nested arrays
* simplified code slightly

## Previous

Please see the git history for the details of previous versions.
