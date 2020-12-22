# CSS External vs Internal vs Inline CSS

This lab covers External vs Internal vs Inline CSS. 

So far, the CSS has been listed separately from the HTML (external CSS). However, you can use a style tag within HTML to specify some CSS. This is called internal CSS (example below). A final type of CSS is inline CSS which involves setting a style attribute within an HTML tag. Inline CSS only lets you style one element at a time, so it's often not as useful as the other two types.

HTML with CSS in the style tag:
```html
<!DOCTYPE html>
<html lang="en">
   <head>
     <style>
       p {color: red;}
     </style>
   </head>
   <body>
     <p>Various species of penguin live on all continents that are partially or totally located in the Sourthern Hemisphere.</p>
   </body>
</html>
```

A website would combine the above CSS and HTML to show:  
![HTML/CSS example of styling by id](./img/08-example_inline_CSS_penguins.png)

# Link to Example

[Test on JSFiddle](https://jsfiddle.net/k_staple/4nfxtbh7/2/)



# Experiment Ideas
1. Change the style within the {}
2. Add a different type of HTML element & style it using the style tag
