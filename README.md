# ES6-Cool-Features-
Some cool stuff about ES6


## Iteration Protocols(ADEDEJI JOLAOLUWA)

Definition-The iterable protocol allows JavaScript objects to define or customize their iteration behavior, such as what values are looped over in a for..of construct.It defines a standard way to produce a sequence of values (either finite or infinite).

* Examples

```js
var iterator = someString[Symbol.iterator]();
iterator + "";    // "[object String Iterator]"
 
iterator.next();  // { value: "h", done: false }
iterator.next();  // { value: "i", done: false }
iterator.next();  // { value: undefined, done: true }

```

Read official documentation on [Mozilla Developer Network: Iteration Protocol] (https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Iteration_protocols)

