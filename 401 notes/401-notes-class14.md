# Class 14: Event Driven Architecture:

## Q and A

1. What’s the difference between a FIFO and a standard queue?
   - to clarify, we can use queues to deliver messages between clients and servers.
   - `standard queue` tries to preserve the order of those messages, and guarentees at-least-once delivery of those messages. the message could be recieved more than once.
   - `FIFO queue` ensures that order is maintained, and messages are sent only once. there are no duplicates. [source](https://www.learnaws.org/2020/12/21/aws-sqs-fifo-deep-dive/#:~:text=A%20standard%20queue%20tries%20to,and%20received%20in%20strict%20order.)
2. How can the server be assured a message was properly received?
   - a callback function can be added to the `send()` or `emit()` method calls. [source](https://www.semicolonworld.com/question/47982/how-to-be-sure-that-message-via-socket-io-has-been-received-to-the-client)
   ```javascript
   socket.send("hi", function () {
     // if the message is recieved, than whatever is in here will trigger.
   });
   ```
3. What classic design pattern is best represented by event driven programming?

   - The Observer Pattern: in which an object maintains a list of dependents, called observers, and notifies them of any state changes. [source](https://en.wikipedia.org/wiki/Observer_pattern)

4. How do you test an event driven system?
   - an asynchronous method is demonstrated in this aritce. [source](https://blog.gurock.com/event-driven-application-architectures/)

## Vocab:

- `FIFO Queue`: as stated before, designed to enhance messaging between applications when the order of operations and events is critical, or where duplicates can't be tolerated. [source](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/FIFO-queues.html) \_
- `Pub/Sub`: publish/subscribe messaging. an asynchronous communication where any item that any message published to an item "or emited to" is recieved by any items that subscribe "or listening with .on" to that item.
