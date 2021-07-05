## Redux - Asynchronous Actions

Connecting a Redux application to a backend service (i.e. an API) requires a bit of additional work, as asynchronous actions can cause issues with the internal Redux store management mechanisms. Today, we will be exploring Redux middleware, specifically "Thunk" which provides the mechanism to work asynchronously with Redux

1. How granular should your reducers be?

There should be a separate reducer function for each slice of data. They are combined before being put into the store.

2. Pro or Con - multiple reducers can "fire" when a commonly named action is dispatched

This is a Con because you may fire off reducers that you did not intend.

---

3. Name a strategy for preventing the above

You can use more specific names that represent the reducer and data want to change .

## Vocuabulary Terms

| Word              | Definition                                                                                                  |
| ----------------- | ----------------------------------------------------------------------------------------------------------- |
| store             | This holds the state of the application. This can only be changed when actions are dispatched to the store. |
| combined reducers | This takes all the reducer functions from an app and combines them to pass to createStore.                  |

## Preview

### Understanding Asynchronous Redux Actions with Redux Thunk

Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.

There are two very popular middleware libraries that allow for side effects and asynchronous actions: `Redux Thunk `and `Redux Saga`

`Thunk` is a programming concept where a function is used to delay the evaluation/calculation of an operation.

### Redux Middleware and Side Effects

a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

- Some common kinds of side effects are things like:

- Logging a value to the console
- Saving a file
- Setting an async timer
- Making an AJAX HTTP request
- Modifying some state that exists outside of a function, or mutating arguments to a function
- Generating random numbers or unique random IDs (such as Math.random() or Date.now())
