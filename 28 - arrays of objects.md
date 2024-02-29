# Intro
Remember the object I made for Preston's cat, Oreo? Well I think the other cats feel left out, so I made a program that has all of Preston's cats on it:
```js
var cat = function(x, y, furCol, name){
    //head
    fill(furCol); //remember when I was talking about variables and how you can store colors in variables with the color function?
    ellipse(x, y, 100, 100);
    
    //ears
    //the first 2 values describe one point, the second 2 describe the second point, and the third 2 describe the third point
    triangle(x-47, y-19, x-16, y-44, x-52, y-66);
    triangle(x+47, y-19, x+16, y-44, x+52, y-66);
    
    //eyes
    fill(0, 0, 0);
    ellipse(x-19, y-13, 20, 20);
    ellipse(x+19, y-13, 20, 20);
    
    //whiskers
    strokeWeight(2);
    line(x-24, y+5, x-7, y+13);
    line(x-24, y+19, x-7, y+13);
    line(x+24, y+5, x+7, y+13);
    line(x+24, y+19, x+7, y+13);
    
    //mouth
    strokeWeight(5);
    line(x, y, x, y+20);
    line(x-15, y+26, x, y+20);
    line(x+15, y+26, x, y+20);

    //name
    fill(0, 0, 0);
    text(name, x-30, y-58);
};
```

