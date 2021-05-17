# Chart.js, Canvas
## EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS
### Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly.
### A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. 
### Setting up:
+ The first thing we need to do is download Chart.js.(copy it).
+ Then create a new html page and import the script.in html code we need <canvas> node to render the chart.
### now to draw line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element .
#### Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart.
### there are different types of chart such as  line chart ,  pie chart , bar chart .

## Basic usage of canvas:
### we used it as <canvas id="tutorial" width="150" height="150"></canvas>
#### it  have only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.
#### he <canvas> element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context. For 2D graphics, such as those covered by this tutorial, you specify "2d" to get a CanvasRenderingContext2D.
#### The script includes a function called draw(), which is executed once the page finishes loading; this is done by listening for the load event on the document. This function, or one like it, could also be called using window.setTimeout(), window.setInterval(), or any other event handler, as long as the page has been loaded first.
### Drawing shapes with canvas :
#### the grid 
![](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes/canvas_default_grid.png)
#### Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y).
#### Drawing rectangles :Unlike SVG, <canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes. 
#### There are three functions that draw rectangles on the canvas:
+ fillRect(x, y, width, height) :Draws a filled rectangle.
+ strokeRect(x, y, width, height) :Draws a rectangular outline.
+ clearRect(x, y, width, height) :Clears the specified rectangular area, making it fully transparent.
#### Drawing paths :A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:
1- First, you create the path.
2- Then you use drawing commands to draw into the path.
3- Once the path has been created, you can stroke or fill the path to render it.
* beginPath(): Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
* Path methods: Methods to set different paths for objects.
* closePath(): Adds a straight line to the path, going to the start of the current sub-path.
* stroke() :Draws the shape by stroking its outline.
* fill() :Draws a solid shape by filling the path's content area .
#### also there is a useful function such as moveTo() function and  lineTo() method which is used to draw straight lines,To draw arcs or circles, we use the arc() or arcTo() methods.
### Applying styles and colors
#### Colors : If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

+ fillStyle = color: Sets the style used when filling shapes.
+ strokeStyle = color: Sets the style for shapes' outlines.
#### Transparency:This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

##### globalAlpha = transparencyValue .
#### Line styles :There are several properties which allow us to style lines.

+ lineWidth = value: Sets the width of lines drawn in the future.
+ lineCap = type :Sets the appearance of the ends of lines.
+ lineJoin = type :Sets the appearance of the "corners" where lines meet.
+ miterLimit = value : Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
* getLineDash() :Returns the current line dash pattern array containing an even number of non-negative numbers.
* setLineDash(segments) :Sets the current line dash pattern.
* lineDashOffset = value :Specifies where to start a dash array on a line.
### Drawing text 
#### The canvas rendering context provides two methods to render text:

1- fillText(text, x, y [, maxWidth]) :Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
2- strokeText(text, x, y [, maxWidth]) :Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
#### Styling text
#### we are already making use of the font property to make the text a bit larger than the default size. There are some more properties which let you adjust the way the text gets displayed on the canvas:

* font = value:The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
* textAlign = value:Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
* textBaseline = value:Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
* direction = value: Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.