# Intro
I want you to get plenty of practice with if statements, because they're very useful, but can get complicated fast.
So let's make something that is somewhat simple, like a button! Before I show you how, try to make a button yourself, and make something happen when you click it.

# Button
First, let's make a button to click:
```js
fill(13, 49, 117);
rect(100, 300, 200, 100); //button

fill(255);
textSize(50);
text("Click Me", 110, 370); //text
```
Not the most interesting button in the world, but it'll do. Now we need to make the functionality of the button, the most important part.
How do we do that? Well, clicking on a button means that we clicked, and our mouse was over the button. Detecting if we clicked is easy, you just use `mouseIsPressed`.
But what about detecting if the mouse is over the button? Well, we know that everywhere on the button has an X value greater than 100 (because the x value of the button is 100), so let's start there.
```js
if(mouseX > 100){
  
}
