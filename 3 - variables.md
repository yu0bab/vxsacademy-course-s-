# Intro to Variables
Hey, you wanna see something cool I made?
```
fill(0, 0, 0); //face color
ellipse(200, 70, 100, 100); //face

fill(255, 255, 255); //eye color
ellipse(180, 60, 20, 20); //eyes
ellipse(220, 60, 20, 20);
ellipse(200, 90, 40, 20);

stroke(0); //body color
strokeWeight(15);
line(200, 120, 200, 280); //body

line(160, 190, 200, 140); //arms
line(240, 190, 200, 140);

line(160, 380, 200, 280); //legs
line(240, 380, 200, 280);
```
It's a stickman! You can see him properly if you copy and paste the code [here](https://vxsacademy.org/computer-programming/new/pjs)
Hmm, actually I want the arms to be longer. So I'll change them like this:
```
line(160, 220, 200, 140); //arms
line(240, 220, 200, 140);
```
No, a bit longer:
```
line(160, 280, 200, 140); //arms
line(240, 280, 200, 140);
```
And now that's too long. This is a bit of a pain, because I have to change both
numbers every single time I want to make a change. It'd be nice if I only had
to change just one number to control them all. Oh wait, there is a way to do
that, and that's what this lesson's all about!

# Variables
Variables in programming are a way to store things so we can use them later on,
which is useful if you're going to use something over and over again, like in
the example with the stickman. How you make a variable is like this:
```
var variableName = 1;
//The = symbol in programing basically means "assign", unlike in math where it means
//"equals". So "var variableName = 1;" means "make variableName and assign it to 1"
```
So for our stickman's arms, we can make a variable called "armHeight" and set it to
the size we want, and then use that size for the eyes. Like this:
```
var armHeight = 260;
line(160, armHeight, 200, 140); //arms
line(240, armHeight, 200, 140);
```
Ah, much better!

Computers read the code top to down, so make sure you make the variable before
you use it:
```
//The computer is thinking "Uh oh, the variable 'eyesSize' wasn't made yet".
line(160, armHeight, 200, 140); //arms
line(240, armHeight, 200, 140);

var armHeight = 260;
```

Also, I want to easily control the height of the shoulders. Variables, to the rescue!
```
var armHeight = 260;
var shoulderHeight = 140;

line(160, armHeight, 200, shoulderHiehgt); //arms
line(240, armHeight, 200, shoulderHiehgt);
```
