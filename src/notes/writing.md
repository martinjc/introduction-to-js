---
layout: page
order: 4
title: Writing JavaScript
---

Here's a demo of writing and running some JavaScript code. The [example code from the video is attached here]({{"/examples/js-examples.zip" | url}}).

{% panopto "63c29b07-0151-444e-bdeb-ac690157a145" %}

We can use `node` to run files containing JavaScript code on the command line.

So, for example, a basic `helloworld.js` containing:

```js
console.log("hello world!");
```

can be run like so:

<div id="termynal" data-termynal data-ty-typeDelay="40" data-ty-lineDelay="700">
    <span data-ty="input">ls</span>
    <span data-ty>helloworld.js</span>
    <span data-ty="input">node helloworld.js</span>
    <span data-ty>hello world!</span>
</div>

<script>
</script>
