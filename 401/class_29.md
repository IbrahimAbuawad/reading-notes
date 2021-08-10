# Advanced State with Reducers
## Review, Research, and Discussion

### How can we ensure that an effect hook runs only once?
#### If we pass an empty array [] , it just renders the component only once like componentDidMount .

### Is useState() synchronous? 
#### useState and setState both are asynchronous.Even though they are asynchronous, the useState and setState functions do not return promises

### Can useState() update more than one state variable at the same time? 
#### No

## Terms 

### State Hook :  Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class

### Component Lifecycle : Components are created (mounted on the DOM), grow by updating, and then die (unmount on DOM). This is referred to as a component lifecycle.


## preperation material :

### useReducer is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook:

1. it helps you manage complex state logic in React applications.
2. useReducer can be a good alternative to Redux or MobX — indeed

#### useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.
#### useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

#### Example : 
```
const [state, dispatch] = useReducer(reducer, initialArg, init);
```
##### it accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method.
