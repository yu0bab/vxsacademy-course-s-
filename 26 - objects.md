# intro
Preston found a cool book to read: Not so Fantastic Bugs and Where to Find Them (it's a made up book, so don't go looking for it). Here's some info on the book:
```js
var bookTitle = "Not so Fantastic Bugs and Where to Find Them";
var bookDescription = "Lots of tips and tricks on how to debug your Javascript programs. For debugging C++ programs, try the book 'How to smash sea bugs.'.";

//the rating is on a scale of 1 to 5
var averageRating = 3;
var prestonsRating = 5;
var bookRatings = [
    "1/5. It doesn't talk about bugs at all, just programming stuff. I want a refund!",
    "5/5. This book is amazing! Taught me a lot about debugging.",
    "4/5. I was hoping it was going to talk about insects, but I'm a programmer so I still found it enjoyable.",
    "2/5. This book is WAY below my level. I don't even know why I got it, I work for NASA lol"
];

var author = "Bobert Rossert"; //No, not the Bobert we all know and love. A different bobert.
var numOfPages = 271828;
var audience = "Not for people who work for NASA";
var genre = "Science nonfiction. Not to be confused with science fiction.";
```
Sounds like a cool book! But hmm, all of these variables are talking about the same thing: the book. I think there should be a better way to describe all these variables since they're talking about the same thing. Luckily, there is another way to describe them: objects!

# Objects
And object in Javascript is a way of storing multiple values in one variable, like arrays. But instead of a list of things like arrays, an object stores properties of things. Let me show you how to make one with an example:
```js
var preston = {
    //These 3 things, name, age, and height, are all properties
    name: "Preston John Smith",
    age: 999999999, //he has existed before the creation of time
    height: 7, //in feet
};
```
We can make an object for preston's book:
```js
var prestonsBook = {
    title: "Not so Fantastic Bugs and Where to Find Them",
    description: "Lots of tips and tricks on how to debug your Javascript programs. For debugging C++ programs, try the book 'How to smash sea bugs.'.",

    //yup, that's right, you can put object inside of objects
    ratings: {
        average: 3,
        preston: 5,
        array: [
            "1/5. It doesn't talk about bugs at all, just programming stuff. I want a refund!",
            "5/5. This book is amazing! Taught me a lot about debugging.",
            "4/5. I was hoping it was going to talk about insects, but I'm a programmer so I still found it enjoyable.",
            "2/5. This book is WAY below my level. I don't even know why I got it, I work for NASA lol"
        ]
    },

    author: "Bobert Rossert",
    numOfPages: 271828,
    audience: "Not for people who work for NASA",
    genre: "Science nonfiction. Not to be confused with science fiction."
};
```
Ok so that's great and all, but how do I access this information on the book? Remember how you get the length of an array? You type the array name and then ".length" at the end. The reason why is because arrays are secretly objects.
