# Intro
Preston is learning to read minds, although right now he's kinda just making random guesses. We're going to help him learn by getting him to guess a number between 1 and 10:
```js
var ourNumber = 6; //change this to whatever number you want him to guess.
var hisGuess = random(1, 10); //the random function generates a random number between 1 and 10
fill(0, 0, 0);
text("Is your number " + hisGuess + "?", 200, 200);
```
If you run that code, you'll see that it's not a whole number, but we want him to guess whole numbers. We can use the round function, which will round it to the nearest whole number:
```js
//code
```
Ok so he's guessing random whole numbers. Now we need to check if he got it right, and say he got it right if he did, otherwise tell him to guess again.
