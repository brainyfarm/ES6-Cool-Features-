# ES6 COOL FEATURES

## Constants (Olah Femi Johson)
=======

The const declaration creates a read-only reference to a value.
It does not mean the value it holds is immutable, just that the variable identifier cannot be reassigned.

Notice: this only makes the variable itself immutable, not its assigned content
(for instance, in case the content is an object, this means the object itself can still be altered).


### Syntax

	const name1 = value1 [, name2 = value2 [, ... [, nameN = valueN]]];
	nameN
	The constant's name, which can be any legal identifier.
	valueN
	The constant's value; this can be any legal expression.



```js
const PI = 3.141593
PI > 3.0 
```

```js
//  only in ES5 through the help of object properties
//  and only in global context and not in a block scope
Object.defineProperty(typeof global === "object" ? global : window, "PI", {
	value:        3.141593,
	enumerable:   true,
	writable:     false,
	configurable: false
 })
PI > 3.0;
```
	
#### Useful Links:
[Mozilla Developers Network](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Statements/const), [es6-features.org](http://es6-features.org/#Constants)

=======
=======


## Iteration Protocols (Adedeji Jolaoluwa)
=======

Definition-The iterable protocol allows JavaScript objects to define or customize their iteration behavior, such as what values are looped over in a for..of construct.It defines a standard way to produce a sequence of values (either finite or infinite).

* Examples

```js
var iterator = someString[Symbol.iterator]();
iterator + "";    // "[object String Iterator]"
 
iterator.next();  // { value: "h", done: false }
iterator.next();  // { value: "i", done: false }
iterator.next();  // { value: undefined, done: true }

```

Read official documentation on [Mozilla Developer Network: Iteration Protocol](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Iteration_protocols)

=======
=======



## Arrow Functions (Abimbola Aderoju)
=======
Arrow functions are a brand new feature in ECMAScript 2015 (ES6). Thay serve two main purposes: more concise syntax and sharing lexical this with the parent scope.


### Expression Bodies 
Read official documentation on [ES6: Expression Bodies](http://es6-features.org/#ExpressionBodies)

Below is a code snippet with expression bodies


```js
odds  = evens.map(v => v + 1)
pairs = evens.map(v => ({ even: v, odd: v + 1 }))
nums  = evens.map((v, i) => v + i)

```

### Statement Bodies
Read official documentation on [ES6: Statement Bodies](http://es6-features.org/#StatementBodies)

Below is a code snippet with statement bodies



```js
nums.forEach(v => {
   if (v % 5 === 0)
       fives.push(v)
})

```

## Extended Parameter Handling (Arigbeta Kessy)
=======

These features are added on ES-6.Simple and intuitive default values for function parameters. Parameter handling has been significantly upgraded in ECMAScript 6.

It now supports parameter:

*default values
*Rest parameters (varargs).
*Named parameters via destructuring.

###Default parameter values:

* Example.

```js
function findClosestShape(x=0, y=0) {
    // ...
}
```
Read official documentation on[Exploring JS: ES6- Features](http://es6-features.org/#DefaultParameterValues)


### Rest parameters:
* Examples:

```js
function format(pattern, ...params) {
    return params;
}
console.log(format('a', 'b', 'c')); // ['b', 'c']
```
Read official documentation on[Exploring JS: ES6-Features](http://es6-features.org/#RestParameter)

### Named parameters via destructuring:
* Example:

```
function selectEntries({ start=0, end=-1, step=1 } = {}) {
    // The object pattern is an abbreviation of:
    // { start: start=0, end: end=-1, step: step=1 }

    // Use the variables `start`, `end` and `step` here
    
}
```
Read official documentation on [Exploring JS: Parameter Handling](http://exploringjs.com/es6/ch_parameter-handling.html)

=======
=======



## Class Declaration (Olawale Akinseye)
=======

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

=======
=======