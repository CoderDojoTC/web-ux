# Drawing A Polygon with SVG

A polygon is a figure with an arbitrary number of straight sides.  We can use the ```polygon``` element to make many different shapes such as triangles, hexagons and octagons.

To draw a polygon we use a ```points``` attribute to specify each of the x,y pairs we need to draw the polygon.  Here is an example of a blue trinagle:

## Drawing a Triangle
```html
<svg height="100" width="100">
  <polygon points="10,90 90,90 50,10"
     fill="blue" stroke="orange" stroke-width="3" />
</svg>
```
Which renders like this:

<svg height="100" width="100">
  <polygon points="10,90 90,90 50,10"
     fill="blue" stroke="orange" stroke-width="3" />
</svg>

Note that the first point is in the lower-left corner (x=10, y=90).  The second point is in the right corner (x=90, y=90) and the last point is in the top center (x=50, y=10).

Note that this triangle is called an isosceles because two of the sides are exactly the same length.
We don't have to make the edges the same size.  We can move the points to make any arbitrary shape.

```html
<svg height="100" width="100">
  <polygon points="30,90 90,70 40,10"
     fill="blue" stroke="orange" stroke-width="3" />
</svg>
```
Which renders like this:

<svg height="100" width="100">
  <polygon points="30,90 90,70 40,10"
     fill="blue" stroke="orange" stroke-width="3" />
</svg>

## Drawing A Hexagon
A hexagon is a shape with six sides.

```html
<svg height="300" width="300">
   <polygon points="300,150 225,280 75,280 0,150 75,20 225,20"
     fill="orange" stroke="blue" stroke-width="3"/>
</svg>
```

<svg height="300" width="300">
   <polygon points="300,150 225,280 75,280 0,150 75,20 225,20"
     fill="orange" stroke="blue" stroke-width="3"/>
</svg>

## Drawing an Octagon
An Octagon is a shape with eight sides.  You might recognize this as the shape of a STOP sign.

```html
<svg height="125" width="125">
   <polygon points="50,5 100,5 125,30  125,80 100,105 50,105  25,80  25, 30"
      ill="red" stroke="silver" stroke-width="5"/>
</svg>
```

<svg height="125" width="125">
   <polygon points="50,5 100,5 125,30  125,80 100,105 50,105  25,80  25, 30"
      fill="red" stroke="silver" stroke-width="5"/>
</svg>

## Five Pointed Star

```html
<svg width="100" height="100">
  <polygon 
      points="50,10 55,30 70,30 60,40 65,55 50,45 35,55 40,40 30,30 45,30"
      stroke="Blue" 
      fill="LightBlue" 
      stroke-width="2"/>
</svg>
```

<svg width="100" height="100">
  <polygon 
      points="50,10 55,30 70,30 60,40 65,55 50,45 35,55 40,40 30,30 45,30"
      stroke="Blue" 
      fill="LightBlue" 
      stroke-width="2"/>
</svg>

## 10 Pointed Star
Here is what a 10 pointed star looks like in SVG:

```html
<svg width="100" height="100">
  <polygon 
    points="50,80 65.451,97.553 67.634,74.271 90.451,79.389 78.532,59.271
    100.000,50.000 78.532,40.729 90.451,20.611 67.634,25.729 65.451,2.447
    50.000,20.000 34.549,2.447 32.366,25.729 9.549,20.611 21.468,40.729
    0.000,50.000 21.468,59.271 9.549,79.389 32.366,74.271 34.549,97.553
    50.000,80.000"
    stroke="black" 
    fill="yellow" 
    stroke-width="2"/>
</svg>
```
And here is how that renders:

<svg width="100" height="100">
  <polygon 
    points="50,80 65.451,97.553 67.634,74.271 90.451,79.389 78.532,59.271
    100.000,50.000 78.532,40.729 90.451,20.611 67.634,25.729 65.451,2.447
    50.000,20.000 34.549,2.447 32.366,25.729 9.549,20.611 21.468,40.729
    0.000,50.000 21.468,59.271 9.549,79.389 32.366,74.271 34.549,97.553
    50.000,80.000"
    stroke="black" 
    fill="yellow" 
    stroke-width="2"/>
</svg>

If you want to create your own stars, you can do it with this tool:
See [SVG Star Generator](https://www.smiffysplace.com/stars.html)

We will learn about paths next!