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
  var x = 0
} else {
  var x = 1
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

Today's topic: 

Truthiness 

----

Prelude:

Aside from numbers, booleans, and strings there are two more types that we need to be familiar with today.

```

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

----

