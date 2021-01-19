# Class 07

## Tables:

- think in terms of a grid lay out.
- uses four key elements for to make tables
  - `<table>` start of a table
  - `<th>` table header-cell
  - `<tr>` start of a table row
  - `<td>` table info-cell

```html
<table>
  <tr>
    <th>table head</th>
    <td>monday</td>
    <td>tuesday</td>
    <td>wednesday</td>
    <td>thursday</td>
    <td>firday</td>
  </tr>
</table>
```

- can use attribute `colspan` and `rowspan` to lengthen table cells by row and height
- `<thead>` can be wrapped around multiple `<th>`
- `<tbody>` to wrap around the body of the table data
- `<tfooter>` to add a footer to a table.

## Functions, Methods, and Objects:

- Obeject constructors can be used as a template to create new obejcts.

  ```js
  function Hotel(name, rooms, booked) {
    this.name = name;
    this.rooms = rooms;
    this.booked = booked;

    this.checkAvailability = function () {
      return this.rooms - this.booked;
    };
  }

  var quayHotel = new Hotel(`Quay`, 40, 25);
  var parkHotel = new Hotel(`Park`, 120, 77);
  ```

  - the `this` keyword is commonly used inside functions and objects. Where the function is declared alters what `this` means. It always refers to one object, usually the object in which the function operates.

  - a **function** becomes a **method** when it is defined inside of an object.

  - arrays ARE objects, and hold a set of key/value pairs. the keys, in this case, being the indicies of the array.

  - there are 3 groups of build in objects
    - Broswer Object Model
    - Document Object Model
    - Global Javascript Objects
