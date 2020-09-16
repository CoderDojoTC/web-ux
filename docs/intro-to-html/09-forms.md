# HTML Forms
In this lab we will learn to create HTML forms that allow us to gather different types of input from users and send the users information to a file or a database.

## Form Structure
Form all have the following structure:

```html
<form action="/http-put-service">

    <label>
    <input>

    <label>
    <input>

    <label>
    <input>

    <input type="submit" value="Submit">
</form>
```

The action attribute is the place where the form data is sent.  Usually HTML forms send their data via an HTTP POST function.  The submit input just before the form close tag is the button that the user presses.  All the rest of the form consists of labels and inputs in pairs.  Sometimes the labels and input pairs are on the same line, and sometimes they are each on their own line. In some inputs such as checkboxes and radio button the label occurs before the input. You can use CSS to determine how your form is styled.

Here are the different types of input fields:

1. **Input fields** - a single line of input
2. **Selection lists** - where a user must select from one or more item of a fixed list
3. **Text Areas** - larger blocks of multi-line text input area
4. **Checkboxes** - check boxes where a user can check many items in a list
5. **Radio Buttons** - a variation of selection lists were all values are visible

## Input Fields

```html
<label for="fname">First name:</label>
<input type="text" id="firstName" name="firstName"/>
<label for="fname">Last name:</label>
<input type="text" id="firstName" name="firstName"/>
<input type="submit" value="Submit">
```

<div style="border:solid black 1px; background-color:silver">
    <form action="/http-put-service">
        <label for="fname">First name:</label>
        <input style="border:solid black 1px" type="text" id="firstName" name="firstName"/><br/>
        <label for="fname">Last name:</label>
        <input style="border:solid black 1px" type="text" id="lastName" name="lastName"/>
        <input type="submit" value="Submit">
    </form>
</div>

## Selection List

```html
<label for="language">Select your language:</label>
<select name="language" id="language">
  <option value="python">Python</option>
  <option value="c">C</option>
  <option value="java">Java</option>
  <option value="kotlin">Kotlin</option>
</select>
```

<label for="fname">Select your language:</label>
<select name="language" id="language">
  <option value="python">Python</option>
  <option value="c">C</option>
  <option value="java">Java</option>
  <option value="kotlin">Kotlin</option>
</select>

## Textarea

```html
<label for="notes">Enter your notes here</label><br/>
<textarea id="notes" name="notes" rows="4" cols="50">
Enter your notes here.
</textarea>
```

<div style="border:solid black 1px; background-color:silver">
    <label for="notes">Enter your notes here</label><br/>
    <textarea id="notes" name="notes" rows="4" cols="50">
    Enter your notes here.
    </textarea>
</div>

## Checkboxes
We use checkboxes when we have a list of items and each item can have a true or a false value.

```html
<p>What programming languages do you know?</p>

    <label for="python">Python</label>
    <input type="checkbox" id="python" name="python"/><br/>

    <label for="c">C</label>
    <input type="checkbox" id="c" name="c"/><br/>

    <label for="java">Java</label>
    <input type="checkbox" id="java" name="java"/><br/>
```

<div style="border:solid black 1px; background-color:silver">
    <p>What programming languages do you know? (check all that apply)</p>

    <input type="checkbox" id="python" name="python"/>
    <label for="python">Python</label>
    <br/>

    <input type="checkbox" id="c" name="c"/>
    <label for="c">C</label>
    <br/>

    <input type="checkbox" id="java" name="java"/>
    <label for="java">Java</label>
    <br/>
</div>

## Radio Buttons
Radio buttons are very similar to the selection list in that only one item is selected at a time.

```html
<p>What is your favorite language? (select only one item)</p>

        <input type="radio" id="python" name="python"/>
        <label for="python">Python</label>
        <br/>

        <input type="radio" id="c" name="c"/>
        <label for="c">C</label>
        <br/>

        <input type="radio" id="java" name="java"/>
        <label for="java">Java</label>
        <br/>
```

<div style="border:solid black 1px; background-color:silver">
    <form>
        <p>What is your favorite language? (select only one item)</p>

        <input type="radio" id="python" name="python"/>
        <label for="python">Python</label>
        <br/>

        <input type="radio" id="c" name="c"/>
        <label for="c">C</label>
        <br/>

        <input type="radio" id="java" name="java"/>
        <label for="java">Java</label>
        <br/>
    <form>
</div>