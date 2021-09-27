# Login  and Auth 

## Review, Research, and Discussion

1. Why is the Context API useful? it help us to share the data between the components at different level without using props
2. Can a component outside of a provider get its context? no 
3. What are some common use cases for using the Context API? as them and authintication
4. Describe “Context Hell” ? is the nasty code you get taking advantage of the React Context API.

## Document the following Vocabulary Terms

+ global state : state when is the data that is shared between all the components within a React application. When the state is changed, or let’s say a filter is added, the components re-render accordingly.
+ global context : t’s designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.
+ provider : React component that allows consuming components to subscribe to context changes.
+ consumer :hat subscribes to context changes. Using this component lets you subscribe to a context within a function component. Requires a function as a child. The function receives the current context value and returns a React node.

## Preparation Materials

``Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.
``

### BENEFITS OF RBAC

Managing and auditing network access is essential to information security. Access can and should be granted on a need-to-know basis. With hundreds or thousands of employees, security is more easily maintained by limiting unnecessary access to sensitive information based on each user’s established role within the organization.

### react-cookies component

"Persisting Data Using Cookies in React Apps" When trying to persist data in React apps, there are generally two ways to go: localStorage or cookies. You will find a lot of information and debate about localStorage vs cookies. 

### Why Cookies
```I could persist even with browser refreshes and across sessions. I could also give the cookie an expiration date.```

Cookies are mainly used for three purposes:

Session management :

1. Logins
2. shopping carts
3. game scores, or anything else the server should remember

[what is role based access control](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

[react-cookies component](https://www.npmjs.com/package/react-cookies)

[react-cookie library](https://www.npmjs.com/package/react-cookie)

[Github view](https://github.com/sbkhaloof/growthmindsit)