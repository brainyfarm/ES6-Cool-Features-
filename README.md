<<<<<<< HEAD
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
=======
# ES6 Cool Features
A documentation of some ES6 cool new awesome features



## Class Declaration (Olawale Akinseye)

Javascript is now more powerful as classes has now been intoduced into the language.

Below is a simple documentation on how to declare and use a basic class.


```js
class name  {
  	// class body
	}

```

**For inheritance, Use the code below**

```js
class name extends class2 {
  	// class body
	}
```

Read official documentation on [Mozilla Developer Network: Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/class)

>>>>>>> 9c35ff029bc8482b71ac223a16e1ae0d8c825083
