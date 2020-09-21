# Introduction

JavaScript is a scripting or programming language that allows you to implement complex features on web pages — every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. — you can bet that JavaScript is probably involved. It is the third layer of the layer cake of standard web technologies, two of which (HTML and CSS)

![The web layer cake](../img/web-layer-cake.png)

* HTML is the markup language that we use to structure and give meaning to our web content, for example defining paragraphs, headings, and data tables, or embedding images and videos in the page.
* CSS is a language of style rules that we use to apply styling to our HTML content, for example setting background colors and fonts, and laying out our content in multiple columns.
* JavaScript is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else. (Okay, not everything, but it is amazing what you can achieve with a few lines of JavaScript code.)

The three layers build on top of one another nicely. Let's demonstrate this using a simple example. For the following code, and for code examples in the other Javascript lessons, create an account for the online web editor [repl.it](https://repl.it/~)

Using a simple text label as an example, We can mark it up using HTML to give it structure and purpose. Paste the following into the body of your index.html file on repl:

```
<p>Player 1: Chris</p>
```

It should display as:

Player 1: Chris

Then we can add some CSS into the mix to get it looking nice, paste the following into style.css on repl.it

```
p {
  font-family: 'helvetica neue', helvetica, sans-serif;
  letter-spacing: 1px;
  text-transform: uppercase;
  text-align: center;
  border: 2px solid rgba(0,0,200,0.6);
  background: rgba(0,0,200,0.3);
  color: rgba(0,0,200,0.6);
  box-shadow: 1px 1px 2px rgba(0,0,200,0.4);
  border-radius: 10px;
  padding: 3px 10px;
  display: inline-block;
  cursor: pointer;
}
```

And it should display as:

![Formatted Button](../img/html-and-css-button.png)

And finally, we can add some JavaScript to implement dynamic behaviour, paste the following in scripts.js on repl.it

```
const para = document.querySelector('p');

para.addEventListener('click', updateName);

function updateName() {
  let name = prompt('Enter a new name');
  para.textContent = 'Player 1: ' + name;
}
```

You should be able to click the text label now and see what happens.

JavaScript can do a lot more than that — let's explore in the next lesson.
