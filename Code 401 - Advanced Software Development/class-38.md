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
