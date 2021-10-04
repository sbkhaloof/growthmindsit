# Redux - Asynchronous Actions

## Review, Research, and Discussion

1. How granular should your reducers be? They should be as granular as possible in order to enhance UI performance. You should make as few components render on state change as possible.
2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched ? Each time an action is dispatched, every connected component will be notified, and as a result all of the selectors used by those connected components must be re-evaluated, and no matter what we pass to dispatch, it is still a single action, and many reducers can react to a single actions, a single reducer can react to multiple actions.
3. Name a strategy for preventing the above ? Redux Thunk middleware

## Document the following Vocabulary Terms

+ store : is an object that holds the global state of your application.
+ combined reducers :helper function combines multiple reducers into one function, which can be passed to createStore and allows you to easily access them throughout your application.

## Preparation Materials

By default, Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.

There are two very popular middleware libraries that allow for side effects and asynchronous actions:
1. Redux Thunk .
2. Redux Saga

Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

![](https://res.cloudinary.com/practicaldev/image/fetch/s--WMHUONcg--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/3psu9opx7qovkdh4dkx8.png)

Adding redux-thunk:

> npm install redux-thunk@2.3.0

>Now apply the middleware when creating your app’s store using Redux’s applyMiddleware.

```import { applyMiddleware } from 'redux';```

```import thunk from 'redux-thunk';```

Using Redux Thunk in a Sample Application

The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.

[async actions](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)

[thunk middleware](https://github.com/reduxjs/redux-thunk)

[redux thunk](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)

[Github view](https://github.com/sbkhaloof/growthmindsit)