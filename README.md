# ES6-Cool-Features-
Some cool stuff about ES6

## Arrow Functions (Abimbola Aderoju)
Arrow functions are a brand new feature in ECMAScript 2015 (ES6). Thay serve two main purposes: more concise syntax and sharing lexical this with the parent scope.


### Expression Bodies 
Read official documentation on [ES6: Expression Bodies](http://es6-features.org/#ExpressionBodies)

Below is a code snippet with expression bodies


```
odds  = evens.map(v => v + 1)
pairs = evens.map(v => ({ even: v, odd: v + 1 }))
nums  = evens.map((v, i) => v + i)

```

### Statement Bodies
Read official documentation on [ES6: Statement Bodies](http://es6-features.org/#StatementBodies)

Below is a code snippet with statement bodies



```
nums.forEach(v => {
   if (v % 5 === 0)
       fives.push(v)
})

```
