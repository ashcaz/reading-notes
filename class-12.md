## Web Designer Depot Article

**Chart.js**

- Chart.js is a great way to diaplay data visually.
- Chart.js is a javascript plugin that uses HTML5's canvas element to draw a graph onto the page
- Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script:

```javascript
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <script src='Chart.min.js'></script>
    </head>
    <body>
    </body>
</html>
```

**Drawing a line chart**

Instead of me sumerizing this badly just go [HERE](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

## Canavas API

**Basic Usage**

- similar to the `<img>` tag but it doesnt have `src` or `alt` attributes.
- `<canvas>` has only two attributes - `width` and `height`

**Drawing Shapes with Canvas**

- There are three functions that draw rectangles on the canvas:

1. fillRect(x, y, width, height)
  - Draws a filled rectangle.
2. strokeRect(x, y, width, height)
  - Draws a rectangular outline.
3. clearRect(x, y, width, height)
  - Clears the specified rectangular are, making it fully transparent.

```javascript
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}
```
[Way more shapes](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
**Applying styles and colors**

- to apply colors to a shape, there are two important properties we can use: `fillStyle` and `strokeStyle`.

1. fillStyle = color
  - Sets the style used when filling shapes.
2. strokeStyle = color
  - Sets the style for shapes' outlines.

  [more here](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)


**Drawing Text**

- rendering context provides two methods to render text:

1. fillText(text, x, y [, maxWidth])
  - Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

```JavaScript
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.fillText('Hello world', 10, 50);
}
```
2. strokeText(text, x, y [, maxWidth])
  - Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

  
```JavaScript
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.strokeText('Hello world', 10, 50);
}
```

[More Here](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)


[Back to Homepage](https://ashcaz.github.io/reading-notes)