---
layout: page
order: 8
title: Writing functions
---

Functions are collections of **statements** that are grouped together and (optionally) have a name that we can use to **call** that function.

{% panopto "ac7826c7-c45d-47eb-b2f3-ac7200cf8604" %}

We can define functions in a couple of different ways

## Functions as variables

We can define a function and refer to that function using a variable

```js
let minus = function (x) {
    return -x;
};
```

This is a JavaScript statement like any other (note the `;` at the end of the function declaration) but rather than storing a value in the variable we are defining and storing a function.

We tell JavaScript we are defining a function using the `function` keyword. This is followed by any **parameters** (or **arguments**) that the function will accept as input. There is then a code block (`{ ... }`) inside which we find the body of the function - the code that is executed each time the function is **called**. This function has a `return` statement which allows us to send a value back out of the function to the code that originally called it. This is optional. A function with no `return` statement will return `undefined`.

## Function declarations

We can define and name functions without storing them in a variable:

```js
function minus(x) {
    return -x;
}
```

Note the lack of the `;` on the end of the declaration in this case. Functions declared in this way are available everywhere inside the **scope** in which they are declared - even **before** their definition. This is just one of the ways in which JavaScript is particularly hostile to new programmers. It's probably best if you don't worry about it for now.

## Arrow notation

This is a relatively new addition to the language which manages to both simplify and complicate writing functions at the same time.

```js
let minus = (x) => {
    return -x;
};
```

The fundamental difference here is that the `function` keyword **before** the parameters of the function has been replaced by the `=>` operator **after** the parameter list. These functions can be simplified further. Where there is only one parameter we can omit the `()` around the parameter list:

```js
let minus = (x) => {
    return -x;
};
```

We can simplify even further: where there is just a return statement in the body of the function we can omit the `{ ... }` and the `return` statement itself:

```js
let minus = (x) => -x;
```

This is clearly **less** code but I'll leave it down to your judgement whether it is necessarily **simpler** code, particularly for a newcomer to the language. There is little doubt that arrow functions are cooler than other function declarations, and once you are used to JavaScript you'll probably use them all the time. For now though, you may want to forget about them.

## Parameters

JavaScript is very flexible with parameters. You can call a function and give it more input parameters than it usually accepts according to it's definition, and JavaScript will ignore any parameters it doesn't need.

```js
let minus = function (x) {
    return -x;
};

console.log(minus(3, "test", false));
```

You can call a function with fewer input parameters than it usually expects, and JavaScript will give the value `undefined` to any parameters that are not supplied as input values.

## Demonstration

{% panopto "8a689d66-a83c-430c-a42a-ac7200d011dd" %}

## Code examples

There are a set of code examples that accompany this course showing the use of JavaScript. (Right click and open in a new window/tab) if you're viewing this on Learning Central.

-   Variable Types [[HTML]](https://github.com/martinjc/introduction-to-js/examples/blob/master/basic-js/types.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/types.html)
-   Numerical Operators [[HTML]](https://github.com/martinjc/introduction-to-js/examples/blob/master/basic-js/numbers.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/numbers.html)
-   Booleans [[HTML]](https://github.com/martinjc/introduction-to-js/examples/blob/master/basic-js/booleans.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/booleans.html)
-   Looping [[HTML]](https://github.com/martinjc/introduction-to-js/examples/blob/master/basic-js/looping.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/looping.html)
-   Functions
    -   Function 1 [[HTML]](https://github.com/martinjc/introduction-to-js/examples/blob/master/basic-js/functions1.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/functions1.html)
    -   Function 2 [[HTML]](https://github.com/martinjc/introduction-to-js/examples/blob/master/basic-js/functions2.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/functions2.html)
    -   Function 3 [[HTML]](https://github.com/martinjc/introduction-to-js/examples/blob/master/basic-js/functions3.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/functions3.html)
    -   Arrow Functions [[HTML]](https://github.com/martinjc/introduction-to-js/examples/blob/master/basic-js/arrow-functions.html) [[Demo]](https://martinjc.github.io/introduction-to-js/examples/basic-js/arrow-functions.html)
