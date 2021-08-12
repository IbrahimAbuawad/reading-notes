# Reading: Context API
## Review, Research, and Discussion
### Describe use cases useState() vs useReducer()
#### useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.
### Why do custom hooks need the use prefix?
#### that can use hooks inside of it and contain a common stateful logic to be reused in other components.
### What do custom hooks usually do?
#### allow us to have cleaner functional components, remove logic from the UI layer,
### Using any list of custom hooks, research and name one that you think will be useful in your applications
#### useState
### Describe how a hook that fetches API data might work
#### Put the fetchData function above in the useEffect hook and call it, like so: useEffect(() => { const url = "https://api.adviceslip.com/advice";

### Terms
#### reducer : useReducer is a React hook function that accepts a reducer function, and an initial state

## preperation material
#### React.createContext: Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

#### Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes.

```
class MyClass extends React.Component {
  componentDidMount() {
    let value = this.context;
    /* perform a side-effect at mount using the value of MyContext */
  }
  componentDidUpdate() {
    let value = this.context;
    /* ... */
  }
  componentWillUnmount() {
    let value = this.context;
    /* ... */
  }
  render() {
    let value = this.context;
    /* render something based on the value of MyContext */
  }
}
MyClass.contextType = MyContext;

```

### Caveats
#### Because context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders.

### Globally Accessible
#### The state of our snackbars (which ones are visible) can be localized to a single centralized component.

###### All consumers that are descendants of a Provider will re-render whenever the Provider’s value prop changes. The propagation from Provider to its descendant consumers (including .contextType and useContext) is not subject to the shouldComponentUpdate method
