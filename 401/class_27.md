# useState() Hook

## Review, Research, and Discussion
### How does React differ from vanilla JS/HTML/CSS? 
#### Plain JS apps usually start with the initial UI created on the server (as HTML), whereas React apps start with a blank HTML page, and dynamically create the initial state in JavaScript. React requires you to break your UI into components, but plain JS apps can be structured in any way you see fit

### What is the primary difference between a function component and a class component ?
#### A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React.


### TERMS
#### Functional Components : Functional components are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword
#### Children / Child Components :  is a special property of React components which contains any child elements defined within the component

## Preparation Materials

### Hooks
#### A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.
#### Hooks apply the React philosophy (explicit data flow and composition) inside a component, rather than just between the components
#### If the React community embraces the Hooks proposal, it will reduce the number of concepts you need to juggle when writing React applications.
#### adopting Hooks could reduce your bundle size because code using Hooks tends to minify better than equivalent code using classes. 

##### Example :
![](https://miro.medium.com/max/700/1*9QhpwSGTKM-c8sc4UNcxqA.png)

####  What Do Square Brackets Mean?
##### The names on the left aren’t a part of the React API. You can name your own state variables

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
