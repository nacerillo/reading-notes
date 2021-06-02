# Class 31: Hooks API

## Q and A:

1. Why do we not need more .html pages in React app?

- because, thanks to JSX, we implement our markup and JS logic inside the same component-files.

2. If we wanted a component to show up on every page, where would we put it and why?
   - Outside of `<BrowserRouter/>`.
   - Inside the `<BroswerRouter/>`.
   - Inside a `<Route/>`.

- inside the `<BrowserRouter/>` but outside of any `<Route/>`. `<BrowserRouter/>` would have to wrap around the entire application. but as long as it isnt wrapped inside a route, items will render on every page. Examples: Headers and Footers. items that are inside of `<Route/>` would ONLY render on that route.

3. What does props.children contain?

- it contains any child elements/props defined within a component.

## Vocab:

- `Compositon: `A development/design patter that is based around the idea that we can build components out of other, smaller components. enforcing state management and reusability.
- `Child Components: `components that are called on by another component. a child component can recieve data/props from a parent.
- `Hash Routing: `part of legacy react. it is routing that uses the hast portion of the URL to keep the UI in sync with the current URL. [SOURCE](https://reactrouter.com/web/api/HashRouter)
- `Link Routing: `a declartive way to navigate to a point in the application.
  Example:[SOURCE](https://reactrouter.com/web/api/Link)

```js
<Link to="/about">About</Link>
```
