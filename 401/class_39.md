# Readings: Redux - Additional Topics
## Review, Research, and Discussion

#### What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application? 
#####  to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.

#### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
##### the function that reurns the tunck (function) middleware

### Terms
#### middleware: Redux middleware is a snippet of code that provides a third-party extension point between dispatching an action and the moment it reaches the reducers.
#### thunk: is a Middleware allows you to write action creators that return a function instead of an action. 

## preperation material
### To install Redux ToolKit on the creation of a new App, from terminal:

` npx create-react-app my-app --template redux. `
Or on an existing application:

`npm install @reduxjs/toolkit.`

#### MobX
#### is a simple, scalable and battle tested state management solution. This tutorial will teach you all the important concepts of MobX in ten minutes
#### RTK Query is provided as an optional addon within the @reduxjs/toolkit package. It is purpose-built to solve the use case of data fetching and caching, supplying a compact .

#### Reactions are very similar to derivations. The main difference is these functions don’t produce a value. Instead, they run automatically to perform some task. Usually this is I/O related. 
#### They make sure that the DOM is updated or that network requests are made automatically at the right time.

