# Drawing Ellipse with SVG
An ellipse can be thought of as a circle that is not perfectly round.  The height and width of an ellipse may be different.  In SVG, the ```ellipse``` element does not have a single radius like a circle, but
it has both a horizontal and a vertical radius.

Here are the attributes of an ellipse element:

* **cx** -  the x or horizontal dimension of the circle's center
* **cy** - the y or vertical dimension of the circle's center 
* **rx** - the x or horizontal radius of the ellipse
* **ry** - the y or vertical radius of the ellipse

## Example Markup for SVG Ellipse
This example will generate an ellipse:

```html
<svg height="200" width="200">
  <ellipse cx="100" cy="80" rx="100" ry="50"
           fill="yellow" stroke-width="3"; stroke="purple" />
</svg>
```
Note that the second line has the color and width of the border.

## Rendering of SVG Ellipse
<svg height="200" width="200">
  <ellipse cx="100" cy="80" rx="90" ry="50"
           fill="yellow" stroke-width="3"; stroke="purple" />
</svg>

Note that the first line is about positioning and size.  The properties in the second line can
also be determined by SVG CSS properties.
