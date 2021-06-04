# Class 33: Context API

## Q and A:

1. **Describe use cases for `useMemo()` and `useReducer()`**

- NOTE: In short, useMemo calls a function when dependencies change, and memoizes/remembers the result of the function between renders.[SOURCE](https://maxrozen.com/understanding-when-use-usememo)
- `useMemo`:
  - You're noticing a component's render is frustratingly slow, and you're passing a calculation to an unknowable number of children, such as when rendering children using `Array.map()`
  - Your app often becomes unresponsive because you're fetching a large amount of data, and having to transform it into a usable format [SOURCE](https://reactjs.org/docs/hooks-custom.html)
- `useReducer`:
  - When you face complex state logic that involves multiple sub-values or when the next state depends on the previous one.
  - `useReducer` also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks. [SOURCE](https://reactjs.org/docs/hooks-custom.html)

This is in contrast with useCallback which remembers an existing value (typically a function's definition), between renders.

2. **Why do custom hooks need the use prefix?**

- so that react will know that it is a hook, and will treat it as one.

3. **What do custom hooks usually do?**

- they can be used to create and hold reusable functions [SOURCE](https://reactjs.org/docs/hooks-custom.html)

4. **Using any list of custom hooks, research and name one that you think will be useful in your applications?**

- `useContext()` which allows us to subscribe to React context without nesting.

5. **Describe how a hook that fetches API data might work**

- a hook could be created to hold CRUD operations. as such: `[get, put, post, delete] = useAIP()`. This `useAPI` hook could then hold the definition and the functional logic of these differnt actions.

## Vocab:

- `reducer: ` a function which takes two arguments — the current state and an action — and returns based on both arguments a new state. [SOURCE](https://medium.com/react-bootcamp/what-is-a-reducer-in-javascript-f4fd40f98324#:~:text=A%20reducer%20is%20a%20very,both%20arguments%20a%20new%20state.)
