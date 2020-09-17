# Conditionals
Conditional statements allow us to represent decision making in JavaScript, like asking a question ("should I eat one cookie or two?")

Let's look at by far the most common type of conditional statement you'll use in JavaScript — the humble if...else statement.

Basic syntax
```
let myCookieCount = 2;
if (myCookieCount >= 1) {
  alert('I will eat a cookie');
} 
else {
  alert('Time to buy more cookies');
}
```

Here we've got:

* The keyword if followed by some parentheses.
* A condition to test, placed inside the parentheses (typically "is this value bigger than this other value?", or "does this value exist?"). The condition makes use of the comparison operators we discussed in the last module and returns true or false.
* A set of curly braces, inside which we have some code — this can be any code we like, and it only runs if the condition returns true.
* The keyword else.
* Another set of curly braces, inside which we have some more code — this can be any code we like, and it only runs if the condition is not true — or in other words, the condition is false.

The last example provided us with two choices, or outcomes — but what if we want more than two?

There is a way to chain on extra choices/outcomes to your if...else — using else if. Each extra choice requires an additional block to put in between if() { ... } and else { ... }
```
let myCookieCount = 10;
if (myCookieCount > 5) {
  alert('I am going to get a stomach ache');
}
else if(myCookieCount >= 1){
  alert('I will eat a cookie');
}
else if(myCookieCount == 0){
  alert('Time to buy more cookies');
}
else {
  alert('How do you have negative cookies?!');
}
```
