---
layout: page
order: 7
title: Strings
---

Strings in JavaScript are sequences of text characters, contained within `'`, `"` or `` ` `` characters.

{% panopto "ee5e116c-4408-4c11-9a84-ac7200cf85cf" %}

We can use any of the three quotes (single, double or backtick) to define Strings, but we must **start** and **end** using the same character

```js
let myName = "Martin";

let myName = "Martin";

let myName = `Martin`;
```

## Special characters

We can include special characters in JavaScript Strings by escaping them using the `\` character. `\n` adds a new line. `\t` adds a tab. `\\` adds a `\`.

```js
let myText = ‘This is one line\nThis is another’;

let myText = “\tThis is indented”;

let myText = “We can escape \” too”;

```

## String concatentation

We can use the `+` operator to join Strings together

```js
let myText = "Hello" + " " + "World!";
```

## Template literals

Strings defined using `` ` `` characters (backticks) are template literals. These are special as we can embed expressions within them.

```js
let numChildren = 2;
let tirednessAmount = "very";
let myText = `Martin has ${numChildren} children, which explains why Martin is ${tirednessAmount} tired`;
```

These expressions can be simple usage of variables, as above, or we can even carry out operations within our `${ ... }` literals:

```js
let bigOneAge = 5;
let thisYear = 2020;
let myText = `Martin's eldest child is ${bigOneAge} so Martin has been tired since ${thisYear - bigOneAge}`;
```

## String Objects

Strings are actually a type of **Object**. Objects are more complicated data types in JavaScript that we aren't going to worry about yet. All we need to know about them is that they have **properties** that tell us more about them, and **methods** which are functions that work on the Object itself...

Strings have a **length** property that tells us how long the String is:

```js
let myText = "When, in disgrace with fortune and men’s eyes,\nI all alone beweep my outcast state,";
console.log(`myText length: ${myText.length}`);
```

Strings have [a lot of different methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) that we can use to alter, search, replace or do other things with:

```js
let m = ‘The quick brown fox …’
console.log(m.toUpperCase());
console.log(m.replace(“fox”, “cat”));
console.log(m.slice(4, 8));
```

## String demo

{% panopto "2fe5a51a-ede3-4e75-8e00-ac7200cfc709" %}
