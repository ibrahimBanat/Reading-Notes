# Redux - Additional Topics

## Review, Research, and Discussion

1. **What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?**

Can use a useEffect() hook to load data on application start.

2. **When using a thunk/async action that dispatches the actual action, which do you export from your reducer?**

You export the actual action from the reducer.

## Vocabulary Terms

- **Middleware**: Code you put in between the framework receiving a request and the framework generating the response (source: [Redux docs](https://redux.js.org/understanding/history-and-design/middleware))
- **Thunk**: Function that wraps an expressio to delay its evaluation (source: [Redux thunk docs](https://github.com/reduxjs/redux-thunk))

## Preparation Materials

### [Redux Toolkit (RTK)](https://redux-toolkit.js.org/)

- `configureStore()` provides simplified config options, combine slice reducers, adds Redux middleware, includes Redux-thunk
- `createReducer()` supply a lookup table of action types to case reducer functions, uses `immer` library to let you write simpler immutable updates
- `createAction()` generates an action creator function for the given action type string
- `createSlice()` accepts an object of reducer functions, a slice name, and an initial state value, creates a slice reducer with corresponding action creators and action types
- `createAsyncThunk` accepts an action type string and a function that returns a promise, generates a thunk that dispatches action based on promise
- `createEntityAdaptor` generates set of reusable reducers adn selectors to manage normalized data in the store
- `createSelector` utility from `Reselect` library re-exported for ease of use
- `npm install @reduxjs/toolkit`

### [Tutorial](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)

- "slice reducer" describes a reducer function responsible for updating a single key/value state
- `createSlice` and `createReducer` wrap function with `produce` from `Immer` library. Can write code that mutates code inside reducer and Immer will return a correct immutably updated result
- `ducks` pattern: "put all action creators and reducers in one file, do named exports of the action creators, and default export of reducer function"  


#### Alternative State Managers

- [MobX](https://mobx.js.org/getting-started.html)
- [HookState](https://hookstate.js.org/)
