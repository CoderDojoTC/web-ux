# Drawing A Polygon with SVG
A polyline element is used to create any drawing that consists of only strait lines.  It is
very similar to the polygon in that it uses a points attribute to store the points.

# SVG Polyline Drawing

```html
<svg height="160" width="200">
  <polyline points="0,40 40,40 40,80 80,80 80,120 120,120 120,160"
      fill="none" stroke="purple" stroke-width="3"/>
</svg>
```

<svg height="160" width="200">
  <polyline points="0,40 40,40 40,80 80,80 80,120 120,120 120,160"
     fill="none" stroke="purple" stroke-width="3"/>
</svg>

Note that we must use the ```fill=none``` attribute or the rendering tool will try to
fill in the area inside the polyline.

<svg height="160" width="200">
  <polyline points="0,40 40,40 40,80 80,80 80,120 120,120 120,160"
     stroke="purple" stroke-width="3"/>
</svg>

This may not be the effect that you want!