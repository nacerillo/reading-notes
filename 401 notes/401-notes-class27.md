# Reading Notes - Class 27:

## Q and A:

1. Does a deployed React application require a server?

- Not necessarily. however, you do have the option of creating a server.

2. Why do we prefer to test a React application at the behavior rather than the unit level?

- because unit tests are meant to tackle issues from the developer's perspective, not from the User's perspective. Behaviour Based Testing is meant to create tests that are readable for the user - IE the ones that would be interacting with the Frontend.

3. What does `npm run build` do?

- this command can be used in the deployment phase. it creates a `build` directory to contain a production build of your react app.

4. Describe the actual composition / architecture of a React application

- A React application is made up of components. in their purest form, components can be nothing more than the rendering of elements on a page. however, components can also have state and props. as a user interacts with the interface, the react components send and recieve information through the sharing of state and props to perform the tasks that they were designed for.

## Vocab:

- `BDD:` Behaviour Driven Development. developmen that comes from communication/collaboration between developers, QA, and non-technical participants. [SOURCE](https://en.wikipedia.org/wiki/Behavior-driven_development)
- `Acceptance Test:` The level of testing where a system of piece of a system is tested not just to see if it "works" but to see if it is compliant with business requirements. it is testing done with respect to the use's needs. [SOURCE](https://softwaretestingfundamentals.com/acceptance-testing/#:~:text=ACCEPTANCE%20TESTING%20is%20a%20level,ISTQB%20Definition)
- `mounting:` refers to how react interacts with the DOM. adding or changing of nodes in the DOM. [SOURCE](https://en.wikipedia.org/wiki/Behavior-driven_development)
- `build:` the production version of your app. this can be created using the `npm build` command.

## Preview:

1. I have a better understanding of how state can be set, and how props can be used to pass data from parent to child. I also have a better understanding of how we can pretty-fiy json data. By using either the third arguement in the `JSON.Stringfy()`, or by using the `react-json-view` module.
2. I hope we can learn how to better design and arrange our applications. and also how to recreate api calls such as PUT, DELETE, and UPDATE for the purposes of our labs this week. I also still need to work on how to do deployment.
3. I am most excited learning more about good-react design.
