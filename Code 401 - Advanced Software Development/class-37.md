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

## Vocabulary Terms

| Word                 | Definition                                                                                                                                                           |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| immutable state      | This allows the state to only change when absolutely necessary to make React apps perform as well as possible.                                                       |
| time travel in redux | This is a feature of redux dev tools that allows you to see every state that a page has been in.                                                                     |
| action creator       | Actions send data from your application to your store, and are the only source of information for the store. An action creator is a function that creates an action. |
| reducer              | Reducers tell the application how to change state in response to an action. dispatch This is the name of the function you use to send actions to the store.          |
| dispatch             | The only way to update the state is to call `store.dispatch()` and pass in an action object                                                                          |
