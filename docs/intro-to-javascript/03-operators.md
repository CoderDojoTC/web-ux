# Operators
JavaScript operators allow us to perform tests, do math, join strings together, and other such things.

First let's look at arithmetic operators, for example:

Addition	`console.log(6 + 9);`

Subtraction	`console.log(20 - 15);`

Multiplication	`console.log(3 * 7);`

Division	`console.log(10 / 5);`

You can also use the + operator to join text strings together (in programming, this is called concatenation).
```
let name = 'Bingo';
console.log(name);
let hello = ' says hello!';
console.log(hello);
let greeting = name + hello;
console.log(greeting);
```
There are also some shortcut operators available, called augmented assignment operators. For example, if you want to simply add a new text string to an existing one and return the result, you could do this:
```
let name = 'Bingo';
name += ' says hello!';
console.log(name);
```
When we are running true/false tests (for example inside conditionals — see next lesson) we use comparison operators. For example:

`===`	Tests strict equality (is it exactly the same?)	
```
5 === 2 + 4; // false
'Chris' === 'Bob'; // false
5 === 2 + 3; // true
2 === '2'; // false; number versus string
```
`!==` Tests	non-equality (is it not the same?)	
```
5 !== 2 + 4; // true
'Chris' !== 'Bob'; // true
5 !== 2 + 3; // false
2 !== '2'; // true; number versus string
```
`<` Tests	less than, `<=`	less than or equal
```
6 < 10; // true
20 < 10; // false
10 < 10; // false
10 <= 10; // true
```
`>`	Tests greater than, `>=` greater than or equal
```
6 > 10; // false
20 > 10;  // true
10 > 10; // false
10 >= 10; // true
```
