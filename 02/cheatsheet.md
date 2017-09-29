# Javascript syntax cheatsheet

## Variables 

```javascript
var foo = 'a string';

var bar = 10;

var truString = 'true'
var truBool = true
```

## Maths 

```
addition: +
subtraction: -
multiplication: *
division: /
```

## Functions 

```js
function sample(args) {
  return args
}

sample(true)
sample('true')
```


## Boolean Logic 

```js
10 > 9
10 > 10 
5 == 5
5 != 5
```


## Conditionals

```js
var x;
if(true) {
  x = 0
} else {
  x = 1
}

if(x > 0) {
  // do something positive
} else if (x < 0) {
  // do something negative
} else {
  // do something if x is neither positive nor negative (i.e. zero)
}
```

## Loops 

```js 
var x = 0
while(x < 1000) {
  // do something while x is less than 1000
  x = x + 1
}

