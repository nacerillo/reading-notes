# Class 37 Notes: Combined Reducers:

## Q and A:

1. Why choose Redux instead of the Context API for global state?

-

2. What is the purpose of a reducer?

- the purpose of a reducer is to evaluate the actions that are passed to it, and in turn help to manage the state change of an application.

3. What does an action contain?

- an action contains a TYPE, which is a string used to mark what kind of action is taking place, and PAYLOAD, data that will be be used to change the state on the action.

4. Why do we need to copy the state in a reducer?

- so that we do not override the current global state of the application.

## VOCAB:

- `immutable state:` State that cannot be changed in any way.
- `time travel in redux:` Refers to the fact that we can use Redux dev tools to see the past state and actions that have triggered in the application.
- `action creator: `A function that creates an action. these functions return an action object, which consists of just a TYPE and a PAYLOAD. [SOURCE](https://www.educative.io/courses/building-teslas-battery-range-calculator-with-react-and-redux/7nVVPYOGVPr)
- `reducer:` a function that evaluates actions, and manages the changing of state when an action occurs. [SOURCE](https://css-tricks.com/understanding-how-reducers-are-used-in-redux/#:~:text=A%20reducer%20is%20a%20function,receives%20to%20determine%20this%20change.&text=Redux%20relies%20heavily%20on%20reducer,to%20execute%20the%20next%20state.)
- `dispatch:` a Redux funtion of the store that is called when we want to let the store know that an action has been triggered. [SOURCE](https://react-redux.js.org/using-react-redux/connect-mapdispatch#:~:text=dispatch%20is%20a%20function%20of,connect%20does%20it%20for%20you.)
