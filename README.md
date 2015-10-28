# Many Examples Project

For one topic, provide many examples so that future developers can read a stuff and master fast.

I want to make this documentation such that when you take one topic and go through all example and possible scenarios, you will almost get the Ninja Capability in that one topic atleast for a good amount of time.

Inspired By: https://www.youtube.com/watch?v=FKTxC9pl-WM

##JavaScript

###Topic: Primitive v/s Reference Values

Objects pass values by reference vs Primitives (```undefined, Null, Boolean, Number, and String```) pass values by copying.

Pass values by copy example:

```
  var a = "String";
  var b = a;
  
  /*Modifying values of 'a'*/
  
  a = "anotherString";
  
  /*Checking b's value*/
  
  console.log(b); /*will give out 'String', because 'b' copied the value of 'a' and stored seperately*/
```

Pass values by reference example:

``` 
  var obj1 = { "id" : "goku_vegeta" };
  var obj2 = obj1;
  
  /* Modifying values of obj1.id */
  
  obj1.id = "gohan_trunks";
  
  /*Checking values of obj2 */
  
  console.log(obj2);
  
  /*Will print : Object { "id" : "gohan_trunks"} */
  
  /*Also adding/deleting properties will be reflected into obj2, because they both are pointing to the same object in the memory*/
  
  obj1.foo = "bar";
  
  console.log(obj2);
  
  /*Will print : Object { "id" : "gohan_trunks", "foo": "bar"} */
  
```

###Topic: IIFE

###Topic: Closures

###Topic: Prototypal Inheritance

###Topic: Functional Programming

###Topic: Weird Parts Of JavaScript | What to avoid!

###Topic: Inbuilt Helpful Functions

###Topic: Dates

```Date.now() ``` was introduced in ES5 which will return millisecond representation of time right now. The browsers which have not yet implemented ```Date.now()``` can use it in following way:

```var nowMs = +new Date()```

##D3.js

###Using Modernizr.

Detect if browser supports SVG or not then display

```
<script src="js/modernizr.js"></script>
<script>

Modernizr.load({

  /*This will test if 'svg' and 'inlinesvg' are valid in browser or not.*/
  test: Modernizr.svg && Modernizr.inlinesvg,
  
  /*This will include 'd3.v3.min.js' and 'script.js' if the test above passed.*/
  yep: ['js/d3.v3.min.js','js/script.js']
  
});

</script>
```
