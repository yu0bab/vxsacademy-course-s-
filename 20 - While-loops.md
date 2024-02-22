# Intro
I have this function that draws preston at any place on the screen (you might remember it when we were talking about functions):
```js
var drawPreston = function(x, y){
    fill(0, 0, 0); //face color
    ellipse(x, y, 100, 100); //face
    
    fill(255, 255, 255); //eye color
    ellipse(x-20, y-10, 20, 20); //eyes
    ellipse(x+20, y-10, 20, 20);
    ellipse(x, y+20, 40, 20);
};
```
One Preston is great, and two is better, but what I want is an entire army of them so I can take over the world! Mwahahahaha >:).
Ok that was a joke, I don't plan to take over the world, but how would I draw a bunch of prestons? Sure, I could just call the drawPreston function a bunch of times, but I'm lazy. How can we get the computer to do all that for us?


# While loops
While loops are a very handy tool. They repeat code *while* a condition is true (hence the name). Here's an example of one:
```
var x = 0; //x starts at 0

//repeat while x < 10
while(x < 10){
    println(x);
    x ++; //increment x by 1
}
println("value of x after the loop: " + x);
```
Try that code. It reapeats the code inside 10 times. That's pretty cool!
