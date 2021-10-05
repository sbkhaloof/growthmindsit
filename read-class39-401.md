# Redux - Additional Topics

# Review, Research, and Discussion

1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application? The most ‘redux-like’ way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method of a Higher Order Component that wraps your app.
2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer? export the state from your reducer 

## Document the following Vocabulary Terms

- middleware :functions that have access to the request object ( req ), the response object ( res ), and the next function in the application’s request-response cycle.
- thunk : is a middleware that allows you to call the action creators that return a function(thunk) which takes the store’s dispatch method as the argument and which is afterwards used to dispatch the synchronous action after the API or side effects has been finished.

## Preparation Materials

The Redux Toolkit package was developed to be the new standard way to write Redux code, handling three major concerns about Redux itself...

1. "Configuring a Redux store is too complicated"
2. "I have to add a lot of packages to get Redux to do anything useful"
3. "Redux requires too much boilerplate code"

RTK Query is a powerful data fetching and caching tool. It is designed to simplify common cases for loading data in a web application, eliminating the need to hand-write data fetching & caching logic yourself.

RTK Query is an optional addon included in the Redux Toolkit package, and its functionality is built on top of the other APIs in Redux Toolkit.

[Redux Toolkit (RTK)](https://redux-toolkit.js.org/)
[Tutorial](https://redux-toolkit.js.org/tutorials/overview)

[Github view](https://github.com/sbkhaloof/growthmindsit)