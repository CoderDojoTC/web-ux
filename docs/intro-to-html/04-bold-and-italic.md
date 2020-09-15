# Adding Bold and Italic to HTML
HTML allows us to add bold and italic to any text in a document.  To do this we need to wrap the text in ```<b>``` elements for bold and ```<i>``` elements for italics.

Here is an example of adding bold and italic to a paragraph of text.
```html
<p>HTML allows us to add <b>bold</b> to any text that we want to
 <b>emphasize.</b>.  We can also add <i>italic</i> text or a 
 combination of both <b><i>bold and italic</i></b>.
</p>
```
Which will render like this:
<p>HTML allows us to add <b>bold</b> to any text that we want to <b>emphasize.</b>.  We can also add <i>italic</i> text or a combination of both
<b><i>bold and italic</i></b> elements turned on.
</p>

!!! Warning
     You must remember to close the bold and italic markup.  They don't just apply to a single world.  Make sure you close the elements in the reverse order that you added them.

## Other Inline Elements
There are two other interesting inline elements that you might want to use.  One is for creating superscripts and one is for subscripts.

### Superscripts
To make text appear shifted up we use the ```<sub>``` tag.
Here we use it in a mathematical formula to show an exponent:

```html
<p>y = x<sup>2</sup> + 2x + 1<p>
```
which will render:
<p>y = x<sup>2</sup> + 2x + 1<p>

You can also use some greek letters if you know how to encode them.  Here the greek letter "pi" is references using ```&pi;```

```html
<p>The formula:<br/>
   e<sup>i&pi;</sup>= -1<br/>
is one of the most elegant formulas in mathematics
</p>
```

<p>The formula:<br/>
   e<sup>i&pi;</sup>= -1<br/>
is one of the most elegant formulas in mathematics
</p>

### Subscripts
```html
<p>The chemical formula for water is
   H<sub>2</sub>O
</p>
```

<p>The chemical formula for water is
   H<sub>2</sub>O
</p>

```html
<p>The chemical formula for caffeine is
   C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>
</p>
```

<p>The chemical formula for caffeine is
   C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>
</p>