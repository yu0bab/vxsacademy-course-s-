# Intro
The little stick figure I made wanted to go to the moon, so I gave him a rocket!
I even added a y variable so we can change the height the rocket's at:
```
var y = 100;

//rocket
fill(222, 139, 22);
rect(150, 125+y, 100, 165); //rocket body
fill(255, 255, 255);
ellipse(200, 190+y, 70, 70); //window
stroke(115, 75, 7);
strokeWeight(10);
line(200, 25+y, 150, 130+y); //top part
line(200, 25+y, 250, 130+y);

//stickman
noStroke();
fill(0, 0, 0);
ellipse(200, 190+y, 50, 50); //face

fill(255, 255, 255);
ellipse(190, 185+y, 10, 10); //eyes
ellipse(210, 185+y, 10, 10);
ellipse(200, 200+y, 20, 10);
```
You can view it by copying and pasting the code [here](https://vxsacademy.org/computer-programming/new/pjs).
If you mess with the y variable, it kinda looks like he's going up (or down, depending on the way you change
the y variable) But how do we actually launch the rocket? So far we can only draw still pictures. We need a
way to draw a bunch of pictures every second, and change the y variable a little bit every time, so it can
be animated.

# The Draw function
How we make animations in Processing.js is by using the Draw function. You use it like this:
```
draw = function(){
  //anything you want to draw a bunch of times a second goes here.
};
```
We'll talk about it later, but a function stores a group of code we can use later, like a variable. The "draw"
is a special one that will allow us to animate our rocket. So put the rocket and stickman inside a draw function
(and leave "var y = 100;" outside). Nothing happens. That's because we're not changing the y variable, so the
rocket stays in place.

# Updating variables
