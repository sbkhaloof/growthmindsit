# Application State with Redux

## Review, Research, and Discussion

1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”
2. Explain 3rd party cookies... , are cookies that are stored under a different domain than you are currently visiting. They are mostly used to track users between websites and display more relevant ads between websites. Another good example is a support chat functionality provided by a 3rd party service.
3. How do pixel tags work? You add the tracking pixel using a code in your site’s HTML code or email, which contains an external link to the pixel server. When someone visits your website, the HTML code is processed by their browser, which follows the link and opens the hidden graphic. This action is identified and recorded in the server’s log files. This method allows for different information about the visitor to be transmitted.

[What Is a Tracking Pixel and How It Works?](https://whatagraph.com/blog/articles/tracking-pixel)


## Document the following Vocabulary Terms

cookies : are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.
authorization : is a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features.
access control : is a security technique that regulates who or what can view or use resources in a computing environment. It is a fundamental concept in security that minimizes risk to the business or organization.
conditional rendering :  refers to the process of delivering elements and components based on certain conditions.

## Preparation Materials

What is Redux?

Redux is an open-source library to improve the predictability of the state in a JavaScript application. It is an independent library. It is commonly used with other libraries like React and Angular for better state management of the application. Redux was created by Dan Abramov in 2015 to handle complex state management in an efficient way.

![](https://cdn-media-1.freecodecamp.org/images/1*VLQNO9Apn9qfm6BPYXG8TA.png)

## Redux Store:

As we discussed earlier, the main purpose of Redux is to provide predictable state management in our applications. Redux achieves this by having a single source of truth, that is a single state tree. The state tree is a simple JavaScript object which holds the whole state of our application. There are only a few ways to interact with the state. And this makes it easy for us to debug or track our state.

Rule #1 — Single source of truth

The state of your whole application is stored in an object tree within a single store.

The ways you can interact with a state tree are:

1. Getting the state
2. Listening to the changes in the state
3. Updating the state

A store is a single unit that holds the state tree and the methods to interact with the state tree. There is no other way to interact with a state inside the store except through these given methods.

![](https://cdn-media-1.freecodecamp.org/images/cDBhHN7x5f-p6JRrZ-1ekpbDx7s0aW4j3jUr)

Let’s talk about the methods a store gives us to interact with the state.

getState() — Returns the current state of the application.

dispatch(action) — The only way to update a state is by dispatching an action and dispatch(action) serves the purpose. 

subscribe(listener) — The purpose of this method is to listen for the state changes. Every time a state is changed, it will be called and will return the updated state.

replaceReducer(nextReducer) — Replaces the reducer currently used by the store to calculate the state.

## Updating state in the application:
The only way to update a state is to dispatch an action. This is the 2nd rule.

Rule #2 — State is read-only

An action is a plain JavaScript object to keep track of the specific event taking place in the application. What makes it special is a ‘type’ property which is a necessary part of it.

Rule#3 — Changes are made with pure functions

Magic happens here. We need a simple pure function, which, as a parameter, takes the current state of the application and an action to perform on the state, and then returns the updated state. These functions are called reducers.

[An intro to Redux and how state is updated in a Redux application](https://www.freecodecamp.org/news/an-intro-to-redux-and-how-state-is-updated-in-a-redux-application-839c8334d1b1/)

[Dan Abramov Redux Tutorials](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)

[Github view](https://github.com/sbkhaloof/growthmindsit)
