# Readings: Redux - Combined Reducers

## Review, Research, and Discussion
### Why choose Redux instead of the Context API for global state?
#### Context API is easy to is use as it has a short learning curve. It requires less code, and because there's no need of extra libraries, bundle sizes are reduced
### What is the purpose of a reducer?
#### In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state.
### What does an action contain?
#### An action is an object that contains two keys and their values. The state update that happens in the reducer is always dependent on the value of action
### Why do we need to copy the state in a reducer?
#### the reducer must create new object, and making a copy is a way to describe the unchanged part.

## TERMS
#### immutable state: is an object whose state cannot be modified after it is created. This is in contrast to a mutable object (changeable object), which can be modified after it is created.
#### time travel in redux: Time travel is the ability to move back and forth among the previous states of an application and view the results in real time.
#### action creator: An action creator is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more actions
#### reducer: a reducer is a pure function that takes an action and the previous state of the application and returns the new state.
#### dispatch: dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change

## Preperation material
### combineReducers
#### helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . 
#### The resulting reducer calls every child reducer, and gathers their results into a single state object
#### The initial shape and contents of your store's state may be defined in two ways. First, preloadedState can be sent as the second parameter to the createStore method.

#### There are several important ideas to be aware of when using combineReducers :
1. One frequently asked question is whether Redux “calls all reducers” when dispatching an action. Since there really is only one root reducer function, the default answer is “no, it does not”
2. you can use it at all levels of your reducer structure, not just to create the root reducer.
