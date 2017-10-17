# Where can I access a variable? 

Over the last 6 sessions we've been creating functions that modify variables that have been declared outside them. 

```js
var array = []

function addToArray(x) {
  array.push(x)
}
```

This is a demonstration of `lexical scope`. 

At it simplest, lexical scope is a property of a programming language that allows functions to access 
variables that are declared in the same `scope` or in a parent `scope`.

A scope is the area in which the language can search for the definition for a variable when attempting to access it's value.

```js
// We are at the root of a document (also known as the global scope)

// We declare a variable in the global scope 
var foo = 3

// we declare a function. This creates a new scope inside the function 
function fun(a) {
  // This is now a new function scope. If we declare variables here, they will not be accessible outside this function
  var insideOnly = true 
  
  // but we can access variables that belong to the parent scope 
  console.log(foo) // this will output 3 
  
  // if we declare a new variable that has the same name as a variable in the parent scope, it takes precedence
  var foo = 1
  console.log(foo) // this will output 1
}

// we cannot access variables delcared inside functions outside of them
console.log(insideOnly) // throws an error
```

Whenever we use a variable, the javascript engine has to search for that variable in memory. The space it is allowed to search in is called `scope`

Lexical scope means that the scope of of a variable is defined at the time in which the code is 
written (`lexically`) as opposed to the time it is run.

No matter where or when a function is run, it wil always have access to the variables within its lexical scope. 

in our first example,

```js
var array = []

function addToArray(x) {
  array.push(x)
}
```



the function addToArray will always have access to the `array` variable even if we call it from other functions. 
Even if the function declares a conflicting variable within it's own scope.


```js
var array = []

function addToArray(x) {
  array.push(x)
}

function addData(x) {
   // ... do something
   var array = [1, 2, 3, 4]
   addToArray(x) // add something to the parent array not to [1,2,3,4]
}
```

TL;DR: Javascript will look for the value of a variable in the location accessible to where the function was `defined` not where it was called.






