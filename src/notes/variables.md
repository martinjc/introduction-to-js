---
layout: page
order: 1
title: Variables and Operators
---

{% panopto "207fb300-a452-4db0-92a7-ac680183632b" %}

## Declaring variables

There are three different keywords that allow us to declare variables in JavaScript:

-   `var`
-   `let`
-   `const`

### `var`

`var` allows us to declare a variable. This variable's value and type can be changed after assignment. The **scope** of the variable is not restricted to the local block

```js
var a = 6;
var myName = "martin";
```

### `let`

`let` allows us to declare a variable. This variable's value and type can be changed after assignment. The **scope** of the variable is limited to the block in which it is declared

```js
let a = 6;
let myName = "martin";
```

### `const`

`const` allows us to declare a **constant** variable. The value of this variable cannot be changed once assigned (this is sometimes referred to as being **immutable**)

```js
const PI = 3.14;
const myName = "Martin";
```

## Naming variables

Variable names must start with a letter, an underscore (\_) or a dollar sign (\$). We normally useCamelCase for naming variables in JavaScript (as opposed to Python where snake_case_is_more_common). We cannot use [reserved words](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar) for variable names.

## Scope

The **scope** of a variable refers to the regions of code in which a variable is valid - the places in the code where the variable exists and can be read from or assigned to. If a variable is out of scope then it cannot be used; if it is in scope then we can refer to it by name and access the value it contains.

In this example, `myName` is out of scope when it is used by `console.log`, as it is declared using `let` so is only valid inside the block of code where it is declared.

```js
if (true) {
    let myName = "Martin";
}

// will throw a ReferenceError because myName is out of scope
console.log(myName);
```

In this example, `myName` is in scope when it is used by `console.log`, as it is declared using `var` so it is valid both inside and outside the block of code where it is declared.

```js
if (true) {
    var myName = "Martin";
}

// will throw a ReferenceError because myName is out of scope
console.log(myName);
```

## Data types in JavaScript

-   boolean: `true` and `false`
-   `null`; a special value for nothing
-   `undefined` for when something exists but has not had a value assigned
-   Number - an integer (whole number) or floating point (decimal) number
-   String - a sequence of characters

### Typing

JavaScript is dynamically typed and weakly typed. We do not need to tell JS what type a variable will be when we declare it, and we can change the type of data stored in a variable once it has been declared. JavaScript will convert types as it needs to during script execution.

## Operators

-   Arithmetic operators: `+`, `-`, `/`, `*`, `%`, `**`
-   Relational operators: `<`, `>`, `<=`, `>=`
-   Equality operators: `==`, `!=`, `===`, `!==`
-   Logical operators: `&&`, `||`, `!`
-   Increment/Decrement: `++`, `--`

## Equality

JavaScript has two ways of comparing equality, `==` and `===`.

`==` and `!=` only consider value

`===` and `!==` consider both value and type
