# Reading 3

## Lists and Keys in React

### What does .map() return?

.map() will return a new array.

### If I want to loop through an array and display each value in JSX, how do I do that in React?

You can place the variable that is being added to the array within curly brackets, within a JSX tag. For example: `<li>{value}</li>`

### What is the purpose of a key?

Each list item needs a unique key.

Keys signal to react which elements are which, and help keep track of when items are removed or added. You can add an id as the index when mapping through an array, for example. But only if the order of the items will not change. You can also use the id that is on the individual item of data. 

## Spread Operator

### What is the spread operator?
The spread operator is three dots that expands an object into a list of arguments. 

### List 4 things that the spread operator can do.

1. It can take values in an array and separate them out to make it easier to run methods such as Math.max.
1. You can use it to copy or combine arrays
1. It helps you use arrays as arguments
1. A good tool to add items to lists

### Give an example of using the spread operator to combine two arrays.

~~~javaScript 
const halfArray = ['one', 'two']
const fullArray = [...halfArray, 'three', 'four']

### Give an example of using the spread operator to add a new item to an array.

~~~javaScript
const littleArray = ['happy', 'sad', 'glad']
const mediumArray = ['excited', 'sorry', ...littleArray]
~~~

### Give an example of using the spread operator to combine two objects into one.

~~~javaScript
const firstObject = {name: 'peyton', place: 'here'}
const secondObject = {name: 'joe', place: 'there'}

const combined = {...firstObject, ...secondObject}
~~~

[Home](https://peymade.github.io/reading-notes/)