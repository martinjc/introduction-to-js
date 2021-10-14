---
layout: page
order: 4
title: Writing JavaScript
---

Here's a demo of writing and running some JavaScript code. The [example code from the video is attached here]({{"/examples/js-examples.zip" | url}}).

{% panopto "674e820e-7111-4bd9-b79f-adc1012b2fb9" %}

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
