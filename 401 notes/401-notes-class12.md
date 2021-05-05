# NOTES: SocketIO

## Q and A

1. What is the benefit of transforming data into packets?
   - By transforming data into packet on TCP/IP networks, it allows a network to accomodate various andwidths, allows for multiple routes, and retransmits the peices of data which are interrupted or lost.
2. UDP is often refered too as a connetionless protocol. Why?
   - It is called "connectionless" because it allows for communication between networks without needing a prior engagement.
3. Can a socket server application have multiple socket connections.

   - Yes, by listiening to a socket fork.

4. Can a socket connection application be connectied to multiple socket servers?
   - Yes, but it must listen for these servers from a single port.
5. Can an application be both a socket server and a socket connectino?
   - You can run input and output streams of a socket on the same thread and supporting a single connection.

## Vocab:

- `Observer Pattern: `A software design pattern in which an object, called the **subject**, maintains a list of its dependents, called observers, and notifies them of any state changes. it is a one-to-many relationship.
- `Listener: ` an object that waits on to on a event to trigger in a web container. and will let us know once it has
- `Event Handler: `code that will run when an event finally fires.
- `Event Driven Programming: `a programming paradigm in which the flow of a program is deteremnd by events, such as those triggered by user input.
- `Event Loop: `A programming construct that waits and dispatches events and or messages in an application. it is often the central control flow of an app.
- `Event Queue: `The idea of delaying the sending of events to a point in the execution flow where it is okay to publish them. literally putting events into a **queue**
- `Call Stack: `A data structure that stores information about the active subroutines of a program.
- `Emit/Raise/Trigger: `
- `Subscribe: `
- `database: `
