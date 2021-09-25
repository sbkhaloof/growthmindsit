# Context API

![](https://cdn.hackernoon.com/images/gp1d3vsm.jpg)

## Review, Research, and Discussion

+ Describe use cases useState() vs useReducer()

useState is a Basic Hook for managing simple state transformation but useReducer used to managing more complex state logic, it is worth noting that useState uses the useReducer internally. This implies that you could use useReducer for everything you can do with useState.
+ Why do custom hooks need the use prefix?

it is a name convention and rules for nameing hook

+ What do custom hooks usually do?

Custom React hooks can help us with some very important principles of good software architecture, such as code readability, separation of concerns, and avoiding code duplication.
In this article we'll see how we can encapsulate fetch calls, logic, caching, and component state, all inside a custom React Hook.

React Hooks allow us to use the component’s state, to hook into the component’s lifecycle, and to use other React features in functional components, like we usually do in class components.

While custom React Hooks are just Javascript functions, we can actually use other hooks inside them. Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

+ Using any list of custom hooks, research and name one that you think will be useful in your applications

1. useMedia hook:is a React sensor hook that tracks the state of a CSS media query. We all know the importance of the media queries and how much important is responsiveness for any site.

2. use-onClickOutside hook: An outside click is a way to know if the user clicks everything but a specific component. You may have seen this behavior when opening a dropdown menu or a modal or a dropdown list.

+ Describe how a hook that fetches API data might work

this is by using useEffect method inside the component after that , Define your URL ; When the user lands on our page, we want to call the API. In other words, we want to call the API during the mounting part of the component's lifecycle.
Then, let's create an asynchronous function to fetch our data. An asynchronous function is a function that needs to wait after the promise is resolved before continuing. In our case, the function will need to wait after the data is fetched (our promise) before continuing.
then create asynchronous function and put it above in effect hook and call it 

## Document the following Vocabulary Terms

* reducer : A reducer is a function that determines changes to an application’s state. It uses the action it receives to determine this change.

## Preparation Materials

### Context :





[Github view](https://github.com/sbkhaloof/growthmindsit)