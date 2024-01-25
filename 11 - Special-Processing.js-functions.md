# Draw function
Remember when we were talking about the draw function, and how we can animate with it? You might be thinking "why does the draw function draw every frame, but the other ones don't?". Well, Processing.js behind the scenes has this code:
```
var draw = function(){
  //blank and boring
};

//no, drawEveryFrame isn't an actual function. If you try using it, the program will error out. This is just to show you what's going on.
drawOnEveryFrame(draw);
```
When we do "draw = function(){...}", we're overriding the draw function that Processing.js has built in, and that's what allows it to be ran every time.

# Are there other functions like draw?
Glad you asked! There are in fact several. Here are the most important ones:
```
keyPressed = function(){
  //runs every time a key on the keyboard is pressed.
};
keyReleased = function(){
  //runs every time a key on the keyboard is released.
};
mousePressed = function(){
  //runs every time a mouse button is pressed.
};
mouseReleased = function(){
  //runs every time a mouse button is released.
};
```

# Special variables
Just like how there's special functions like draw and mousePressed, there's also special variables! Here's
