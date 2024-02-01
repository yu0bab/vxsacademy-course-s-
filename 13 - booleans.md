# Value Types
If you are an artist, you probably know that there are many different tools, and they're used for different things. Pencils are used for drawing, crayons are used for coloring, erasers are used for erasing, brushes are used for painting, tablets are used for digital art and animation, and so on so forth. When you use them together in the right ways, you can make some pretty amazing art (of course, you need other things for great art, like practice, good ideas, references, etc.). Just like with art utensils, there are many programing "utensils" called value types. You already know of a few, like numbers, strings of text, and functions. They're all used for different things, like how text is for words, and functions are to run certain chunks of code. I'm going to teach you a new value type: the Boolean.

# Booleans
Booleans, which were invented by George Boole, are an answer to a yes or no question (maybe isn't an answer tho). Programmers don't call them "yes", and "no", but "true" and "false". If you type "true" or "false" into the coding environment you'll see that they're in color, which means that they're special little fellas. What's the point of booleans? For if statements! You might have guessed that the condition we put in an if statement is secretly a boolean in disguise, which it is. Here's an example of booleans in action:
```js
var programmingIsCool = true; //Yup, we can assign variables to a boolean. We can assign a variable to a value of any type, actually.
if(programmingIsCool){
  //programmingIsCool is true, so it will run through code in here
}

var profCobraIsHuman = false; //I'm prof. Cobra, and I'm not human, but a snake-droid.
if(profCobraIsHuman){
  //profCobraIsHuman is false, so nothing will run in here
}
```
And like in math how you have expressions, like 2 + 3 * 5, there's also boolean expressions. We used 2 earlier when making the portals. < and > are boolean expressions. Another one is <=, meaning "less than or equal to". As you might guess, it sees if the number on the left is less than or equal to the one on the right, as so:
```js
if(41 <= 42){
  //41 is less than or equal to 42, so this will run.
}

if(42 <= 42){
  //42 is less than or equal to 42, so this will run.
}

if(43 <= 43){
  //43 is NOT less than or equal to 43, so this will not run.
}
```
