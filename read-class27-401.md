# useState() Hook

## Review, Research, and Discussion

+ How does React differ from vanilla JS/HTML/CSS? React breaks down the UI into smaller and reusable components that can move around data amongst each other. This breaking down of the UI is what gives React an edge over Vanilla JS. This is where React comes in with a great feature i.e its own virtual DOM. The virtual DOM is a shortcut to bypass the manual work.
+ What is the primary difference between a function component and a class component? A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional

## Document the following Vocabulary Terms

+ Functional Components : basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI.
+ Children / Child Components :children is a special property of React components which contains any child elements defined within the component

## Preparation Materials

### What is a Hook? are functions that let you “hook into” React state and lifecycle features from function components.  For example, useState is a Hook that lets you add React state to function components

### React provides a few built-in Hooks like useState. You can also create your own Hooks to reuse stateful behavior between different components.

### The Effect Hook, useEffect, adds the ability to perform side effects from a function component. It serves the same purpose as componentDidMount, componentDidUpdate, and componentWillUnmount in React classes,

#### When you call useEffect, you’re telling React to run your “effect” function after flushing changes to the DOM. Effects are declared inside the component so they have access to its props and state. By default, React runs the effects after every render — including the first render. 

### Declaring a State Variable: by  call the useState Hook directly inside our component

### useState returns a pair: the current state value and a function that lets you update it

### ✌ Rules of Hook

+ Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.

+ Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. (There is just one other valid place to call Hooks — your own custom Hooks.



[making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

[the state hook](https://reactjs.org/docs/hooks-state.html)

[hooks api](https://reactjs.org/docs/hooks-overview.html)
[hooks api reference](https://reactjs.org/docs/hooks-reference.html)

[Github view](https://github.com/sbkhaloof/growthmindsit)
