# Class 09:

## Forms:

- **Form:** An element that allows a webpage to collect information from visitors of the site. bascially anything that takes input from user.
- forms take input from _form controls_
  - Examples: search boxes, log in, button-inputs text areas, etc

```html
<!-- httm layout for a form. 
    all forms have an ACTION and METHOD attribute

    action = value is the url for the page on the server that will recieve the information in the form when it is submitted

    method = can be 'get' or 'post' method.
-->
<form action="http://www.example.cpm/subscribe.php" method="get">
  <p>This is where the form controls will go</p>
</form>
```

- the `input` element can be used inside a form to collect text based input.

  - has type of both `text`, and `password`.

- other types of input include:
  - Radio Button
  - Checkbox
  - Drop down List
  - multiple selection box
  - file input
  - submit button

## Lists,Table & Forms

### Lists

- lists can be given different bullet styles using css. and can postion markers inside or outside

  ```css
  ol {
    list-style-type: lower-roman;
    list-style-position: outside;
  }
  ul {
    list-style-image: url("image/image.png");
    list-style-position: inside;
  }
  ```

  ### Tables:

  - tables have the following css properties.

    - `width, padding, text-transform, letter-spacing, font-size, border botto text-align, background-color, :hover`

    - can use `empty-cells` property to maek empty cells invisible.
    - `border-spacing` controls wheter cells have gaps between them.

### From Style:

- common to use styling on Text inputs/areas, submit buttons, and form labels.
- tricker to style the other types.
- properties can be found pages 342-347.

## Events:

- created by interactions from the user.
- triggering some kind of response from the server. and creating a response.
  - event types include
    - UI events
    - Keyboard events
    - mouse events
    - focus events `(zoom in/out)`
    - Form changes/inputs
    - Mutations in the DOM.
