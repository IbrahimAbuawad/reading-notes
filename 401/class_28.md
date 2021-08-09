# useState() Hook

## Review, Research, and Discussion
### Why do we not need more .html pages in a multi-page React app?
####  because some of react apps need static html page and render it once and some not

### If we wanted a component to show up on every page, where would we put it and why?
#### Inside the <BrowserRouter />, outside a <Route /> .. cuz if we put it inside the route it will be render it in this specific route

### What does routing do with the components that were rendered when a new route is requested ?
#### go throw the code again inside the routing and search for the new routing requesting if it exist it will rendered and if it is not will show 404 not found

### What does props.children contain?
#### it is used to display whatever you include between the opening and closing tags when invoking a component.

### how do useState() and this.setState() differ?
#### useState its a hooks use inside a funtion , this.setState its used inside a class to use and change states

### TERMS
#### State Hook : Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class
#### Mounting and Un-Mounting : mounting is when the component rendered and unmount when the component not showing

## Preparation Materials

### Hooks
#### A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.
#### Hooks apply the React philosophy (explicit data flow and composition) inside a component, rather than just between the components

##### Example :
![](https://miro.medium.com/max/700/1*9QhpwSGTKM-c8sc4UNcxqA.png)

### useEffect
#### The Effect Hook, useEffect, adds the ability to perform side effects from a function component.
#### It serves the same purpose as componentDidMount, componentDidUpdate, and componentWillUnmount in React classes

#### Example : 

```
import React, { useState, useEffect } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  // Similar to componentDidMount and componentDidUpdate:
  useEffect(() => {
    // Update the document title using the browser API
    document.title = `You clicked ${count} times`;
  });
```
