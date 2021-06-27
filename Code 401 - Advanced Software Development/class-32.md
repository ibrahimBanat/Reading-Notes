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
