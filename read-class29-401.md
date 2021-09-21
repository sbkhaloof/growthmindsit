# Advanced State with Reducers

## Review, Research, and Discussion

+ How can we ensure that an effect hook runs only once?If we pass an empty array [] , it just renders the component only once like componentDidMount .
+ Can useState() update more than one state variable at the same time? we could combine the all the states into one state object and then we could do one setState call and there will only be one render.
+ Is useState() synchronous? useState and setState both are asynchronous. Even though they are asynchronous, the useState and setState functions do not return promises. Therefore we cannot attach a then handler to it or use async/await to get the updated state values.

## Document the following Vocabulary Terms

+ State Hook: A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later.
+ Component Lifecycle: Every React Component has a lifecycle of its own, lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component’s existence. … A React Component can go through four stages of its life

## Preparation Materials

### useReducer

### useReducer() is a method from the React Hooks API, similar to useState but gives you more control to manage the state. It takes a reducer function and initial state as arguments and returns the state and dispatch method

### 3 Reasons to Use It

1. Next state depends on the previous.
2. Complex state shape
3. Easy to test

### useReducer() is an alternative to useState() which gives you more control over the state management and can make testing easier. All the cases can be done with useState() method, so in conclusion, use the method that you are comfortable with, and it is easier to understand for you and colleagues

[Github view](https://github.com/sbkhaloof/growthmindsit)
