1. What's the difference between `PUT` and `PATCH`?

- The main differnce between PUT and PATCH requests is in the way the server processes the enclosed entity to modify the resource identified by the Request-URI.
- In a `PATCH` request, the enclosed entity contains instructions describing how a resource on the origin server should be modified.
- In a `PUT` request, a modified version of the enclosed entity is on the origin server, and the client is requesting to have the stored version to be replace.

2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server.

3. SOAP vs REST:

- SOAP: Simple Object Access Protocol
- REST: Representational State Transfer.
- Differences: [Source](https://www.guru99.com/comparison-between-web-services.html#:~:text=SOAP%20stands%20for%20Simple%20Object%20Access%20Protocol%20whereas%20REST%20stands,REST%20is%20an%20architectural%20pattern.&text=SOAP%20only%20works%20with%20XML,can%20make%20use%20of%20SOAP.)

  - SOAP stands for Simple Object Access Protocol whereas REST stands for Representational State Transfer.
  - SOAP is a protocol whereas REST is an architectural pattern.
  - SOAP uses service interfaces to expose its functionality to client applications while REST uses Uniform Service locators to access to the components on the hardware device.
  - SOAP needs more bandwidth for its usage whereas REST doesn’t need much bandwidth.
  - SOAP only works with XML formats whereas REST work with plain text, XML, HTML and JSON.
  - SOAP cannot make use of REST whereas REST can make use of SOAP.

- Vocab:
  - Web Server:
  - Express: a web framework written in JS and hosted in the Node.js runtime environment. we use it to make handlers for different http requests, make middleware, etc.
  - Routing
  - WRRC: Web Reqest Response Cycle. how the internet works. a client sends requests - GET, PUT, DELETE, POST - to a server, which in turn response back to the client.
