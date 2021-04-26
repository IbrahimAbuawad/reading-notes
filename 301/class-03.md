## Lifting State Up
#### We will start with a component called BoilingVerdict.
#### It accepts the celsius temperature as a prop

##### two functions to convert from Celsius to Fahrenheit and back :
```
function toCelsius(fahrenheit) {
  return (fahrenheit - 32) * 5 / 9;
}

function toFahrenheit(celsius) {
  return (celsius * 9 / 5) + 32;
}
function toCelsius(fahrenheit) {
  return (fahrenheit - 32) * 5 / 9;
}

function toFahrenheit(celsius) {
  return (celsius * 9 / 5) + 32;
}
```
![Lifting state](https://miro.medium.com/max/2904/1*3DpOVY9vZpw2Ll4nWBFu9w.png)

#### In React, sharing state is accomplished by moving it up to the closest common ancestor of the components that need it
###### props are read-only

#### React calls the function specified as onChange on the DOM <input>. In our case, this is the handleChange method in the TemperatureInput component.

#### There should be a single “source of truth” for any data that changes in a React application

#### Lifting state involves writing more “boilerplate” code than two-way binding approaches

######  you can implement any custom logic to reject or transform user input.

## Lists and Keys

#### we use the map() function to take an array of numbers and double their values. 
##### Example :

```
const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);
```

#### You can build collections of elements and include them in JSX using curly braces {}.

### Keys help React identify which items have changed, are added, or are removed. 

```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
);
```

###### We don’t recommend using indexes for keys if the order of items may change.

####  if you extract a ListItem component, you should keep the key on the <ListItem /> elements 

#### Keys Must Only Be Unique Among Siblings

#### JSX allows embedding any expression in curly braces so we could inline the map() result

###### Keep in mind that if the map() body is too nested, it might be a good time to extract a component.

## How to Use the Spread Operator (…) in JavaScript to :

1. Copying an array
2. Concatenating or combining arrays
3. Using Math functions
4. Using an array as arguments
5. Adding an item to a list
6. Adding to state in React
7. Combining objects
8. Converting NodeList to an array

##### Example: 
```
const fruits = ['Apple','Orange','Banana','watermelone','mango']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) ['Apple','Orange','Banana','watermelone','mango']
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍
```

