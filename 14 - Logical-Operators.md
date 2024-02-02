# Logical Operators
In the previous article, I talked about booleans and how to make them with comparison symbols (like < and ===). But let's say we want to combine booleans together, like how you can combine numbers together. How do we do that? One of the ways we can do that is checking if one boolean OR another is true. How we do that is by typing "||" (hold shift and press the \ key, which should be above the enter key).
```js
//It's looking to see if one OR the other boolean is true

if(false || false){
  //none of them are true, so this won't run
}

if(true || false){
  //one of them is true, so this will run
}

if(false || true){
  //one of them is true, so this will run
}

if(true || true){
  //both true, so this will run
}
```
Another one checks if both the first AND the second booleans are true. We do that by typing "&&" (hold shift and press the 7 key).
```js
//It's looking to see if both the first AND the second booleans are true

if(false && false){
  //none of them are true, so this won't run
}

if(true && false){
  //only one of them are true, so this won't run
}

if(false && true){
  //only one of them is true, so this won't run
}

if(true && true){
  //both are true, so this will run
}
```

# Example
Remember the portal I made, and how I said that there's a problem with the code? Here's the code for it in case you forgot:
```js
var ballX = 200;
var ballSpeed = 2;

draw = function(){
    background(255, 255, 255);

    strokeWeight(1);
    fill(125);
    ellipse(ballX, 200, 60, 60); //ball

    ballX += ballSpeed; //move the ball according to the speed

    if(ballX > 400){ //if the ball goes into the right portal, go to the left portal
        ballX = 0;
    }
    if(ballX < 0){ //if the ball goes into the left portal, go to the right portal
        ballX = 400;
    }

    stroke(0, 0, 255);
    strokeWeight(20);
    line(390, 100, 390, 300); //right portal

    stroke(0, 255, 0);
    line(10, 100, 10, 300); //left portal
};
```
Let's say that we want the ball 
