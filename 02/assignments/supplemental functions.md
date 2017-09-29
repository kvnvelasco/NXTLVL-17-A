## Describe the functions

Listed below are 5 functions that perform a variety of tasks. 

Your assignment is to translate these functions into english (or tagalog). You must describe every possible output of a function given it's input. 

For example:

Function: 

```js
function add(a, b) {
  return a + b
}
```

Answer:

The function add takes two numbers and returns their sum.


### 1

```js
function divide(a, b) {
  if(b < 0)
    return a / b
  else 
    return 0
}
```
### 2
```js
  function divisibleBy2(a) {
    return a%2 == 0
  }

```
### 3 
```js 
  function largerNum(a, b) {
    if(a > b) {
      return a
    }      
    else {
      return b
    }
  }
```

### 4
```js
  function sumOfEvens(l) {
    var sum = 0 
    var current = 0
    while(current < l) {
      if(current%2 == 0) {
        sum = sum + current
      }      
      current = current + 1
    }
    return sum
  }
```

### 5

```js
function sayManyTimes(word, times) {
  var str = ""
  var num = 0
  while(num < times) {
    str = str + word
    num = num + 1
  }
  return str
}
``` 