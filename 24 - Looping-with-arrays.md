# Intro
In the last lesson, we made a list of Preston's favorite activities. Here's the code:
```js
var favActivities = ["Programming", "Math", "Science", "Art", "Gaming"];
fill(0, 0, 0);
text("Preston likes " + favActivities.length + " things.", 10, 40);
text("Preston likes " + favActivities[0], 10, 60);
text("Preston likes " + favActivities[1], 10, 80);
text("Preston likes " + favActivities[2], 10, 100);
text("Preston likes " + favActivities[3], 10, 120);
text("Preston likes " + favActivities[4], 10, 140);
```
But let's say that Preston finds an interest in music all of a sudden. Or he lost interest in Art. I'd have to add or remove a text function and change the values. But I don't want to because I'm lazy. Well I see a lot of repetition, maybe we can use a for loop?

# Looping with Arrays

