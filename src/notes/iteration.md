---
layout: page
order: 3
title: Iteration
---

There are a number of different ways to loop or iterate in JavaScript: `for`, `while`, `do ... while`

## For Loops

{% panopto "3aea16ee-b8bc-4ef6-a0a4-ac6801836233" %}

A `for` loop has the following general structure:

```js
for (initialisation; condition; final - expression) {
    // ... code to execute on each iteration
}
```

-   The **initialisation** is where we set up the variable used in iteration (a counter for instance)
-   The **condition** is the boolean expression we check on each iteration to check whether the loop should continue
-   The **final-expression** is code that is always executed last of all on each iteration (usually to increment/decrement the counter)

```js
for (let i = 0; i < 10; i++) {
    console.log(i);
}
```

## While loops

{% panopto "d5fb2e60-8ba3-49ec-bd7b-ac7200cf8592" %}

A `while` loop has the following general structure:

```js
while(boolean condition) {
    //  ... code to execute on each iteration
}
```

The block of code within the loop will be run while the boolean condition evaluates to `true`. It is very easy to cause an **infinite loop** with a while loop as you can easily forget to ensure that the boolean condition will change at some point.

### `break`

We can use the `break` keyword to exit a loop

```js
for (let i = 0; i < 10; i++) {
    console.log(i);
    if (i > 5) {
        break;
    }
}
```

### `continue`

We can use the `continue` keyword to stop the current iteration and skip to the next

```js
for (let i = 0; i < 10; i++) {
    if (i % 2 === 0) {
        continue;
    }
    console.log(i);
}
```

## Code examples

There are a set of code examples that accompany this course showing the use of JavaScript. (Right click and open in a new window/tab) if you're viewing this on Learning Central.

-   Variable Types [[HTML]](https://github.com/martinjc/introduction-to-js/blob/main/src/examples/basic-js/types.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/types.html)
-   Numerical Operators [[HTML]](https://github.com/martinjc/introduction-to-js/blob/main/src/examples/basic-js/numbers.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/numbers.html)
-   Booleans [[HTML]](https://github.com/martinjc/introduction-to-js/blob/main/src/examples/basic-js/booleans.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/booleans.html)
-   Looping [[HTML]](https://github.com/martinjc/introduction-to-js/blob/main/src/examples/basic-js/looping.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/looping.html)
