# Event Driven Application

## Review, Research, and Discussion

1. Why is access control important?

- implements a layer of security for confidential information

2. Describe an application that would need access control.modules, specifically with classes

- any app that has signup/signin capabilities
- shopping websites
- blogs

3. What is a role used for?

- dictates what users capabilities are

4. Why is role based access control more scalable than discretionary or mandatory access control?

- it is more scalable by allowing users access to confidential information, all you have to do is change their role. Other methods to perform the same action can become overly complicated

## Terminology

- Authorization:
  - allows users permissions to access to content

- Role Based Access Control:
  - method of restricting network and private information based on roles of individual users

- Capabilities:
  - a given action to users that allows individual users to perform certain tasks or access otherwise private information

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?

- Roles, Auth, and Capabilities

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Username Passwords and authentication, how user specific data is retrieved and rendered, creating a CRUD app utilizing username and password.
- I want to learn more about Events and how things change real time on other computers
- working with multiple servers on a single app

3. What are you most excited about trying to implement or see how it works?

- Real time events!

## Preparation Materials

### Event-Driven Programming
#### Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision

#### Every time you interact with a webpage through it’s user interface, an event is happening

#### use of the following concepts :
1. An Event Handler is a callback function
2. A Main Loop listens for event triggers

### Node.js v16.4.2 documentation

#### example of Asynchronous vs. synchronous

```
const myEmitter = new MyEmitter();
myEmitter.on('event', (a, b) => {
  setImmediate(() => {
    console.log('this happens asynchronously');
  });
});
myEmitter.emit('event', 'a', 'b');
```
#### example of Handling events only once :

```
const myEmitter = new MyEmitter();
let m = 0;
myEmitter.on('event', () => {
  console.log(++m);
});
myEmitter.emit('event');
// Prints: 1
myEmitter.emit('event');
// Prints: 2
```

## References

- https://www.citrix.com/solutions/secure-access/what-is-access-control.html
