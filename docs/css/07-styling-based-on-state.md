# CSS Styling based on State

This lab covers styling based on state. 

In addition to selecting by element type, class, or id, CSS can select by state. An example is selecting elements as the mouse hovers over them. Another example is the visited state for links that have already been clicked on (note: this does not appear to work in JSFiddle)

CSS:
```css
a:hover {
  color: DarkSlateGray;
  font-weight: bold;
}
``` 

HTML:
```html
<!DOCTYPE html>
<html lang="en">
   <body>
     <a href="https://www.w3schools.com/tags/tag_a.asp">Click here if you want to know more about the HTML link element!</a>
     <br/>
     <a href="https://www.w3schools.com/colors/colors_picker.asp">Here's a link to the w3schools CSS color picker</a>
   </body>
</html>
```

This interaction is best viewed live. Try the example below. on JSFiddle.

# Link to Example

[Test on JSFiddle](https://jsfiddle.net/k_staple/rmj251Ls/16/)



# Experiment Ideas
1. Make the link being hovered over change font
2. Change the color of links being hovered over with the w3schools color picker
