# Class 38 Notes: Redux - Asynchronous Actions

## Q and A:

1. How granular should your reducer's be?

- it is important to modularize your reducers just like we would with our components in an application. Also, when an action would trigger different levels of statechange, it is good practice to have reducers share an action.

2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched?

- can be both, the only con that i understand is that dispatching several times synchronously in a row in the places might affect overall performance. [SOURCE](https://redux.js.org/faq/actions#should-i-dispatch-multiple-actions-in-a-row-from-one-action-creator)

3. Name a strategy for preventing the above.

- make use of the `redux-ignore` or `reduxr-scoped-reducer` to make sure that only certain reducers listen to specific actions.[SOURCE](https://redux.js.org/faq/performance#wont-calling-all-my-reducers-for-each-action-be-slow)

## VOCAB:

- `store: `A store is a state container. store hold the global state of the application. [SOURCE](https://www.tutorialspoint.com/redux/redux_store.htm#:~:text=A%20store%20is%20an%20immutable,need%20to%20specify%20the%20reducer.)

- `combined reducers: `when multiple reduces share the same store. can be accomplished using the `combineReducers()` function.

## 3 Things to learn for next session:

- how can asyncronous programming be incorporated with redux?
- lately i've been passing the entire reducer down as props, would like to go back to what we've done previously for a better way.
- how to interact with the server with redux.
