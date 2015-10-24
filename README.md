# Many Examples Project

For one topic, provide many examples so that future developers can read a stuff and master fast.

I want to make this documentation such that when you take one topic and go through all example and possible scenarios, you will almost get the Ninja Capability in that one topic atleast for a good amount of time.

Inspired By: https://www.youtube.com/watch?v=FKTxC9pl-WM

##JavaScript

###Topic: IIFE

###Topic: Closures

###Topic: Prototypal Inheritance

###Topic: Functional Programming

###Topic: Weird Parts Of JavaScript | What to avoid!

###Topic: Inbuilt Helpful Functions

##D3.js

###Using Modernizr.

Detect if browser supports SVG or not then display

```
<script src="js/modernizr.js"></script>
<script>

Modernizr.load({
  //This will test if 'svg' and 'inlinesvg' are valid in browser or not.
  test: Modernizr.svg && Modernizr.inlinesvg,
  //This will include 'd3.v3.min.js' and 'script.js' if the test above passed.
  yep: ['js/d3.v3.min.js','js/script.js']
});

</script>
```
