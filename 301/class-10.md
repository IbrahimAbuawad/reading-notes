# THE CALL STACK


### The Call Stack defined on MDN

*Call Stack* 
> A mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc. - MDN

* When script finds an invoke statement the interpreter adds it to the 'stack' and starts to carry out the function
* Functions called within that currently invoked function are added to the stack and run when their calls are reached
* When the current function finishes it's removed from the stack
* Stack overflows occur when the stack takes up more space than it had assigned to it. 

This is a great visual for how javascript handles order of operations for functions! 

### Understanding the JavaScript Call Stack

>“function hierarchy and execution order”

*LIFO - Last in, First out:*
>When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

Picture this like a literal stacking of items on top of each other. Like a queue in a grocery store, stacks are synchronous. 

As functions are invoked they are 'popped off' the stack. 

Stack overflows occur when there is a function that calls itself without an exit point. 

### JavaScript error messages

Common Types of Errors:
* Reference errors
* Syntax errors
* Range errors
* Type errors (one of the most frequent)

Debugging: 
* use console.log()
* debugger statement in your code

Call stack: Add names to your functions whenever possible. This will make it much easier to read your stack. You can also try console.trace()

Handling errors: 
* try {} catch {} : use these when your checks are becoming longer than your function logic. 

Tools to avoid runtime errors: 
AKA you can only see what's wrong with your code after you run it. 
* quokka
* eslint
* TypeScript

Being able to read error messages will make you a strong developer! And remember to clean up your debugging stuff before you ACP your code to github. 

