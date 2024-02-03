# Intro
Preston is learning to read minds, although right now he's kinda just making random guesses. We're going to help him learn by getting him to guess a number in our head between 1 and 10:
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

# Else Statements
We *could* have an if statement to check if he got it right and another if statement if he got it wrong, but a better way is to use an else statement. An else statement works like this:
```js
fill(0, 255, 255);
var hasPancakes = false;

if(hasPancakes){
    text("Yay, pancakes!", 200, 200);
}else{
    text("Aw, no pancakes :(", 200 200):
}
```
The if statement will run **IF** the boolean is true, **ELSE** run the else statement. So in the pancakes example, the text will be sad that there’s no pancakes.
