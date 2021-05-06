# Class 13 Notes: MESSAGE Queues:

## Q And A:

1. What does it mean that web sockets are bidirectional? Why is this useful?

- this means that web sockets can both reieve and and send data across a server. this is useful in and of itself.

2. Does socket.io use HTTP? Why?

- Yes. A client can fall back on an HTTP call if it cannot establish aconnection with a web socket.

3. What happens when a client emits an event.

- it is sending information out to the server. which should be listening with on the other side.

4. What happens when the server emits and event?

- when a server emits an event, it can emit to all clients associated with its namespace.

5. What happens if a client “misses” an event?

-

6. How can we mitigate this

- we can fall back on a http call.

## Vocab:

- `Socket:` an object that allwos for two-way communication between two entities.
- `Web Socket:` a socket that allows communication between a browser and its host server
- `Socket.io:` a library for enabling web sockets. [LEARN MORE](https://socket.io/docs/v4/index.html)
- `Client:` a platform - can be either hareware or software that access services and information via connection to a server
- `Server:` a device that provides provides a service or functionality to a client
- `OSI Model:` Open Systems Interconnection Model [Wiki](https://en.wikipedia.org/wiki/OSI_model)
- `TCP:` Transmission Control Protocol. Takes messages from an application/server and divides them into packets. [wiki](https://en.wikipedia.org/wiki/Transmission_Control_Protocol)
  - Protocol: a set of rules that dictate how information should be transferred and handled by entities communicating with one another [Source](https://www.sdxcentral.com/resources/glossary/protocol/)
- `TCP Model:`
- `UDP:` User Datagram Protocol
- `Packets:` units of data that is usually trafficed across a network between clients and servers.
