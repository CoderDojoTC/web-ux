# Functions
Functions are reusable blocks of code that you can write once and run again and again, saving the need to keep repeating code all the time. This is really useful. There are a number of ways to define functions, but for now we'll concentrate on one simple type. 

Here we have defined a function by using the keyword function, followed by a name, with parentheses put after it. After that we put two curly braces ({ }). Inside the curly braces goes all the code that we want to run whenever we call the function.
When we want to run the code, we type the name of the function followed by the parentheses.
```
function issueGreeting(){
  console.log('Hello ' + name + '! And welcome to our site.');
}
let name = 'Jessie';
issueGreeting();
let name = 'James';
issueGreeting();
```
## Function parameters
We can make the above code even easier using parameters, this allows us to pass values for our function to use, kind of like setting a variable specifically for our function to use.
```
function issueGreeting(name){
  console.log('Hello ' + name + '! And welcome to our site.');
}
issueGreeting('Jessie');
issueGreeting('James');
```
