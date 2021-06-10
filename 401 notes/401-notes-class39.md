# Class 39 Notes: Redux- Additional Topics:

## Q and A:

1. What’s the best practice for “pre-loading” data into the store - on application start - in a Redux application?

- Best way way of handling thedata would be to trigger the async action in the lifecycle method (probably `componentWillMount`) of a Higher Order Component that wraps your app. However, do not use the results of the API call directly in that component - it needs to be handled with a reducer that puts it into the app store. This will require the use some sort of thunk middleware to handle the async action. Then use `mapStateToProps` to simply pass it down to the component that renders the data [SOURCE](https://stackoverflow.com/questions/39356517/correct-way-to-pre-load-component-data-in-reactredux)

2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

- export the action creator from the reducer.[SOURCE](https://medium.com/@stowball/a-dummys-guide-to-redux-and-thunk-in-react-d8904a7005d3)

## Vocab:

- `middleware:` software that provides common services and capabilities to app outside of what is normally offered by the OS. in the context of redux, middlware provides an extentison point between dispatching an action, and the moment that it reaches the reducer [SOURCE1](https://www.redhat.com/en/topics/middleware/what-is-middleware#:~:text=Middleware%20is%20software%20that%20provides,offered%20by%20the%20operating%20system.&text=Middleware%20helps%20developers%20build%20applications,applications%2C%20data%2C%20and%20users.)[SOURCE2](https://redux.js.org/understanding/history-and-design/middleware
- `thunk:`middleware designed for redux that allows us to return a function instead of just an action. this allows us to make async action calls.[SOURCE](https://www.freecodecamp.org/news/redux-thunk-explained-with-examples/)
