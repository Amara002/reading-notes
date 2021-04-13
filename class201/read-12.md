# Charts
***harts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.***

## Types of drawing chart
- **Drawing a line chart**
- **Drawing a pie chart**
- **Drawing a bar chart**

## Creating a Chart
***It's easy to get started with Chart.js. All that's required is the script included in your page along with a single '< canvas >' node to render the chart.***

> ***Note: If your renderings seem distorted, try specifying your width and height attributes explicitly in the '< canvas >' attributes, and not using CSS.***

## Checking for support
***The fallback content is displayed in browsers which do not support '< canvas >'. Scripts can also check for support programmatically by testing for the presence of the getContext() method.***

## Drawing shapes with canvas
1. **Drawing rectangles:**
***First let's look at the rectangle. There are three functions that draw rectangles on the canvas:***

- ***fillRect(x, y, width, height) Draws a filled rectangle.***
- ***strokeRect(x, y, width, height) Draws a rectangular outline.***
- ***clearRect(x, y, width, height) Clears the specified rectangular area, making it fully transparent.***

2. **Drawing paths**
***Here are the functions used to perform these steps:***

- ***beginPath()Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.***
- ***Path methods Methods to set different paths for objects.***
- ***closePath() Adds a straight line to the path, going to the start of the current sub-path.***
- ***stroke() Draws the shape by stroking its outline.***
- ***fill() Draws a solid shape by filling the path's content area.***

3. **Drawing a triangle**
***One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the moveTo() function.***

4. **Lines**
***For drawing straight lines, use the lineTo() method.***

***lineTo(x, y) Draws a line from the current drawing position to the position specified by x and y.*** 

5. **Arcs**
***To draw arcs or circles, we use the arc() or arcTo() methods.***

***arc(x, y, radius, startAngle, endAngle, counterclockwise) Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by counterclockwise (defaulting to clockwise).***

6. **Rectangles**
***rect(x, y, width, height) Draws a rectangle whose top-left corner is specified by (x, y) with the specified width and height.***

7. **Path2D objects**
***The Path2D() constructor returns a newly instantiated Path2D object, optionally with another path as an argument (creates a copy), or optionally with a string consisting of SVG path data.***

## Applying styles and colors
***Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.***

***fillStyle = color Sets the style used when filling shapes.***
***strokeStyle = color Sets the style for shapes' outlines.*** 

## Drawing text
***The canvas rendering context provides two methods to render text:***

***fillText(text, x, y [, maxWidth]) Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.***
***strokeText(text, x, y [, maxWidth]) Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.*** 