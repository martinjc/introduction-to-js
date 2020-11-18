---
layout: page
order: 9
title: "Week 4 Exercise: JavaScript Problem Solving"
---

## Reading files

To solve some of these exercises you will need to read a file. When JavaScript runs in the web browser this is usually not possible - JavaScript is **sandboxed** away from the file system of the machine on which the web browser is running. However, when we run JavaScript on the command line using node we can access the file system using the `fs` module. We need to `require` this module, which tells node to load the library and make it available to our code.

So, for example, to read the contents of a text file `hello.txt` into a variable `data`

```js
const fs = require("fs");

const data = fs.readFileSync("hello.txt", "utf8");
console.log(data);
```

We'll talk more about file access in node (and some better ways to do it) later in the course. For now though, this will do.

## Exercises

1. Write JavaScript code that finds all the words in [words.txt](/examples/words.txt) with three consecutive double letters.

2. Write JavaScript code that finds the longest common prefix string amongst a given array of strings. Return false If there is no common prefix. For Example, the longest common prefix of "abcdefgh" and "abcefgh" is "abc".

3. Write JavaScript code to check whether a given number is Oddish or Evenish. A number is called "Oddish" if the sum of all of its digits is odd, and a number is called "Evenish" if the sum of all of its digits is even.
