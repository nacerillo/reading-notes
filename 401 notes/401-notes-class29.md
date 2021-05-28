# Class 29: Routing

## Q and A:

1. Do child components have direct access to props/state from the parent?

- parent components can pass down state AS props to child components

2. When a component “wraps” another component, how does the child component’s output get rendered?

- a child that is wrapped up by another component will typically render when the parent is also rendered.

3. Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?

- Yes. this is basically what we did in lab29, where we have the homepage render history when a method is ran, while at the same time we could call history as a stand-alon component on a different route.

4. What trick can a parent use to share all props with it’s children

- this can be done by using the `...` spread operator.

## Vocab:

- `props.children:` can be used to allow a parent component to pass down props without actually know what child-components it will pass them to.

- `composition:` It is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these components are, they can be used in building many other components.
