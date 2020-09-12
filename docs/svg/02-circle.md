# Drawing a Circle with SVG

Lets start with drawing a single circle.  We will need to
tell our web browser to draw it in a region that is 100 pixels
high and 100 pixels wide.  We then need to tell the web browser
where to center the circle in both the X and Y dimensions (cx and cy) and what the radius of the circle should be.  Here is an example:

```html
<svg height="100" width="100">
  <circle cx="50" cy="50" r="40"/>
</svg>
```

This example will generate the following circle:

<svg height="100" width="100">
  <circle cx="50" cy="50" r="40" />
</svg>

That is kind of a dark circle.  Let's fill in the circle with blue and make the border be red.  We will do this by adding the fill, stroke (for the color of the border) and the stroke-width that will change the width of the border of the circle.

```html
<svg height="100" width="100">
  <circle cx="50" cy="50" r="40" stroke="red" stroke-width="4" fill="blue" />
</svg>
```

This will generate the following result:

<svg height="100" width="100">
  <circle cx="50" cy="50" r="40" stroke="red" stroke-width="4" fill="blue" />
</svg>

Try changing the color of the fill or the stroke and see what happens!

## Run on JS Fiddle.net

[Run on Fiddle](https://jsfiddle.net/9cnogwuh/)