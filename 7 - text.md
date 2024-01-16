# Text
About the stickman, I decided to name him "Preston John Smith", or simply "Preston".
I want to make it so that Preston says his name. We can do that by using the text
command. It goes like this:
```
//NOTE: if you don't add the "" around the text you want, the computer will think
//it's supposed to be a variable.
text("text", 200, 200);
```
The first value we put in it is the text we want to display. Us programmers call
text "strings" (we're weird, don't ask). But what about the other two? As always,
mess around with the values first before I tell you.

If you tried the code, you wouldn't have seen anything, because it draws text white by
default. We're drawing white on white, which makes no sense! So you'll have to add a
fill command before the text to make it a different color.

So the second value is the X, and the third is the Y, just like with ellipse and rect.
Although it's actually slightly different. With rect, the X and Y are the top left
corner, but with text, it's the bottom left. Weird, I know, but I don't make the rules.

But the text right now is too small for me. How do we change the size. We just use the
textSize command, like this:
```
//the value is the size we want for the text.
textSize(20);
```

So now I can make Preston say his name!
```
fill(3, 166, 166);
textSize(20);
text("Hi! I'm Preston.", 150, 120);

textSize(15);
text("(so nice to be able to talk now)", 150, 140);

fill(0, 0, 0); //face color
ellipse(200, 200, 100, 100); //face

fill(255, 255, 255); //eye color
ellipse(180, 190, 20, 20); //eyes
ellipse(220, 190, 20, 20);
ellipse(200, 220, 40, 20);
```

# More On Text
Before you ask me, yes, you can put text in a variable.
```
var txt = "I'm in a variable!";
```

If you want to add quotation marks in your text, you can do it like this:
```
var ok = "I'm using \"quotation marks\" in a string";

//the computer thinks that "I'm using " and " in a string" are separate strings of text,
//and "quotation marks" is a variable. I mean, how is it supposed to know otherwise?
var notOk = "I'm using "quotation marks" in a string";
```

And another thing, if you want a string of text to have multiple lines, there's two ways
you can do it:
```
// "\n" adds a new line
var slashNMethod = "this \nhas \nmultiple \nlines";

// doing a \ and then adding a new line is ok
var slashMethod = "this\
has\
multiple\
lines";

//this makes the computer freak out.
var notOk = "this
has
multiple
lines";
```