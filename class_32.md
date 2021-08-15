## Review, Research, and Discussion
### When you have multiple contexts, what component type should you use (class/function) and why?
#### The difference is pretty obvious. Class components are ES6 classes and Functional Components are functions. The only constraint for a functional component is to accept props as an argument and return valid JSX.


### (Links to an external site.)How can you best test context?
#### The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).

## Context api
#### Context provides a way to pass data through the component tree without having to pass props down manually at every level and In a typical React application, 
#### The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This default value can be helpful for testing components in isolation without wrapping them

#### We want to test our components in the same way that developers do (behavioral testing) and in the same way that they would operate in our environment.

#### All consumers that are descendants of a Provider will re-render whenever the Provider’s value prop changes. 
