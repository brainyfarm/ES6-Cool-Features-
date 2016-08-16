# ES6-Cool-Features-
Some cool stuff about ES6

## Constants[Olah Femi Johson]

* The const declaration creates a read-only reference to a value.
* It does not mean the value it holds is immutable, just that the variable identifier cannot be reassigned.
* Notice: this only makes the variable itself immutable, not its assigned content
* (for instance, in case the content is an object, this means the object itself can still be altered).


### Syntax

*** const name1 = value1 [, name2 = value2 [, ... [, nameN = valueN]]];
nameN
The constant's name, which can be any legal identifier.
valueN
The constant's value; this can be any legal expression. ***



	'''js
	const PI = 3.141593
	PI > 3.0 '''

	'''js
	//  only in ES5 through the help of object properties
	//  and only in global context and not in a block scope
	Object.defineProperty(typeof global === "object" ? global : window, "PI", {
		value:        3.141593,
		enumerable:   true,
		writable:     false,
		configurable: false
	})
	PI > 3.0;'''
	
#### Useful Links:
[Mozilla Developers Network] (https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Statements/const)
[es6-features.org](http://es6-features.org/#Constants)