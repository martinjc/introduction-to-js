---
layout: page
order: 5
title: Using functions
---

Functions are collections of **statements** that are grouped together and (optionally) have a name that we can use to **call** that function.

We've already used a few different functions. For instance `console.log` is a function. We **call** a function, which asks JavaScript to execute the statements within the function

Functions can accept input **arguments**, though not all functions require them.

If we use a function name without the `( ... )` we are referring to the function itself, if we add the `( ... )` then the function will be executed (or **called**).

## Math

JavaScript has a `Math` object that contains a number of functions useful for doing ... well, maths. You can see the full list of these functions in the [`Math` documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math).

For example, calling `Math.floor(x)` and passing in a floating point number `x` will return the largest integer less than or equal to `x`.

```js
// will return 3
Math.floor(3.2);

// will return 6
Math.floor(6.9);

// will return NaN
Math.floor();

// is a function
Math.floor;
```
