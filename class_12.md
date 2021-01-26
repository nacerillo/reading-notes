# Class 11 notes:

## Charts.js:

- Chart.js is a free open-source JavaScript library for data visualization, which supports 8 chart types: bar, line, area, pie, bubble, radar, polar, and scatter.

Below is an example of a chart in in HTML/JS

```html
<canvas id="myChart" width="400" height="400"></canvas>
<script>
  var ctx = document.getElementById("myChart").getContext("2d");
  var myChart = new Chart(ctx, {
    type: "bar",
    data: {
      labels: ["Red", "Blue", "Yellow", "Green", "Purple", "Orange"],
      datasets: [
        {
          label: "# of Votes",
          data: [12, 19, 3, 5, 2, 3],
          backgroundColor: [
            "rgba(255, 99, 132, 0.2)",
            "rgba(54, 162, 235, 0.2)",
            "rgba(255, 206, 86, 0.2)",
            "rgba(75, 192, 192, 0.2)",
            "rgba(153, 102, 255, 0.2)",
            "rgba(255, 159, 64, 0.2)",
          ],
          borderColor: [
            "rgba(255, 99, 132, 1)",
            "rgba(54, 162, 235, 1)",
            "rgba(255, 206, 86, 1)",
            "rgba(75, 192, 192, 1)",
            "rgba(153, 102, 255, 1)",
            "rgba(255, 159, 64, 1)",
          ],
          borderWidth: 1,
        },
      ],
    },
    options: {
      scales: {
        yAxes: [
          {
            ticks: {
              beginAtZero: true,
            },
          },
        ],
      },
    },
  });
</script>
```

## Canvas API:

### Basic Usage:

- The `<canvas>` element has only two attributes, `width` and `height`. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.
- The `<canvas>` element can be styled with `margin, border, background, etc`. but these don't affect the actual drawing on the canvas.
- The `<canvas>` element creates a fixed-size drawing surface that exposes rendering contexts, which are used to create and manipulate content shown.

Below is an example of canvas template with the `draw()` function:
This will draw two squares to the screen.

```html
<html>
  <head>
    <meta charset="utf-8" />
    <script type="application/javascript">
      function draw() {
        var canvas = document.getElementById("canvas");
        if (canvas.getContext) {
          var ctx = canvas.getContext("2d");

          ctx.fillStyle = "rgb(200, 0, 0)";
          ctx.fillRect(10, 10, 50, 50);

          ctx.fillStyle = "rgba(0, 0, 200, 0.5)";
          ctx.fillRect(30, 30, 50, 50);
        }
      }
    </script>
  </head>
  <body onload="draw();">
    <canvas id="canvas" width="150" height="150"></canvas>
  </body>
</html>
```

## Drawing Shapes with the canvas:

- the canvas can be navigated as a x,y coordinate space, and each unit represents a single pixel.
- canvas only supports 2 shapes, paths and squares.
- other shapes need to be created using a combination of 1 or more paths.

**There are three functions that draw rectangles on the canvas:**

`fillRect(x, y, width, height)`
Draws a filled rectangle.

`strokeRect(x, y, width, height)`
Draws a rectangular outline.

`clearRect(x, y, width, height)`
Clears the specified rectangular area, making it fully transparent.

**Rectangular shape example**

````js
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}```
````

**Functions for drawing Paths**
`beginPath()`
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.

`closePath()`
Adds a straight line to the path, going to the start of the current sub-path.

`stroke()`
Draws the shape by stroking its outline.

`fill()`
Draws a solid shape by filling the path's content area.

Other Functions
`moveTo(x,y)` - Moves the pen to the coordinates specified by x and y.
`lineTo(x,y)` - Draws a line from the current drawing position to the position specified by x and y.

For Drawing Arcs and Cickles:
`arc(x, y, radius, startAngle, endAngle, anticlockwise)`
`arcTo(x1, y1, x2, y2, radius)`

Bezier and quadratic curves:
`quadraticCurveTo(cp1x, cp1y, x, y)`
`bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)`

## Applying and Style Colors:

- there are two important properites for coloring shapes:
- `fillStyle = color` Sets the style used when filling shapes.
  `strokeStyle = color` Sets the style for shapes' outlines.

  ```js
  //fill style example
  ctx.fillStyle = "orange";
  ctx.fillStyle = "#FFA500";
  ctx.fillStyle = "rgb(255,165, 0)";
  ctx.fillStyle = "rgba(255, 165, 0, 1)";

  //stroke style example
  function draw() {
    var ctx = document.getElementById("canvas").getContext("2d");
    for (var i = 0; i < 6; i++) {
      for (var j = 0; j < 6; j++) {
        ctx.strokeStyle =
          "rgb(0, " +
          Math.floor(255 - 42.5 * i) +
          ", " +
          Math.floor(255 - 42.5 * j) +
          ")";
        ctx.beginPath();
        ctx.arc(12.5 + j * 25, 12.5 + i * 25, 10, 0, Math.PI * 2, true);
        ctx.stroke();
      }
    }
  }
  ```

  - There are several properties that allow us to style lines.
    - `lineWidth = value` Sets the width of lines drawn in the future.
    - `lineCap = type` Sets the appearance of the ends of lines.
    - `lineJoin = type` Sets the appearance of the "corners" where lines meet.
    - `miterLimit = value` Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
    - `getLineDash()` = Returns the current line dash pattern array containing an even number of non-negative numbers.

## Draw Text:

- canvas has two methods for rendering text.

  - `fillText(text, x, y [, maxWidth])`
  - `strokeText(text, x, y [, maxWidth])`

  for styling text, there are the following properties:

  - `font` : The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
  - `textAlign` : Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
  - `textBaseline` : Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
  - `direction` : Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.
