# Component Lifecycle / useEffect()

![](https://1.bp.blogspot.com/-eL2sbdeL9Qc/XdPR4RscrjI/AAAAAAAAVfc/zVXHv6vrPsswu5sZhGCYeOUAEZVGapSxgCLcBGAsYHQ/s1600/React-Components-Lifecycle.png)

## Review, Research, and Discussion

+ Why do we not need more .html pages in a multi-page React app? In Multi-page apps, we get back multiple HTML pages, where each page has content for given Router.
+ If we wanted a component to show up on every page, where would we put it and why? Inside the BrowserRouter />, outside a Route />
+ What does routing do with the components that were rendered when a new route is requested? it goes to the new componetnt and remove the old one
+ What does props.children contain?it is used to display whatever you include between the opening and closing tags when invoking a component.
+ How do useState() and this.setState() differ?setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won’t touch the rest. The useState’s updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

## Document the following Vocabulary Terms

+ State Hook :Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.
+ Mounting and Un-Mounting:Mounting a file system attaches that file system to a directory (mount point) and makes it available to the system. The root / file system is always mounted. Any other file system can be connected or disconnected from the root / file system. These files are not permanently affected by the mounting process, and they become available again when the file system is Un-Mounting.

## Preparation Materials

## Using the Effect Hook

### 🙄 What does useEffect do? By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API

### Why is useEffect called inside a component? Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution

### Does useEffect run after every render? Yes! By default, it runs both after the first render and after every update. (We will later talk about how to customize this.) Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects

[Github view](https://github.com/sbkhaloof/growthmindsit)
