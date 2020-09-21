# Events
Events are actions or occurrences that happen in the system you are programming, which the system tells you about so you can respond to them in some way if desired. For example, if the user selects a button on a webpage, you might want to respond to that action by displaying an information box

In the case of the Web, events are fired inside the browser window, and tend to be attached to a specific item that resides in it — this might be a single element, set of elements, the HTML document loaded in the current tab, or the entire browser window. There are many different types of events that can occur. For example:

* The user selects a certain element or hovers the cursor over a certain element.
* The user chooses a key on the keyboard.
* The user resizes or closes the browser window.
* A web page finishes loading.
* A form is submitted.
* A video is played, paused, or finishes.
* An error occurs.

Each event can have an event handler, which is a block of code (usually a JavaScript function that you as a programmer create) that runs when the event fires.

Let's use a button click event as an example to learn how we can create event handlers. You've probably seen events and event handlers used in some of the other examples, but let's take a closer look. First we need to create a button so that we have an html element to click on. Place the following code in your html body:
```
<button>Change color</button>
```
Now we need the JavaScript to handle the click event. Place the following in your script.js file:
```
const btn = document.querySelector('button');

function random(number) {
  return Math.floor(Math.random() * (number+1));
}

btn.onclick = function() {
  const rndCol = 'rgb(' + random(255) + ',' + random(255) + ',' + random(255) + ')';
  btn.style.background = rndCol;
}
```
Run the site and you should be able to see the button color change when you click on it.

In this code, we store a reference to the button inside a constant called btn, using the Document.querySelector() function. We also define a function that returns a random number. The third part of the code is the event handler. The btn constant points to a button element, and this type of object has a number of events that can fire on it, and therefore, event handlers available. We are listening for the click event firing, by setting the onclick event handler property to equal a function containing code that generates a random RGB color and sets the <button> background color equal to it.

This code is run whenever the click event fires on the button element, that is, whenever a user selects it.
  
There are many different event handler properties available. Feel free to experiment.

Try changing btn.onclick to the following different values in turn, and observing the results in the example:

* btn.onfocus and btn.onblur — The color changes when the button is focused and unfocused; try pressing the tab to focus on the button and press the tab again to focus away from the button. These are often used to display information about filling in form fields when they are focused, or displaying an error message if a form field is filled with an incorrect value.
* btn.ondblclick — The color changes only when the button is double-clicked.
* window.onkeypress, window.onkeydown, window.onkeyup — The color changes when a key is pressed on the keyboard. The keypress event refers to a general press (button down and then up), while keydown and keyup refer to just the key down and key up parts of the keystroke, respectively. Note: It doesn't work if you try to register this event handler on the button itself — we've had to register it on the window object, which represents the entire browser window.
* btn.onmouseover and btn.onmouseout — The color changes when the mouse pointer hovers over the button, or when the pointer moves off the button, respectively.

You can also bind an event handler using the following code:
```
btn.addEventListener('click', function);
```
The behavior of addEventListener() is very similar, but allows you to add multiple handlers to the same event or even dynamically remove them. This method takes two arguments, a string of the event, and either a function name to run, or a new anonymous function. It is useful for larger and more complex sites.
