# Notes for Week 1, Day 3

**Focus: JavaScript Data Types**

## The 6 Primitive Data Types in JavaScript
1. `undefined`
2. `null`
3. `boolean`
4. `string`
5. `number`
6. `symbol` (*Introduced in ES6 an not something we need to focus on right now*)

**Objects Are Not Primitives**

Anything not in the above list is an Object. Together, the six primitive types, plus `object`, make up the **seven fundamental types of JavaScript**.

*Note:* Arrays and functions are technically sub-categories of objects.

## Object Literals

- string literal: "lighthouse", "labs"
- number literals: 5, 7.5
- array literal [1, 2, 3]

Objects have a literal syntax using braces `{}`

Object literal assigned to a variable:
```javascript
const emptyObject = {};
```
Object literal with a single key-value pair:
```javascript
const tinyObject = {size: 'Tiny'};
```

## Object Key Rules:

1. Keys are always strings.
2. Each key is unique (can only occur once in the object).
3. Each key is associated with exactly one value. _Arrays and objects count as one value, even though they contain other values_

## Notes from Today's Lecture

> **VSCODE Tip**: hold down _option_ to drop as many cursors as you want

### Array stuff

`for ... of` will get you the content of the array

`for ... in` will get you the indices. It's like a cleaner version of the for C-style loop (`for (let i = 0; i < ...)`)

> [Here](https://stackoverflow.com/questions/5263847/javascript-loops-for-in-vs-for) is an informative discussion on Stack Overflow about `for` vs. `for...in` Javascript loops 

### Object stuff

Nima says: 
> For accessing object values, square bracket syntax is the only good syntax. Dot syntax is annoying. Stick with square brackets and strings.

**How do you loop through an object?**

Only way to do it is use a `for...in` loop.

Example:
```javascript
for (let key in obj) {
  console.log(key); 
  console.log(obj[key]);
}
```

**Another thing to explore:** this 