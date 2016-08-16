# ES6-Cool-Features-
Some cool stuff about ES6
##Extended Parameter Handling (Arigbeta Kessy)

Thesde features are added on ES-6.Simple and intuitive default values for function parameters. Parameter handling has been significantly upgraded in ECMAScript 6.

It now supports parameter:

*default values
*Rest parameters (varargs).
*Named parameters via destructuring.

###Default parameter values:

Example.
```js
function findClosestShape(x=0, y=0) {
    // ...
}
```
Read official documentation on[Exploring JS: ES6- Features](http://es6-features.org/#DefaultParameterValues)


###Rest parameters:
Examples:
```js
function format(pattern, ...params) {
    return params;
}
console.log(format('a', 'b', 'c')); // ['b', 'c']
```
Read official documentation on[Exploring JS: ES6-Features](http://es6-features.org/#RestParameter)

###Named parameters via destructuring:

Example:
```
function selectEntries({ start=0, end=-1, step=1 } = {}) {
    // The object pattern is an abbreviation of:
    // { start: start=0, end: end=-1, step: step=1 }

    // Use the variables `start`, `end` and `step` here
    
}
```
Read official documentation on [Exploring JS: Parameter Handling](http://exploringjs.com/es6/ch_parameter-handling.html)
