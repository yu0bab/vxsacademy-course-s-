# Intro
In the last lesson, we made an object describing Preston's book (keep in mind that it's an imaginary book):
```js
var prestonsBook = {
    title: "Not so Fantastic Bugs and Where to Find Them",
    description: "Lots of tips and tricks on how to debug your Javascript programs. For debugging C++ programs, try the book 'How to smash sea bugs.'.",

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
    numOfPages: 271,
    audience: "Not for people who work for NASA",
    genre: "Science nonfiction. Not to be confused with science fiction."
};
```
Bobert Rossert saw this object describing his book, and he would actually prefer that we include his middle name, Normert, which makes his full name "Bobert Normert Rossert". We could simply edit the code, but if we want to make a book website for example, I doubt authors would want to go into the code to make updates to their book. So how else can we update the author name parameter?

# Modifying Objects
Remember how we update variables, or items in arrays? If not, you do it like this:
```js
var numOfCats = 4; //preston has 4 cats

numOfCats = 5;
```
