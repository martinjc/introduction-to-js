---
layout: page
order: 2
title: Branching and Boolean Expressions
---

{% panopto "a0538af8-b1e3-4bb6-9730-adc101287067" %}

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

## Code examples

There are a set of code examples that accompany this course showing the use of JavaScript. (Right click and open in a new window/tab) if you're viewing this on Learning Central.

-   Variable Types [[HTML]](https://github.com/martinjc/introduction-to-js/blob/main/src/examples/basic-js/types.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/types.html)
-   Numerical Operators [[HTML]](https://github.com/martinjc/introduction-to-js/blob/main/src/examples/basic-js/numbers.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/numbers.html)
-   Booleans [[HTML]](https://github.com/martinjc/introduction-to-js/blob/main/src/examples/basic-js/booleans.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/booleans.html)
