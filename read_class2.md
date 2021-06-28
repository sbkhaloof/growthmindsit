# State and Props
## What are component lifecycle events?
### there are three phases of the component lifecycle.
+ Mounting ,  Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting .
+ Updating , static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps.
+  Unmounting
![](https://miro.medium.com/max/1718/1*u8hTumGAPQMYZIvfgQMfPA.jpeg)
### The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance.
### static getDerivedStateFromProps() :This method exists for rare cases where the state relies on changes in props over time.
### render() :Render is the only required method in a class component. It will examine this.props and this.state when called. 
### componentDidMount() :This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().
### shouldComponentUpdate() :The default behavior in react is to rerender after every state change. Setting shouldComponentUpdate() to false allows you to prevent this from happening. This is in order to optimize performance.
### getSnapshotBeforeUpdate() :This is another rarely used method that allows you to capture a picture of the DOM to check it before actually changing anything on the DOM.
### componentDidUpdate() :This method is useful for performing network requests after a change has occurred.
### componentWillUnmount() :This method allows you to clean up the DOM and netwrok requests/ subscriptions.

