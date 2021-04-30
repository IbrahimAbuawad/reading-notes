## What Is Node.js

#### Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.
#### Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

### Node Is Built on Google Chrome’s V8 JavaScript Engine

#### The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers including :

1. Brave
2. Opera
3. Vivaldi

#### the creator of Node (Ryan Dahl) took the V8 engine and enhanced it with various features

#### You can check that Node is installed on your system by opening a terminal and typing

`node -v`   you should see something like `v12.14.1`

### Node.js Has Excellent Support for Modern JavaScript

#### Node has excellent support for ECMAScript 2015 (ES6) and beyond. As you’re only targeting one runtime (a specific version of the V8 engine)
#### The node_modules folder shouldn’t be checked in to version control

#### in node_modules folder the npm has saved lodash and any libraries that lodash depends on. 

![Node](https://i.stack.imgur.com/QRePV.jpg)

### What Is Node.js Used For?

#### ne of the biggest use cases for Node.js — running JavaScript on the server. 

##### Node.js, however, is the first implementation to gain any real traction, and it provides some unique benefits,

##### the server has to wait for the database lookup to complete before it cais n move on to processing the result. If new requests come in while this is happening, the server will spawn new threads to deal with them.

#### Node JS is event-driven, which means that everything that happens in Node is in reaction to an event. 

##### The following image depicts Node’s execution model:
![Node’s execution model](https://uploads.sitepoint.com/wp-content/uploads/2012/10/1516152673node_event_loop.png)



####  “Hello, World!” example HTTP server:

```
const http = require('http');

http.createServer((request, response) => {
  response.writeHead(200);
  response.end('Hello, World!');
}).listen(3000);

console.log('Server running on http://localhost:3000');
```

#### The anonymous function is called with two arguments :

1. request
2. response

##### These contain the request from the user and the response, which we use to send back a 200 HTTP status code, along with our “Hello World!” message.

#### Node is particularly suited to building applications that require some form of real-time interaction or collaboration

###### JSON is probably the most important data exchange format on the Web, and the lingua franca for interacting with object databases (such as MongoDB)

## 6 Reasons for Pair Programming

![Pair](https://martinfowler.com/articles/on-pair-programming/driver_navigator.png)

1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness


## Things I want to know more about

1. Node.js
2. data structures
3. AI


