## Creating a Chart
It's easy to get started with Chart.js. All that's required is the script included in your page along with a single `<canvas>` node to render the chart.
## The `<canvas>` element 
At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high
## The rendering context
The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The `<canvas>` element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context
## Checking for support
The fallback content is displayed in browsers which do not support `<canvas>`. Scripts can also check for support programmatically by testing for the presence of the getContext()

by canvas element we can draw rectangles, triangles, lines, arcs and curves, providing familiarity with some of the basic shapes.
## Drawing text
The canvas rendering context provides two methods to render text:
- 
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
