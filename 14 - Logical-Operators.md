# Logical Operators
In the previous article, I talked about booleans and how to make them with comparison symbols (like < and ===). But let's say we want to combine booleans together, like how you can combine numbers together. How do we do that? One of the ways we can do that is checking if one boolean OR another is true. How we do that is by typing "||" (hold shift and press the \ key, which should be above the enter key).
```js
//It's looking to see if one OR the other boolean is true

if(false || false){
  //none of them are true, so this won't run
}

if(true || false){
  //one of them is true, so this will run
}

if(false || true){
  //one of them is true, so this will run
}

if(true || true){
  //both true, so this will run
}
```
Another one checks if both the first AND the second booleans are true. We do that by typing "&&" (hold shift and press the 7 key).
```js
//It's looking to see if both the first AND the second booleans are true

if(false && false){
  //none of them are true, so this won't run
}

if(true && false){
  //only one of them are true, so this won't run
}

if(false && true){
  //only one of them is true, so this won't run
}

if(true && true){
  //both are true, so this will run
}
```

# Example
Remember the portal I made, and how I said that there's a problem with the code?
