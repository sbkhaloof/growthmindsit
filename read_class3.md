# Passing Functions as Props
1- What does .map() return?
### The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.the array will be the same lenght of the origin one .
2- if I want to loop through an array and display each value in JSX, how do I do that in React?
### I can do that by using map() array metod .
3- Each list item needs a unique _key___.
4- What is the purpose of a key? 
###  Keys are necessary to improve performance of our React app ;Keys help React identify which items have changed (added/removed/re-ordered). To give a unique identity to every element inside the array, a key is required.
## How to Use the Spread Operator (…) in JavaScript
### The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
## What is the spread operator? 
### The spread operator is a new addition to the set of operators in JavaScript ES6. It takes in an iterable (e.g an array) and expands it into individual elements. The spread operator is commonly used to make shallow copies of JS objects. Using this operator makes the code concise and enhances its readability.
## What is ... used for?
### The spread syntax “spreads” the array into separate arguments.
## What else can … do?
+ Copying an array
+ Concatenating or combining arrays
+ Using Math functions
+ Using an array as arguments
+ Adding an item to a list
+ Adding to state in React
+ Combining objects
+ Converting NodeList to an array
## Give an example of using the spread operator to combine two arrays.
### Const myArray = [1,2,3]
### const yourArray = [4,5,6]
### const ourArray = [...myArray,...yourArray]
## Give an example of using the spread operator to add a new item to an array.
### const fewLett = ['a','b','c']
### const fewMoreLett = ['d', 'e', ...fewLett]
### console.log(fewMoreLett) //  Array(5)
## Give an example of using the spread operator to combine two objects into one
### const objectOne = {hello: "🤪"}
### const objectTwo = {world: "🐻"}
### const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
### console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
### const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
### objectFour.laugh() // 😂😂😂😂😂
## How to Pass Functions Between Components? pass a functions as stat to child components .and there are several ways to make sure functions have access to component attributes like this.props and this.state
## In your own words, what does the increment function do? it's for maching the name with the names in the array of object if it simmilar will the counter value be counter+1 .
## How can you pass a method from a parent component into a child component? Passing method as a prop.
## How does the child component invoke a method that was passed to it from a parent component?

