# Variables
Variables are containers for values (such as numbers, or strings of text). You create a variable with the keyword let (or var) followed by a name for your variable. 

```
let name = 'Bob';
console.log('My name is ' + name);
name = 'Alice';
console.log('My name is ' + name);
```

## Naming variables
You can call a variable pretty much anything you like, but there are limitations. Generally, you should stick to just using Latin characters (0-9, a-z, A-Z) and the underscore character.

* You shouldn't use other characters because they may cause errors or be hard to understand for an international audience.
* Don't use underscores at the start of variable names — this is used in certain JavaScript constructs to mean specific things, so may get confusing.
* Don't use numbers at the start of variables. This isn't allowed and causes an error.
* A safe convention to stick to is so-called "lower camel case", where you stick together multiple words, using lower case for the whole first word and then capitalize subsequent words. We've been using this for our variable names in the article so far.
* Make variable names intuitive, so they describe the data they contain. Don't just use single letters/numbers, or big long phrases.
* Variables are case sensitive — so myage is a different variable from myAge.
* One last point: you also need to avoid using JavaScript reserved words as your variable names — by this, we mean the words that make up the actual syntax of JavaScript! So, you can't use words like var, function, let, and for as variable names. Browsers recognize them as different code items, and so you'll get errors.

## Variable Types
There are a few different types of data we can store in variables.

Note: JavaScript is a "dynamically typed language", which means that, unlike some other languages, you don't need to specify what data type a variable will contain (numbers, strings, arrays, etc).

### Numbers
You can store numbers in variables, either whole numbers like 30 (also called integers) or decimal numbers like 2.456 (also called floats or floating point numbers). You don't need to declare variable types in JavaScript, unlike some other programming languages. When you give a variable a number value, you don't include quotes:

```
let myAge = 15
```

### Strings
Strings are pieces of text. When you give a variable a string value, you need to wrap it in single or double quote marks; otherwise, JavaScript tries to interpret it as another variable name.

```
let myName = 'John';
```

### Booleans
Booleans are true/false values — they can have two values, true or false. These are generally used to test a condition, after which code is run as appropriate. So for example, a simple case would be:

```
let isLoggedIn = false;
```

### Arrays
An array is a single object that contains multiple values enclosed in square brackets and separated by commas.

```
let myNameArray = ['Chris', 'Bob', 'Jim'];
let myNumberArray = [10, 15, 40];
```

### Objects
In programming, an object is a structure of code that models a real-life object. You can have a simple object that represents a box and contains information about its width, length, and height, or you could have an object that represents a person, and contains data about their name, height, weight, what language they speak, how to say hello to them, and more.

```
let dog = { name : 'Spot', breed : 'Dalmatian' };
```

To retrieve the information stored in the object, you can use the following syntax:

```
dog.name
```

### Constants
Constants are used to store values that are immutable or can't be changed and are created with the keyword const.

```
const daysInWeek = 7;
```

const works in exactly the same way as let, except that you can't give a const a new value. In the following example, the second line would throw an error:
```
const daysInWeek = 7;
daysInWeek = 8;
```
