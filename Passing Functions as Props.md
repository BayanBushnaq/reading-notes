# Passing Functions as Props

## React Docs - lists and keys

### What does .map() return?
It should return an modified Array 

### If I want to loop through an array and display each value in JSX, how do I do that in React?
by using foreach function 

### Each list item needs a unique ____.

a key 

### What is the purpose of a key?

 help React identify which items have changed, are added, or are removed.

## The Spread Operator

### What is the spread operator?
 its abuilt in function used to take an array and expands it into individual elements

### List 4 things that the spread operator can do.

- Copying an array.
- Concatenating or combining arrays.
- Using Math functions.
- Using an array as arguments.

### Give an example of using the spread operator to combine two arrays.
[...["ððððĪŠð"]] // Array [ "ððððĪŠð" ]
[..."ððððððĨ°ððĪĐ!"] // Array(9) [ "ð", "ð", "ð", "ð", "ð", "ðĨ°", "ð", "ðĪĐ", "!" ]

const hello = {hello: "ððððĪŠð"}
const world = {world: "ððððððĨ°ððĪĐ!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "ððððĪŠð", world: "ððððððĨ°ððĪĐ!" }

### Give an example of using the spread operator to add a new item to an array.

const fruits = ['ð','ð','ð','ð','ð']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "ð", "ð", "ð", "ð", "ð" ]
fruits[0] = 'ð'
console.log(...[...fruits,'...',...moreFruits]) //  ð ð ð ð ð ... ð ð ð ð ð

### Give an example of using the spread operator to combine two objects into one.

[...["ððððĪŠð"]] // Array [ "ððððĪŠð" ]
[..."ððððððĨ°ððĪĐ!"] // Array(9) [ "ð", "ð", "ð", "ð", "ð", "ðĨ°", "ð", "ðĪĐ", "!" ]

const hello = {hello: "ððððĪŠð"}
const world = {world: "ððððððĨ°ððĪĐ!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "ððððĪŠð", world: "ððððððĨ°ððĪĐ!" }


