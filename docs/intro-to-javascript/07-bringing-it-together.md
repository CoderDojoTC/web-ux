# Bring it all together
Create a new project in Repl.it or Glitch and place the following div element in the body of the index.html file:
```
    <div>
      <input type="text" id="name" class="nameField">
      <button class="greet">
        Greet
      </button>
    </div>
```
This will give us a text field and a button that we can bind Javascript to.

Add the following code to the script.js file.

```
const nameField = document.querySelector('.nameField');
const greet = document.querySelector('.greet');
function issueGreeting(){
  let name = nameField.value;
  let hello = 'Hello ';
  let greeting = hello + name + '!';
  alert(greeting);
}

greet.addEventListener('click', issueGreeting);
```
Note: document.querySelector('.someClass') is an easy way to refer to html elements using an identifying class, we won't get into the mechanics during this intro course

Now view your site. Enter a name in the text field and click the 'Greet' button. You should see an alert pop up greeting you by name.

For a more interesting example to walk through, enter the following html into your body tag:
```
<h1>Number guessing game</h1>

<p>We have selected a random number between 1 and 100. See if you can guess it in 10 turns or fewer. We'll tell you if your guess was too high or too low.</p>

<div class="form">
  <label for="guessField">Enter a guess: </label>
  <input type="text" id="guessField" class="guessField">
  <input type="submit" value="Submit guess" class="guessSubmit">
</div>

<div class="resultParas">
  <p class="guesses"></p>
  <p class="lastResult"></p>
  <p class="lowOrHi"></p>
</div>
```
And the following Javascript into your script.js file:
```
let randomNumber = Math.floor(Math.random() * 100) + 1;

const guesses = document.querySelector('.guesses');
const lastResult = document.querySelector('.lastResult');
const lowOrHi = document.querySelector('.lowOrHi');

const guessSubmit = document.querySelector('.guessSubmit');
const guessField = document.querySelector('.guessField');

let guessCount = 1;
let resetButton;

function checkGuess() {
  let userGuess = Number(guessField.value);
  if (guessCount === 1) {
    guesses.textContent = 'Previous guesses: ';
  }
  guesses.textContent += userGuess + ' ';
 
  if (userGuess === randomNumber) {
    lastResult.textContent = 'Congratulations! You got it right!';
    lastResult.style.backgroundColor = 'green';
    lowOrHi.textContent = '';
    setGameOver();
  } else if (guessCount === 10) {
    lastResult.textContent = '!!!GAME OVER!!!';
    setGameOver();
  } else {
    lastResult.textContent = 'Wrong!';
    lastResult.style.backgroundColor = 'red';
    if(userGuess < randomNumber) {
      lowOrHi.textContent = 'Last guess was too low!';
    } else if(userGuess > randomNumber) {
      lowOrHi.textContent = 'Last guess was too high!';
    }
  }
 
  guessCount++;
  guessField.value = '';
  guessField.focus();
}

function setGameOver() {
  guessField.disabled = true;
  guessSubmit.disabled = true;
}

guessSubmit.addEventListener('click', checkGuess);
```
