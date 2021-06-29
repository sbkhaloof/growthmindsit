# React and Forms
## HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.
## in react in most cases, it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form. The standard way to achieve this is with a technique called “controlled components”.
## controlled components ; n HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState(). We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.
### The textarea Tag :
#### In HTML, a <textarea> element defines its text by its children but In React, a <textarea> uses a value attribute instead. 
### The select Tag :
#### In HTML, <select> creates a drop-down list . 
##### Note that the Coconut option is initially selected, because of the selected attribute. React, instead of using this selected attribute, uses a value attribute on the root select tag. This is more convenient in a controlled component because you only need to update it in one place.
#### Overall, this makes it so that <input type="text">, <textarea>, and <select> all work very similarly - they all accept a value attribute that you can use to implement a controlled component.
### The file input Tag :
#### in HTML ets the user choose one or more files from their device storage to be uploaded to a server or manipulated by JavaScript via the File API 
#### Handling Multiple Inputs :When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.
#### Controlled Input Null Value .
1-  What is a ‘Controlled Component’?A controlled component is a component element whose value is controlled by React using state, so with a controlled component, the element value is always driven by the React state.
2-  Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.no ,update value using set.State by users response as soon as enter them.to be dynamic as html.
3-  How do we target what the user is entering if we have an event handler on an input field?The event handler exists on each input field using onChange attribute where the handler itself is using event to target the crossponding input.


## The Conditional (Ternary) Operator 
1- Why would we use a ternary operator? we need it if we want to rewite if condition statment in only one line 
2- Rewrite the following statement using a ternary statement:
### x===y ? console.log(true):console .log(false)