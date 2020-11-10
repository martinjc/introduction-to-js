---
layout: page
order: 2
title: Branching and Boolean Expressions
---

{% panopto "66f34584-6b61-46d2-9219-ac68018361c5" %}

## Branching - `if`, `else if`, `else`

We can use `if`, `else if` and `else` in JavaScript. Each `if` statement will check whether a given condition (`boolean` expression) is true or false. If true, it will execute the block of code it contains. If false it will skip over the block to the next section of code.

```js
if (true) {
    let myName = "martin";
}
```

```js
let x = 6;
if (x % 2 === 0) {
    console.log("X is even");
} else {
    console.log("X is odd");
}
```

## `false`

Almost everything is `true` in JavaScript, except for:

-   `false`
-   `''`
-   `0`
-   `undefined`
-   `null`
