# Class 32: Custom Hooks

## Q and A:

1. What does a component's lifecycle refer to?

- A components lifecycle is defined by 3 things actions: it's **mounting** to the DOM, it's **updating** of the DOM, and it's **unmounting** from the DOM.

2. Why do you sometimes need to "wrap" functions in `useCallback` when called within `useEffect`?

- `useCallback` will return a memoized version of the callback that only changes if one of the dependencies has changed. we wrap functions in `useCallback` inside `useEffect` to avoid re-creating a function on each new render. [SOURCE](https://reactjs.org/docs/hooks-reference.html#usecallback)

3. Why are functional components prefered over class components?

- We dont need the `this` keyword. They can also require fewer lines of code to create. [SOURCE](https://djoech.medium.com/functional-vs-class-components-in-react-231e3fbd7108)

4. What is wrong with the following code?

```js
import React, { useState, useEffect } from "react";

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = [];

  for (let i = 0; i < count; i++) {
    useEffect(() => {
      console.log("component mount/update");
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (
    <div>
      <input type="number" value={count} onChange={changeCount} />
      {renderedItems}
    </div>
  );
}
```

- the function `useEffect` should not be called inside of a forloop.

## Vocab:

- `state hook: `
- `effect hook: `
- `reducrer hook: `
