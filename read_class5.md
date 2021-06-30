# Putting it all together
## Thinking in React
#### One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React.

### Start With A Mock
##### How would you break a mock into a component heirarchy?
###### first thing you should draw a boxes around the components in a mock and use  single responsibility principle . Since you’re often displaying a JSON data model to a user, you’ll find that if your model was built correctly,Separate your UI into components, where each component matches one piece of your data model.finnaly that we’ve identified the components in our mock, let’s arrange them into a hierarchy. Components that appear within another component in the mock should appear as a child in the hierarchy.
##### What is the single responsibility principle and how does it apply to components?
###### is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part. All of that module, class or function's services should be narrowly aligned with that responsibility.
##### What does it mean to build a ‘static’ version of your application?
###### that takes your data model and renders the UI but has no interactivity.
##### Once you have a static application, what do you need to add?
###### Identify The Minimal (but complete) Representation Of UI State.
##### What are the three questions you can ask to determine if something is state?
1- Is it passed in from a parent via props? If so, it probably isn’t state.
2- Does it remain unchanged over time? If so, it probably isn’t state.
3- Can you compute it based on any other state or props in your component? If so, it isn’t state.
##### How can you identify where state needs to live?
###### For each piece of state in your application:Identify every component that renders something based on that state.after that Find a common owner component (a single component above all the components that need the state in the hierarchy).Either the common owner or another component higher up in the hierarchy should own the state.If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
