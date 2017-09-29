Welcome Back

<small>Let's review some of the things we learned last week</small>

---

Git 

----

```bash
$ git commit
```

----

```bash
git checkout 
```

----

```bash
git checkout -b name
```

----

```bash
git merge aBranch
```

---

Javascript Basics 

----

Variables 

```javascript
var foo = 'a string';

var bar = 10;

var truString = 'true'
var truBool = true

```

----

Maths 

```
addition: +
subtraction: -
multiplication: *
division: /
```

----


Functions 

```js
function sample(args) {
  return args
}

sample(true)
sample('true')
```

----


Boolean Logic 

```js
10 > 9
10 > 10 
5 == 5
5 != 5
```

----

Conditionals

```js
var x;
if(true) {
  x = 0
} else {
  x = 1
}
```

----

Comments:

```js
function sample(args) {
  // comment
}
```

---

Prelude to today's class:

The modulo operation `%` returns the remainder of a division operation.

```
5 % 5 = 0
5 % 3 = 2 
5 % 2 = 3 
5 % 6 = 6 
```

---

There are also two other operations that allow us to increment or decrement a value 

```
x++
x-- 
```

this is roughly equal to 
```
x = x + 1
x = x - 1
```


---

Let's talk about truth

----

Prelude:

Aside from numbers, booleans, and strings there are two more types that we need to be familiar with today.



```
var a = null
var b = undefined
```

----

Different literals can have different levels of truthiness. 

```js
true === true
"true" == true
"" == false
1 == true 
0 == false 
```

----

This means that we can use non-boolean values inside conditionals

```js
if(1) {
  alert(1)
} else {
  alert 0
}
```

```js
var tru = ""
if(tru) {
  alert(1)
} else {
  alert(1)
}
```

---

Exercise! 

Write a function that takes a `string`.
If the string is blank, return `"Oh No!"`
If the string is not blank, return the same string five times 

Example 

```js
fiveStrings("Tony!") // returns Tony!Tony!Tony!Tony!Tony!
fiveStrings("") // returns "Oh No!
```

----

Exercise 2:

Write a function that takes a number. 
If the number is even, return `true`
If the number is not even, return `false`

example


```js
isEven(12) // true
isEven(5) // false
```

---

```
if(x > 0) {
  return 'Positive'
} else if ( x < 0) {
  return 'Negative
} else {
  return 'Zero'
}
```

---

if x is divisible by 5 return 'fizz' 
if x is divisible by 3 return 'buzz'
if x is divisible by neither 3 or 5 return 'buzzfizz'

---

Combined Logic 

Logic in `if` statements can be "combined" together using logical operators.
There are two that we use in javascript 

```
&& // and 
|| // or 
```

---

For example 

```
if(x > 0 && x < 10) {
  return 'x is between 0 and 10'
} else {
  return 'This number is not between x 
}
```

---

A variation of the previous exercise 

if x is divisible by 5 return 'fizz' 

if x is divisible by 3 return 'buzz'


if x is divisible by 3 AND 5 return 'fizzbuzz'

---

Loops!

----

Loops are a way for us to do the same thing over and over again.


----

There are two ways in which we can do that


----


```
while(true) {
  // do something
}

```

----

```
for(var i = 0; i < 10; i++) {

}
```


