# Intro
Remember the program from last lesson that draws Preston's cats onto the screen? If not, here's the code:
```js
var drawCat = function(catObj){ //obj stands for object
    var x = catObj.x;
    var y = catObj.y;
    var furCol = catObj.furCol; //furCol is short for "fur color"
    var name = catObj.name;

    strokeWeight(1); //head
    fill(furCol); //remember when I was talking about variables and how you can store colors in variables with the color function?
    ellipse(x, y, 100, 100);
    
    //ears
    //the first 2 values describe one point, the second 2 describe the second point, and the third 2 describe the third point
    triangle(x-47, y-19, x-16, y-44, x-52, y-66);
    triangle(x+47, y-19, x+16, y-44, x+52, y-66);
    
    fill(0, 0, 0); //eyes
    ellipse(x-19, y-13, 20, 20);
    ellipse(x+19, y-13, 20, 20);
    
    strokeWeight(2); //whiskers
    line(x-24, y+5, x-7, y+13);
    line(x-24, y+19, x-7, y+13);
    line(x+24, y+5, x+7, y+13);
    line(x+24, y+19, x+7, y+13);
    
    strokeWeight(5); //mouth
    line(x, y, x, y+20);
    line(x-15, y+26, x, y+20);
    line(x+15, y+26, x, y+20);

    fill(0, 0, 0); //name
    text(name, x-34, y-58);
};

var cats = [
    {
        x: 100,
        y: 100,
        color: color(66, 41, 20),
        name: "Oreo"
    },
    {
        x: 100,
        y: 300,
        color: color(92, 47, 5),
        name: "Chester"
    },
    {
        x: 300,
        y: 100,
        color: color(191, 97, 15),
        name: "Jasper"
    },
    {
        x: 300,
        y: 300,
        color: color(90, 99, 32),
        name: "Thomas"
    }
];

cats.forEach(function(v, i){
    drawCat(v);
});
```
Hmm... look at the cats array. Each cat is basically the same when it comes to code: it's just an X and Y, a color, and a name. 
