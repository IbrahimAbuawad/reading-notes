# React
### What Is React?
#### React is a declarative, efficient, and flexible JavaScript library for building user interfaces. 

#### It lets you compose complex UIs from small and isolated pieces of code called “components”.

## JSX

#### It is called JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like.

#### React embraces the fact that rendering logic is inherently coupled with other UI logic:
1. how events are handled.
2. how the state changes over time.
3. how the data is prepared for display.

![JXS](https://miro.medium.com/max/3440/1*Rvs7u_g6dnDTRF-FMY4vsA.png)

#### React separates concerns with loosely coupled units called “components”

#### React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code.

#### In the example below, we declare a variable called name and then use it inside JSX by wrapping it in curly braces:

```
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;

ReactDOM.render(
  element,
  document.getElementById('root')
);
```
##### After compilation, JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.

#### ou may use quotes to specify string literals as attributes:
`const element = <div tabIndex="0"></div>;`

#### If a tag is empty, you may close it immediately with />, like XML:

`const element = <img src={user.avatarUrl} />;`

#### By default, React DOM escapes any values embedded in JSX before rendering them. 

```
const title = response.potentiallyMaliciousInput;
// This is safe:
const element = <h1>{title}</h1>;
```

#### Babel compiles JSX down to React.createElement() calls.

##### These two examples are identical:

```
const element = (
  <h1 className="greeting">
    Hello, world!
  </h1>
);
```

```
const element = React.createElement(
  'h1',
  {className: 'greeting'},
  'Hello, world!'
);

```



`const element = <h1>Hello, world!</h1>;`

### Rendering Elements
#### An element describes what you want to see on the screen:
##### Example : 
`const element = <h1>Hello, world</h1>;`

#### Unlike browser DOM elements, React elements are plain objects, and are cheap to create.

#### We call a “root” DOM node because everything inside it will be managed by React DOM.

#### To render a React element into a root DOM node, pass both to :
`ReactDOM.render():`
```
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));

```

#### React elements are immutable. Once you create an element, you can’t change its children or attributes.

```
function tick() {
  const element = (
    <div>
      <h1>Hello, world!</h1>
      <h2>It is {new Date().toLocaleTimeString()}.</h2>
    </div>
  );
  ReactDOM.render(element, document.getElementById('root'));
}

setInterval(tick, 1000);
```
![React](https://miro.medium.com/max/2484/1*CeuWv9fCjD1uTiTuKytnBQ.png)
### React Only Updates What’s Necessary
#### Even though we create an element describing the whole UI tree on every tick, only the text node whose contents have changed gets updated by React DOM.

## Components and Props

#### The simplest way to define a component is to write a JavaScript function:
```
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```
#### This function is a valid React component because it accepts a single “props”

#### ES6 class to define a component:
```
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

![Func VS Class](https://image.slidesharecdn.com/svn1aqx5rombdmxcxvox-signature-3c2725b6926a6a70a7c24118f64b2cb1760fb9359bc9b181dea3c7789a170437-poli-180714120536/95/react-redux-js-75-638.jpg?cb=1531570280)

#### When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object.

#### Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. 

###### new React apps have a single App component at the very top.

###### We recommend naming props from the component’s own point of view rather than the context in which it is being used.

### Props are Read-Only Like :
```
function sum(a, b) {
  return a + b;
}
```