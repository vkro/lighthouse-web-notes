# Notes for Week 1, Day 4

**Focus: Callback Functions**

## What is a callback function?
Function that gets passed to another function (to be invoked by that other function).

## What is an arrow function?

It's just cleaner.
```javascript
const sayHello = function(name {
  console.log(name);
})
```
=== _same as_ ===
```javascript
const sayHello = (name) => {
  console.log(name);
```
_If you use `this` in an arrow function that's inside an object (a method), `this` will refer to the object the function's called within._

>**Note:**
Every function in JavaScript has a return value. If you don't explicitly return something, there is an implicity return value of `undefined`.

>**Note:**
You can use `const` for arrays and objects, it still lets you change the contents of those objects (ie. pushing to an array, changing or adding properties to an object.)

>**Tip:**
Use [pythontutor.com/javascript](http://pythontutor.com/javascript.html#mode=edit) - it'll walk you through your code step by step.
