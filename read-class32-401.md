# Context API - Behaviors

## Review, Research, and Discussion

1. When you have multiple contexts, what component type should you use (class/function) and why? we can use both of them but each one have specific method for class component used with consumer but with functional component using useContext hook .
2. What are some good use cases for using the Context API for global state? thems and authintication 
3. How can you best test context? The best way to test Context is to make our tests unaware of its existence and avoiding mocks


## Document the following Vocabulary 

+ context :provides a way to pass data through the component tree without having to pass props down manually at every level.

+ useContext():  is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level.

+ static context :A static method or, block belongs to the class and these will be loaded into the memory along with the class. You can invoke static methods without creating an object. used with class component when your app has one context


