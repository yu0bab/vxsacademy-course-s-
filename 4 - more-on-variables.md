# Math with variables
In the last article, I made a stickman and controlled the arm and shoulder heights with variables. Here's the code:
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

//yay variables!
var armHeight = 260;
var shoulderHeight = 140;

line(160, armHeight, 200, shoulderHeight); //arms
line(240, armHeight, 200, shoulderHeight);

line(160, 380, 200, 280); //legs
line(240, 380, 200, 280);
```
