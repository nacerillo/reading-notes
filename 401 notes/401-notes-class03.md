# Class Notes 03

1. Name 3 real world use cases where you’d want to change the request with custom middleware

- User authentication

2. True or false: The route handler is middleware?
   In what ways can a middleware function end the process and send data to the browser?\

- Technically yes, since they can have middleware functions attached to them. [StackOverflow](https://stackoverflow.com/questions/58925276/what-is-the-difference-between-a-route-handler-and-middleware-function-in-expres#:~:text=They%20are%20not%20middleware%20functions,they%20are%20only%20handler%20functions.)

3. At what point in the request lifecycle can you “inject” middleware?

   - middleware can be injected just as a request is going from the client to the server.

4. ## What can cause express to error with “Request headers sent twice, cannot start a second response”

## Vocabulary Words:

**Middleware** - software that acts as a bridge between an operating system or database and applications, especially on a network. [Oxford](https://languages.oup.com/google-dictionary-en/)
**Request Object** - an object that serves entry point for an application to send an http request to a server
**Response Object** - an object that communicates between the server and client, and returns output from the server
**Application Middleware** - Bind application-level middleware to an instance of the app object by using the `app.use()` and `app.METHOD()` functions, where METHOD is the HTTP method of the request that the middleware function handles - such as GET, PUT, or POST - in lowercase. [Express](https://expressjs.com/en/guide/using-middleware.html#middleware.router)
**Routing Middleware** - Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of `express.Router()`. [Express](https://expressjs.com/en/guide/using-middleware.html#middleware.router)
**Test Driven Development** - software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing software again all test cases. [WIKI](ttps://en.wikipedia.org/wiki/Test-driven_development)

1. Which 3 things had you heard about previously and now have better clarity on?

- Routing Middleware, Application Middleware, REST

2.  Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- TDD, SOAP
