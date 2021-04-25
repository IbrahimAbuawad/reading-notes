## State and lifecycle
#### In Rendering Elements, we have only learned one way to update the UI.

#### You can convert a function component like Clock to a class in five steps:
1. Create an ES6 class, with the same name, that extends React.Component.
2. Add a single empty method to it called render().
3. Move the body of the function into the render() method.
4. Replace props with this.props in the render() body.
5. Delete the remaining empty function declaration.

#### Adding Local State to a Class :
##### Example :
```
class Clock extends React.Component {
  constructor(props) {
    super(props);
    this.state = {date: new Date()};
  }

  render() {
    return (
      <div>
        <h1>Hello, world!</h1>
        <h2>It is {this.state.date.toLocaleTimeString()}.</h2>
      </div>
    );
  }
}

ReactDOM.render(
  <Clock />,
  document.getElementById('root')
);
```
#### While this.props is set up by React itself and this.

#### Do Not Modify State Directly
##### For example, this will not re-render a component:
`this.setState({comment: 'Hello'});`

#### A component may choose to pass its state down as props to its child components:

`<FormattedDate date={this.state.date} />`

## Handling Events

#### React events are named using camelCase, rather than lowercase.

#### With JSX you pass a function as the event handler, rather than a string.

###### When using React, you generally don’t need to call addEventListener to add listeners to a DOM element after it is created. 

```
class Toggle extends React.Component {
  constructor(props) {
    super(props);
    this.state = {isToggleOn: true};
```

#### Inside a loop, it is common to want to pass an extra parameter to an event handler. For example:

```
<button onClick={(e) => this.deleteRow(id, e)}>Delete Row</button>
<button onClick={this.deleteRow.bind(this, id)}>Delete Row</button>
```

## Conditional Rendering

#### Conditional rendering in React works the same way conditions work in JavaScript. 

##### In the example below, we will create a stateful component called LoginControl.

```
class LoginControl extends React.Component {
  constructor(props) {
    super(props);
    this.handleLoginClick = this.handleLoginClick.bind(this);
    this.handleLogoutClick = this.handleLogoutClick.bind(this);
    this.state = {isLoggedIn: false};
  }

  handleLoginClick() {
    this.setState({isLoggedIn: true});
  }

  handleLogoutClick() {
    this.setState({isLoggedIn: false});
  }

  render() {
    const isLoggedIn = this.state.isLoggedIn;
    let button;
    if (isLoggedIn) {
      button = <LogoutButton onClick={this.handleLogoutClick} />;
    } else {
      button = <LoginButton onClick={this.handleLoginClick} />;
    }

    return (
      <div>
        <Greeting isLoggedIn={isLoggedIn} />
        {button}
      </div>
    );
  }
}

ReactDOM.render(
  <LoginControl />,
  document.getElementById('root')
);

```

### Inline If-Else with Conditional Operator

#### he <WarningBanner /> is rendered depending on the value of the prop called warn.

#### Returning null from a component’s render method does not affect the firing of the component’s lifecycle methods. For instance componentDidUpdate will still be called.

