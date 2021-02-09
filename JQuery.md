```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
    <script src="https://code.jquery.com/jquery-3.1.1.js"></script>
  </head>
  <body></body>
</html>
```

```js
// Ready function runs once HTML doc is done loading
$(document).ready(function () {
  // jQuery code goes here
});

//or

$(function () {
  // jQuery code goes here
});
```

##Example below of how to change html _Start_ to _Go_

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
    <script src="https://code.jquery.com/jquery-3.1.1.js"></script>
  </head>
  <body>
    <div id="start">Start</div>
  </body>
</html>
```

```js
$(function () {
  $("#start").html("Go!");
});
```

```js
/*
jQuery is used to select (query) HTML elements and perform "actions" on them.
Basic syntax is: $("selector").action()
- The $ accesses jQuery.
- The (selector) finds HTML elements.
- The action() is then performed on the element(s).
*/

$("p").hide(); // hides all <p> elements
$(".demo").hide(); // hides all elements with class="demo"
$("#demo").hide(); // hides the element with id="demo
```

## Selectors

```js
$("div")  // selects all <div> elements

Next are the id and class selectors, which select the elements by their id and class name:
$("#test") // select the element with the id="test"
$(".menu") //selects all elements with class="menu"
```

As we have seen in the previous lessons, the `html()` and `text()` methods can be used to get and set the content of a selected element. However, when these methods are used to set content, the existing content is lost.
jQuery has methods that are used to add new content to a selected element without deleting the existing content:
`append()` inserts content at the end of the selected elements.
`prepend()` inserts content at the beginning of the selected elements.
`after()` inserts content after the selected elements.
`before()` inserts content before the selected elements.
