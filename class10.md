# Class 10;

## Error Handeling & Debugging:

- for debugging, it is important to understand _order of executution_.
- Executuon Context:

  - global context
  - function context

- **hoisting:** calling on a function before it has been declared in code. or assigning value to a variable that has not yet been declared.
- each execution context creates its own _variable object_.

### Errors:

- **exceptions:** messages output by the computer when an error occurs in code.
- when errors occur, we can using exception-handling in our code to tell the computer what to do when we run int specific errors.
- Error Object is cast by message, and has the following properties

  - name
  - message
  - fileNumber
  - lineNumber

- seven types of error objects.

  - Error: generic
  - SyntaxError: incorrect syntax
  - ReferenceError: failed to reference a variable that was not declared
  - TypeError: unexpected data type was cast
  - RangeError: numbers or indicies out of range
  - URIError: incorrect usage of URI methods
  - EvalError: incorrect usage of eval method

- Errors can be dealt with either through debugging, or just handleing.

  - sometimes errors will occur due to issues outside of our control, which makes handeling an option seperate from straight debugging.

- Must be able to find WHERE the problem is, and know WHAT it is.

  - **Breakpoints:** setting stopping points in your code that sets the execution of the code on pause at a specific point. good for seeing what is happening with data at a specific point in code.

- Browser Dev Tools and console are also very useful for finding where
- find errors in the console, and can also write test code into console.

### Exception Handeling/ TryCatch

- can handle errors/exceptions in code by wrapping code inside of a try/catch block.
  - try: first specificy the code that you wish run to. code wrapped in the try block will be examined.
  - Catch: catch an exception if one is thrown by the try block.
  - Finally: code that will always run after the code in the try/catch.

```js
try {
  //try to execture this code
} catch (exception) {
  //If there is an exception, run the code wrapped in catch()
} finally {
  // always run this code wrapped in finally
}
```

- can also generate our own errors using `throw new Error('message')`.

### Debugging tips:

- can try running in different browser
- add to variables, and log variables values to the console.
- use the search tool to find specific elements
- USE BREAKPOINTS
