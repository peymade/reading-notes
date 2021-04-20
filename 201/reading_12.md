# Reading 12

## Chart.JS

You can use plug-ins to add to the functionality of HTML and JavaScript! One of these is Chart.js. 

### To create a chart

- Make a `<canvas>` element in the HTML
- Write JavaScript that uses `document.getElementById` to retrieve the canvas
- Creat the data in the script! You could use an object to do this. 
- To create pie charts, use array data
- You can create pie charts, bar graphs, and many other types.

## Canvas Element

- Example: `<canvas id="graph" width="400" height="400"></canvas>` 
  - The canvas element should have an id, and a width and a height. 
- CSS can be used on the element, but it won't have an affect on the styling of the inside of the chart
- Add fallback content betweeen the tags for older browsers. Make sure to have that closing tag!
- The canvas is rendered using the `draw()` function
- The draw function can happen after a certain action or event, like user interaction or a browser level event. 

## Drawing with Canvas

- Canvas operates on a grid- which starts at 0,0 in the top left corner. 
- The canvas tag supports rectangles and paths (points connected by lines)
  - `fillRect(x, y, width, height)` A filled rectangle
  - `strokeRect(x, y, width, height)` An outline of a rectangle
  - `clearRest(x, y, width, height)` Clears a rectangular area of other things
- The x, y coordinates specify the top left position of the rectangle
- Paths must first be created, with the `beginPath()` function, THEN they can be drawn. `closePath()` adds a straight line to the path. `stroke()` and `fill()` can be used to further draw it. 
- The `moveTo(x, y)` function moves the pen 
- Create a line from current position to another position using `lineTo(x, y)`
- You can also create arcs, and bezier and quadratic curves. 
  - Bezier takes two control points, while quadratic takes one


## Styles and Colors

- To apply colors to a shape, use `fillStyle = color` or `strokeStyle = color`. 
- Add an a at the end of rgba, and another number at the end of the number sequence, between 0 and 1, to determine opacity

Lines can be styled using the following properties:

- `lineWidth = value` sets line width for future lines
- `lineCap = type` sets apperance of ends of lines
- `lineJoin = type` sets apperance of corners
- `miterLimit = value` establishes miter on sharp angle
- `getLineDash()` gives you line dash pattern array
- `setLineDash(segments)` sets line dash pattern
- `lineDashOffset = value` sets start of dash array on line

Shadows and gradients can also be created. 

- `createLinearGradient(x1, y1, x2, y2)` creates the basis for a gradient. Add color stops to set the colors it will transition from and to. You can also make conic and radial gradients. 
- Shadows need `shadowOffset` and `shadowBlur` and `shadowColor`

## Drawing Text

There is fillText and strokeText- two ways to render text. 

- `fillTest(text, x, y [, madWidth])` 
- `strokeText(text, x, y [, maxWidth])`

Just like in CSS, there are lots of properties for styling text. Including:

- `font = value`
- `text-align = value`
- `textBaseline = value`
- `direction = value`




[Home](https://peymade.github.io/reading-notes/)