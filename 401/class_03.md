# Express REST API

## Terms

- Middleware: 
  - function (typically a module_ hat executes during the lifecycle of a request to a route.
  - middlewares have access to the request and response object for each route they are attached to
  - can terminate an HTTP request, or pass the request by using next()
  - has the ability to modify an HTTP request before the server receives the data
- Request Object: 
  - parameter of a callback function / route handler
  - object that contains information passed from a client/front end
- Response Object: 
  - also a parameter of a callback function / route handler
  - sends a response to the client, answering to a request
- Application Middleware: middleware on a global level. this middleware executes on all route route calls
- Routing Middleware: middleware that is used in a route that is able to modify request/response objects
- Test Driven Development: software development approach where tests are created to ensure functional code / software
  - tests before typing any code
  - red, green, refactor
- Behavioral Testing Development: a team escentric workflow that accomodates specifically on whys/ features wanted in a program/software

## Review, Research, and Discussion
1. Name 3 real world use cases where you’d want to change the request with custom middleware
  - send an error when user sends invalid information
  - if the request object does not provide the information you want to return to the client
  - authentication purposes 
2. True or false: The route handler is middleware?
  - yes, it can be
3. In what ways can a middleware function end the process and send data to the browser?
  - throwing an error `throw new Error('enter error message here')
  - `next('enter error message here')`
4. At what point in the request lifecycle can you “inject” middleware?
  - you can inject middleware between the endpoint and handler within a code block
5. What can cause express to error with “Request headers sent twice, cannot start a second response”
  - my guess is if two routes are called at the same time providing 2 responses or in any case where something would trigger to send 2 responses

## Preview
1. Which 3 things had you heard about previously and now have better clarity on?
- Databases. Its interesting digging deeper on the fundamentals and seeing how everything is functioning.
- REST and CRUD.
- Request and Response Objects
- Classes

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- MongoDB
- REST and CRUD terminology
- Classes

3. What are you most excited about trying to implement or see how it works?
- MONGO DB! Seems way more pratical than SQL.

### References:
- https://developer.okta.com/blog/2018/09/13/build-and-understand-express-middleware-through-examples#:~:text=Middleware%20literally%20means%20anything%20you,or%20path)%20it's%20attached%20to.

- https://expressjs.com/en/guide/using-middleware.html

- https://www.javatpoint.com/expressjs-request

- https://www.javatpoint.com/expressjs-response

- https://www.guru99.com/test-driven-development.html

