# Data Modeling

## Terms
- functional programming:
  - programming paradigm for developing software using functions
  - relies on expressions on devlarations rather than statements
  - outputs only depend on arguments that are passed in
  - easier to test
- Object Oriented Programming(OOP):
  - programming paradigm based on concept of objects which contain data and code
- class:
  - data format and available procedures for a given type of class of object
- super:
  - used in extension of classes, super is a keyword that refers to the parent of its containing class.
  - it is used to call the constructor of the parent class which grants access to the parents properties and methods
- this:
  - outer most object
  - terminal -> global
  - broswer -> window
  - class context: refers to the variable name of the instantiated object
- Test Driven Development(TDD):
  - software development approach in which test cases are developed to specify and validate what code will do
  - focus on developing and running automated tests before actual development application
- Jest:
  - javascript framework designed to ensure correstness of any JavaScript Codebase
- Continuous Integration(CI):
  - a pratice of automating intergration of code changes from multiple contributions into a single project
  - allows software developer tasks to be completed independently and parallel amongst other tasks
- representational state transfer(REST):
  - architectural style for application program interface (API) uses HTTP requests tp access and use data
  - these actions are mapped to a CRUD action which ultimately modfies data
  - uses less bandwith
- Data Model:
  - data structure that displays the storage, model, and functionality of data

## Review, Research, and Discussion
1. Name 3 advantages to Test Driven Development
  - reduced software failure with minimal use of resource/time
  - built around the answer/solution
  - lead to improved design qualities and overall internal/technical qualities

2. In what case would you need to use beforeEach() or afterEach() in a test suite?
  - in an instance where tests should be explicit
  - when tests should never share the same state between tests

3. What is one downside of Test Driven Development?
  - too many tests/uncesessary testing

4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
  - prototype classes do not have subclasses and are unable to pass properties and methods to other subclasses

5. Why REST?
  - speed, popularity, flexibility on response formats: JSON, XML, HTML, EJS, plain text. etc

## Preview
- Which 3 things had you heard about previously and now have better clarity on?
  - beforeEach() and afterEach()
  - REST
  - Object Oriented Programming

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - beforeEach() and afterEach(), specificially how to implement them
  - More about classes!
  - Continuous Intergration in action with a development team
    - we have been working on group projects where we have to meet up and have 'merge parties'. Curious to know how CI changes the process

- What are you most excited about trying to implement or see how it works?
  - CI!

### References:
- https://www.keycdn.com/blog/functional-programming
- https://en.wikipedia.org/wiki/Object-oriented_programming
- https://en.wikipedia.org/wiki/Class_(computer_programming)
