# Readings: Redux - Asynchronous Actions
## Review, Research, and Discussion
#### How granular should your reducers be?
##### I think the advantage of granular actions would be the events more accurately reflect what the user did
#### Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
##### Con as it gets messy and actions need to get filtered through.
#### Name a strategy for preventing the above
##### Make a reducer for each component that will be affected by the dispatcher, only effecting a specific amount of the state it self.

### Term
#### store: A store is an immutable object tree in Redux. A store is a state container which holds the application's state.
#### combined reducers: The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore 

## Preperation material

### Redux Thunk
#### is a middleware that lets you call action creators that return a function instead of an action object. 
#### a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. 
```
import { client } from '../api/client'

const delayedActionMiddleware = storeAPI => next => action => {
  if (action.type === 'todos/todoAdded') {
    setTimeout(() => {
      // Delay this action by one second
      next(action)
    }, 1000)
    return
  }

  return next(action)
}

const fetchTodosMiddleware = storeAPI => next => action => {
  if (action.type === 'todos/fetchTodos') {
    // Make an API call to fetch todos from the server
    client.get('todos').then(todos => {
      // Dispatch an action with the todos we received
      storeAPI.dispatch({ type: 'todos/todosLoaded', payload: todos })
    })
  }

  return next(action)
}
```

### Redux Middleware and Side Effects
#### A “side effect” is any change to state or behavior that can be seen outside of returning a value from a function. Some common kinds of side effects are things like: 
1. Logging a value to the console
2. Saving a file
3. Setting an async timer
