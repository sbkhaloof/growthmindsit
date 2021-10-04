# Redux - Combined Reducers

## Review, Research, and Discussion

1. Why choose Redux instead of the Context API for global state? Context API Resourceful and ideal for small applications where state changes are minimal but 
Redux Perfect for larger applications where there are high-frequency state updates
2. What is the purpose of a reducer? The reducer takes two parameters: state and action. You need to have an initial value so that when Redux calls the reducer for the first time with undefined, it will return the initialState. Then the function uses a switch statement to determine which type of action it's dealing with. If there is an unknown action, then it should return the state, so that the application doesn't lose its current state.
3. What does an action contain?Actions are objects that have a type property and any other data that it needs to describe the action(payload).
4. Why do we need to copy the state in a reducer? to avoid losing existing data

## Document the following Vocabulary Terms

+ immutable state: If an object is immutable, any changes that need to be made to it within a function must be made to a copy of the object.

+ time travel in redux:Time travel is the ability to move back and forth among the previous states of an application and view the results in real time. 

+ Reducer :is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action.

+ action creator: is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store’s dispatch() function.

+ dispatch :is a function of the Redux store. You call store.dispatch to dispatch an action. This is the only way to trigger a state change.

## Preparation Materials

CombineReducers mutates an object whose values are different reducer functions into a single function, which then can be passed to createStore. This combineReducers function calls every child reducer and collects their results into a single state object. This state object “namespaces” the states updated from each reducer with the keys.

[Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

[Redux Docs: Using Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)

[Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

[Github view](https://github.com/sbkhaloof/growthmindsit)