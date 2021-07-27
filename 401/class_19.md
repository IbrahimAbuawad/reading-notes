

## What is the difference between a FIFO and standard queue
* A FIFO queues have similar features to standard queues but also are able to perform exactly-once proccessing or in other words making sure they read/write only one exact time. FIFO queues help to stop unintentional duplicates.
## How can a server be assured a message was properly received?
* A server can expect a response from a client to prove as a confirmation that a message was properly received, as a fail safe it can keep it in a queue until the confirmation is received.

## Define the following terms
* Serverless API
  * A serverless API is based on a cloud service that allows for the creation of API endpoints with specific http request methods such as POST and GET. This allows a coder to create a website without needing a server to host their code.
* Triggers
  * Triggers are a way of setting up functions to activate based on certain events. When an event occurrs, a trigger initiates a specific function as a result.
* Dynamo vs. Mongo
  * Dynamo and Mongo are both NoSQL databases, Mongo is independent while Dynamo is an AWS service.
* Dynamoose vs. Mongoose
  * Dynamoose and Mongoose are npm packages that allow for node.js interface with DynamoDB and MongoDB respectively


## SQS and SNS 

#### SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.

#### SQS is distributed queuing system. Messages are not pushed to receivers.
#### Receivers have to poll or pull messages from SQS. Messages can't be received by multiple receivers at the same time. 
####  You can have SNS send messages to email, SMS or HTTP end point apart from SQS.
#### SQS is mainly used to decouple applications or integrate applications
#### You could use SNS and send this data to multiple subscribers, each replicating the messages it receives to different storage systems


