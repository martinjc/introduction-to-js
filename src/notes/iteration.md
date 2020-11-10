---
layout: page
order: 3
title: Iteration
---

There are a number of different ways to loop or iterate in JavaScript: `for`, `while`, `do ... while`

## For Loops

{% panopto "3aea16ee-b8bc-4ef6-a0a4-ac6801836233" %}

A for loop has the following general structure:

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
