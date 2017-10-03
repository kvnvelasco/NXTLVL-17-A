Welcome Back! 

<small>
  We've been doing a lot the last week, 
  so we're going to go a bit slower today
</small>

---

Today we're going to talk about HTML and CSS

---

Javascript allows us to add functionality and interactivity to 
HTML

---

HTML is a **markup language** 

<small>this means that it's used to create layouts and views</small>

---

Building blocks

----


An HTML tag is the smallest logical unit of HTML. It looks like this

```
<html></html>
```

The text between the `<` `>` is the *name* of the tag

```
<name attribute="value">
  <child attribute="value"> 
    text
  </child>
</name>
```

A tag can also contain attributes and children


---


This is the basic structure of an html document 

```
<html> 
  <head>
    <title> Page Title </title>
  </head>
  <body>
    Hello world!
  </body>
</html>
```

---

I've sent you all a cheatsheet on slack with a bunch of tags and what they do. 


---

First Exercise 

---

CSS

---


Remember those id and class attributes that we saw earlier? 

Those are used for a variety of things, but one of them is for styling.

---

CSS is placed inside a `<style>` tag inside the `<head>` of a document and has the following pattern


```

.className {
  color: green
  background: blue
  width: 300px
  height: 200px
  margin: 20px;
  padding: 20px;
}

#id {
  color: green
  background: blue
  width: 300px
  height: 200px
  margin: 20px;
  padding: 20px;
}

```


---

Specific CSS selection 

```
.parent .child div {
  color: green
}
```

```html
<div class="parent">
  <div class="child">
    <div> 
     This is the selected div
    </div>
  </div>
</div>
```

---

The CSS Box model 

![](https://www.kasandbox.org/programming-images/misc/boxmodel.png)


---

