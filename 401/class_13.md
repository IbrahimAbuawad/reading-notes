# Message Queues

## Review, Research, and Discussion

1. What does it mean that web sockets are bidirectional? Why is this useful?

- yes. being bidirectional is a communication protocal that is able to send data from client to server or from server to client reusing the established connection

2. Does socket.io use HTTP? Why?

- Yes, the initial connection setup is done over HTTP.
- sockets are made within this connection

3. What happens when a client emits an event?

- Event is thrown into an event pool and is triggered by any client/event that is listening for the event
- listeners typically have a callback function which runs a codeblock when the event is triggered

4. What happens when a server emits an event?

- event is sent to specific subs, all clients, or both.
- triggers a callback that is assigned to the listener and runs the code

5. What happens if a client “misses” an event?

- missed events are ignored which prevents the rest of a chain of code to run (which is bad)

6. How can we mitigate this?

- unheard events should be stored in a queue system on the server that is resumed as a client connects

## Terminology

- Socket.io:
  - library that enables real-time, bidirectional and event-based communication between the browser and the servers

- Socket:
  - one endpoint of a two-way communication line between the programs on a network
  - a socket is bound to a PORT# so that the TCP layer can identify the application that data is destined to be sent to

- Web Socket:
  - primary interface for connecting to a websocket server and sending and receiving data on the connection

- Client:
  - a client is a computer or program
  - relies on sending requests to another program (server/backend) or hardware that accesses a service made available by the server

  - examples
    - web browsers are cleintes connected to web services that retrieves web pages
    - email client to retrieve email from mail servers
    - client and servers connect via interprocesses communication techniques

- Server:
  - a piece of computer hardware/software that provides functionality for other programs or devices called 'clients'
  - architecture: client-server model
    - requests-response model

- OSI Model:
  - open systems interconnection model
  - consists of 7 layers: physical, data link, network, transport, session, presentation, application
  - logical and conceptual model that defines network communications used by systems that are open to interconnection and communication with other systems

- TCP Model:
  - transmitter control protocol
  - consits of 4 layers: process/application layer, host-to-host/ transparent layer, internet layer, network access/link layer
  - more reliable network than OSI
  - helps determine how a specific computer should be connected to the internet and transfer data between them

- TCP:
  - Transmission Control Protocol
  - communication between two computers needs to be 'good' and reliable to guarantee that the data is received correctly
  - ensures full transfer of data before rendering/uploading
  - connection oriented protocol
  - GUARENTEES DELIEVERY OF DATA

- UDP:
  - User Datagram Protocol
  - connectionless
  - does not establish session
  - doesnt guarentee delievery of data
  - faster than TCP

- Packets:
  - packets are intended to transfer data reliably instead of transferring a large block of data
  - sending smaller packets help ensure each section is transmitted successfully
  - dropped packets are easily fixed by resending the packet that was dropped.

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?

- Clients, Servers, and Socket.io

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- I read about OSI and TCP but I want to see an example to help me understand further, What is OSI used for and some examples, what is TCP used for and some examples

3. What are you most excited about trying to implement or see how it works?

- Working with creating servers and clients and making them optimal!


## socket example

```
 form.addEventListener('submit', function(e) {
    e.preventDefault();
    if (input.value) {
      socket.emit('chat message', input.value);
      input.value = '';
    }
  });
```

## Rooms

#### A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients:

![socket room](https://socket.io/images/rooms.png)


## References

- https://www.forcepoint.com/cyber-edu/osi-model#:~:text=The%20OSI%20Model%20(Open%20Systems,between%20different%20products%20and%20software.
