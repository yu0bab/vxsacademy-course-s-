# What Are Functions?
So let's talk about something you already know but don't know the name of: functions.
We've been using functions this whole time! Rect, ellipse, line, and text are all examples of functions.
They are chunks of code that were given a name so we can use them more easily. Behind the scenes, the rect function is actually just 4 lines. Aren't you glad that you only have to type "rect(200, 200, 20, 20);" instead of 4 lines?

In a way, we use functions in our daily lives. When you make breakfast, you probably get a bowl, pour cereal, pour milk, and get a spoon to eat it with. That’s a function, because a list of instructions grouped together and given a name: making breakfast. You don’t have to say the entire procedure, because everyone will understand you if you say "making breakfast"

# Custom Functions
I want to make a clone of Preston. **[add the code for him here]** I could copy and paste the code for him, but what if I want to make a change to both? And what if I want to add a third or fourth Preston? It'd be nice if we could make our own functions to make this easier.

Guess what, we *can* have custom functions! Here's how we do it:
```
//It's like the draw function when we were doing animation, but with var at the beginning, and a different name. We have var at the beginning because functions are technically a variable.
var functionName = function(){
    //put your code here
};
```
We're going to make a function that draws Preston, like so:
```
var drawPreston = function(){
    //code for Preston
};
```
Try out that code. You'll notice that nothing happens, because we need to tell the computer to actually use the drawPreston function (programmers like saying that we call, or run, the function). We do that in the same way we run the rect or ellipse function:
```
//make sure that you have the "var drawPreston = ..." part before this, or else the computer won't get what you mean
drawPreston();
```
Hey cool, it's drawing Preston again! And what's better, we can run the function again to get 2 Prestons. But if you were to try that (and I would encourage you to), you would notice that you only see 1 Preston. Why? Well, think about it: we didn’t change X or Y for the second Preston, so they were drawn on top of each other. How can we change the X and Y values?

# Parameters
For the rect and ellipse functions, we can put in some numbers describing the position and size of them. With fill and stroke, we can put in 3 numbers describing the color we want. The numbers you put into functions are called parameters. This is how you can make parameters for custom functions:
```
var functionName = function(x, y){}
```
