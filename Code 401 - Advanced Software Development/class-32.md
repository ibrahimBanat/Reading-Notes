# Custom Hooks

Below you will find some reading material, code samples, and some additional resources that support today's topic and the upcoming lecture.

## Review, Research, and Discussion

1. What does a component’s lifecycle refer to?

   it refers to the time from when a component mounts to when it umount. There are methods that you can call associated with it.

2. Why do you sometimes need to “wrap” functions in `useCallback` when called from within `useEffect`?

   because it fires a memoized version of the callback only if one of it's dependents has changed. This makes it faster and more efficient.

3. Why are functional components preferred over class components?

   Functional components are less code, easier to read, perform better, and make it easier to separate components.

4. What is wrong with the following code?

```javasccript
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```

    `useEffect` should be outside of the for loop in this example.

## Vocabulary Terms

| Term         | Definition                                                                                                                                                   |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| state hook   | like `useState` is a Hook that lets you add React state to function components.                                                                              |
| effect hook  | The Effect Hook lets you perform side effects in function components                                                                                         |
| reducer hook | is used to store and update states, just like the `useState` Hook. It accepts a reducer function as its first parameter and the initial state as the second. |

## Preview

- Custom Hooks

  The easiest way to describe Hooks is to show side-by-side examples of a class component that needs to have access to state and lifecycle methods, and another example where we achieve the same thing with a functional component.

  - The Benefits of Using Hooks
    Hooks have a lot of benefit to us as developers, and they are going to change the way we write components for the better.
  - Important Rules for Hooks

    1. Never call Hooks from inside a loop, condition or nested function
    1. Hooks should sit at the top-level of your component
    1. Only call Hooks from React functional components
    1. Never call a Hook from a regular function
    1. Hooks can call other Hooks
    1. React Hooks with Async-Await
