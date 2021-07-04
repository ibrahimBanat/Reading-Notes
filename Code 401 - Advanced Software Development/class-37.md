# Redux - Combined Reducers

Redux excels at not only global state, but complex global state. Today, we'll be using multiple reducers to manage separate parts of the store.

## Review, Research, and Discussion

1.  Why choose Redux instead of the Context API for global state?

Redux is the industry standard for managing state of large applications, so it is important to know well. It is more optimized for larger projects, because the context API re-renders more often.

2. What is the purpose of a reducer?

We need reducers to tell the application how to change state in response to an action. The action does not do anything except describe what happened and it is up to the reducer to respond to this.

3. What does an action contain?

An action contains a type and whatever payload you want it to have.

4. Why do we need to copy the state in a reducer?

The reducer needs to be a pure function without any side-effects. It should only take in an action and return the new state.
