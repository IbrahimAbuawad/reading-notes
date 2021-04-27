## Forms

#### HTML form elements work a little bit differently from other DOM elements in React, because form elements naturally keep some internal state

#### The standard way to achieve this is with a technique called “controlled components”.

#### In React, mutable state is typically kept in the state property of components

#### We can combine the two by making the React state be the “single source of truth”.

#### In HTML, a textarea element defines its text by its children:

```
<textarea>
  Hello there, this is some text in a text area
</textarea>
```

#### In React, a <textarea uses a value attribute instead: 

```
  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          Essay:
          <textarea value={this.state.value} onChange={this.handleChange} />
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
```

#### In HTML, <select creates a drop-down list. For example: 

```
<select>
  <option value="grapefruit">Grapefruit</option>
  <option value="lime">Lime</option>
  <option selected value="coconut">Coconut</option>
  <option value="mango">Mango</option>
</select>
```

 #### React, instead of using this selected attribute, uses a value attribute on the root select tag

 ```
     <select value={this.state.value} onChange={this.handleChange}>
```
###### file it is an uncontrolled component in React.

#### When you need to handle multiple controlled input elements, you can add a name attribute to each elemen

#### Also, since setState() automatically merges a partial state into the current state:

```
var partialState = {};
partialState[name] = value;
this.setState(partialState);
```

###### It can sometimes be tedious to use controlled components, because you need to write an event handler for every way your data can change and pipe all of the input state through a React component