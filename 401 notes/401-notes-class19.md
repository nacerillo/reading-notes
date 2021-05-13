# Class 19:

## Q and A:

1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

- both allow for the implementation of RESTful API.both allow allow us to communicate with a server, and perform CRUD actions

2. List the AWS Database offerings and talk about the pros and cons of each

-

3. What’s the difference between a FIFO and a standard queue?

- Standard queue is at-least-once queue, and a FIFO Queue is a one-time-only queue

4. How can the server be assured a message was properly received?

- the server can emit a event that sends data back to the user to show that it has been reached.

## Vocab:

- `Serverless API`: more streamlined and be more scalable thanks to cloud computing. a resource that can exist in the cloud instead of on a server.
- `Triggers`: setting a condition or prompt for when a function will run.
- `Dynamo vs Mongo`: [SOURCE](https://www.xplenty.com/blog/dynamodb-vs-mongodb-differences/#:~:text=DynamoDB%20is%20a%20fully%20managed,fully%20managed%20with%20MongoDB%20Atlas.&text=DynamoDB%20uses%20tables%2C%20items%20and,and%20has%20fewer%20size%20restrictions.):

  - MongoDB is vendor agnostic, Open Source, and can be deployed anywhere. DynamoDB is only available on AWS.
  - DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas.
  - DynamoDB as an integrated AWS service makes it easier to develop end to end solutions.
  - DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents.
  - DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions.

- `Dynamoose vs Mongoose`:
