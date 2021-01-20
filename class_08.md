# Class 08:

## Layout:

- Block-level Elements start a new line.
  - `h1, p, ul, li`
- Inline Elements flow between surrounding text.
  - `img, b, i`
- Position Properties
  - CSS has the following positioning schemas:
    - normal flow
    - relative positioning
    - absolute positioning
  - can set the positioning schema using the `position` property.

\

- **Absolute:** positions the elements in relation to its containg elements. it does not affect the position of its
  surrounding elements
- **Fixed:** Removes element from the normal flow, and instead positon something relative to the view port?
- **Relative:** keeps the element within the normal flow, but can be moved left and right, and can still use as an anchor point
- **Static/Normal Flo1:** flow is preserved. cannot be used as anchor point.
- **Sticky:** combination of fixed and absolute.

- can using the `z-index` property to control which elements sit on top of others.
- the `float` property allows you to take an element in normal flow and placie it as far to the left or right of a containing element as you wish.
  - float can allow us to place box elements side by side.
- `clear` property allows you to say that no element is allowed to touch the left/right sides of the box.

  - note: can create mulit-column elements by making proper use of
    `div` and the properites `width`,`float` and `margin`

    ```css
    .column1of3 .column2of3 .column3of3 {
      float: left;
      width: 300px;
      margin: 10px;
    }
    ```

### Layout Types:

- Fixed Width Layout:
  - width specified in pixels.
  - will stay the same no matter the size of the broswer window.
- Liquid Layout:
  - width specified using percentage.
  - boxes will stretch and shrink with the browser window.

### Grid Layouts

- possible option = 960 Pixel Wide 12 Column Grid

### CSS Frameworks:

- provide the code for grid layouts and styling forms.
  - example: the 960.GS CSS Framwork.
  - can be found on **page 393 of textbook**
