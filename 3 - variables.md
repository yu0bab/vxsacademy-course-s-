# Intro to Variables
Hey, you wanna see something cool I made?
```
stroke(0, 0, 0);
strokeWeight(20);
line(200, 200, 100, 250); //left legs
line(200, 200, 83, 200);
line(200, 200, 100, 150);
line(200, 200, 143, 110);

line(200, 200, 300, 250); //right legs
line(200, 200, 318, 200);
line(200, 200, 300, 150);
line(200, 200, 262, 110);

fill(0, 0, 0);
ellipse(200, 200, 100, 100); //body

fill(255, 255, 255);
noStroke();
ellipse(180, 210, 20, 20); //eyes
ellipse(220, 210, 20, 20);
ellipse(200, 235, 25, 15); //mouth
```
It's a spider! You can see him properly if you copy and paste the code [here](https://vxsacademy.org/computer-programming/new/pjs)
Hmm, actually I want the eyes to be bigger (going for a cute spider). So I'll
change them like this:
```
ellipse(180, 210, 30, 30); //eyes
ellipse(220, 210, 30, 30);
```
No, a bit bigger:
```
ellipse(180, 210, 50, 50); //eyes
ellipse(220, 210, 50, 50);
```
And now that's too big. This is a bit of a pain, because I have to change 4
numbers every single time I want to make a change. It'd be nice if I only had
to change just one number to control them all. Oh wait, there is a way to do
that, and that's what this lesson's all about!

# Variables
Variables in programming are a way to store things so we can use them later on,
which is useful if you're going to use something over and over again, like in
the example with the spider. How you make a variable is like this:
```
var variableName = 1;
//The = symbol in programing basically means "assign", unlike in math where it means
//"equals". So "var variableName = 1;" means "make variableName and assign it to 1"
```
So for our spider eyes, we can make a variable called "eyesSize" and set it to
the size we want, and then use that size for the eyes. Like this:
```
var eyesSize = 35;
ellipse(180, 210, eyesSize, eyesSize); //eyes
ellipse(220, 210, eyesSize, eyesSize);
```
Ah, much better!

Computers read the code top to down, so make sure you make the variable before
you use it:
```
//The computer is thinking "Uh oh, the variable 'eyesSize' wasn't made yet, so
//I don't know what that means".
ellipse(180, 210, eyesSize, eyesSize);
ellipse(220, 210, eyesSize, eyesSize);

var eyesSize = 35;
```

Also, I want to be able to easily control the location of the eyes. Variables, to the rescue!
```
var eyesSize = 35;
var eyeHeight = 210;

ellipse(180, eyeHeight, eyesSize, eyesSize); //eyes
ellipse(220, eyeHeight, eyesSize, eyesSize);
```
