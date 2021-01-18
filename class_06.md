# Class 0 6 Notes

## Article: Understanding Problem Domain

- **Problem Domain**: the goal that defines a project. what is the costumer asking us to make for them?

- repetion of building similar applications helps to solidy understanding of the technology.
- Very often, the problem domain is not clear-cut, its like a jigsaw puzzle.
- breaking down a problem domain into seperate tasks and features makes it much easier to tackle.

## Object Literals:

- creating an object literal notation:

```js
var hotel = {
  //properties
  name: "Quay",
  rooms: 40,
  booked: 25,
  //method
  checkAvailability: function () {
    return this.rooms - this.booked;
  },
};

//we can access an object with the following notations
var hotelName = hotel.name;
var roomsFree = hotel.checkAvailability();

var hotelName = hotel["name"];
var roomsFree = hotel["checkAvailability"]();
```

## Document Object Model - DOM -:

- DOM: specifies how browsers should create a model of anHTML page
  and how javascript can access and update the contents of a webpage while it is in the browser window
- it does covers...
  - Making a model of the HTML Page
  - Accessing and changing the HTML page.
- the DOM is an **API** or **Application Programming Interface**.
- APIs let programs talk to one another. in the case of the DOM, it states what your script can ask the browser about the current page, and how to tell the browser to update what is being shown to the user.

- **DOM Tree:** the model of the webpage stored in the browser's memory
- consists of 4 main node types:

  - Document node:
  - Element node:
  - Attribute node:
  - Text node:

- updating the DOM tree involves two steps:
  - Locate the node the represents the element you want to work with
  - Use its text content, child elements, and attributes.

### Accessing Elements:

- Methods That Return A Single Element:
  - `getElementById(id)`
  - `querySelector(css selector)`
- Methods Thar Return Multiple Elements:

  - `getElementsByClassName(class)`
  - `getElementsByTagName(tagName)`
  - `querySelectAll(css selector)`

- **Node lists:** Dom queries that return more than one element
  - **live Nodelists:** Nodelist that updates that updates at the same time as your script update.
  - **static Nodelists:** Nodelist _does not_ update with changes to your script

Two ways of getting element from Nodelist:

```js
//item() method
var elements = documents.getElementsByClassName("hot");
if (elements.length >= 1) {
  var firstItem = elements.items(0);
}

//array syntax
var elements = documents.getElementsByClassName("hot");
if (elements.length >= 1) {
  var firstItem = elements[0];
}
```

Selecting Elemetns by Class/Tag/CSS Selectos

```js
//selecitng by class
var elements = documents.getElementsByClassName(`hot`);
if (elements.length > 2) {
  var el = elements[2];
  el.className = `cool`;
}

//selecting by tag

var elements = document.getElementsByTagName(`li`);
if (elements.length > 0) {
  var el = elements[0];
  el.className = `cool`;
}

var el = document.querySelector("li.hot");
el.className = "cool";

var els = document.querySelectorAll("li.hot");
els[1].className = "cool";
```

When it comes to traversing the DOM, when you have an element node, you can
select another element in relation to it using these five properties...

- parentNode
- prviousSibling
- nextSibling
- firstChild
- lastChild

## Adding and Removing HTML Content

using the innerHTML property...
Adding:

1.  Store new content as a string in a variable.
2.  Select the elements whose content you want to replace
3.  Set the element's `innerHTML` property to the new string.

    Removing:
    set `innterHTML` to an empty string.
