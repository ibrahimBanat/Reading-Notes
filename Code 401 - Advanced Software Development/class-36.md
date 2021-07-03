# Application State with Redux

Managing global state at the application level can definitely be a challenge. While the Context API provides a mechanism to accomplish this very tactically, Redux is a library that specializes in sharing state between components using a global "Store"

## Review, Research, and Discussion

1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”

Cookies are read server-side, and local storage is read client-side, so if the server needs the data, then it is better to use cookies.

2. Explain 3rd party cookies.

Tracked by websites other than the one you are currently visiting.

3. How do pixel tags work?

Pixel tags are typically single pixel, transparent GIF images that are added to a web page. Even though the pixel tag is virtually invisible, it is still served just like any other image you may see online.

## Vocabulary Terms

| Word                  | Definition                                                                                                                                                |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| cookies               | They are pieces of code that web servers use to put information on a user’s browser, and then retrieve that information at a later time for various uses. |
| authorization         | Authorized the user to go to different areas based on what they are allowed to see and do                                                                 |
| access control        | This restricts access to different areas of a network based on a person's role in an organization.                                                        |
| conditional rendering | Check some logic before render the user certain components.                                                                                               |

## Redux

- What is Redux ?

Redux is a pattern and library for managing and updating application state, using events called "actions".

It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience

- Why Should I Use Redux?

Redux helps you manage "global" state - state that is needed across many parts of your application

- When Should I Use Redux?

Redux helps you deal with shared state management, but like any tool, it has tradeoffs. There are more concepts to learn, and more code to write. It also adds some indirection to your code, and asks you to follow certain restrictions. It's a trade-off between short term and long term productivity.

    - Redux is more useful when:

    - You have large amounts of application state that are needed in many places in the app

    - The app state is updated frequently over time

    - The logic to update that state may be complex

    - The app has a medium or large-sized codebase, and might be worked on by many people

## Redux Terms and Concepts

- State Management

It is a self-contained app with the following parts:

    - The state, the source of truth that drives our app

    - The view, a declarative description of the UI based on the current state

    - The actions, the events that occur in the app based on user input, and trigger updates in the state

- Immutability

"Mutable" means "changeable". If something is "immutable", it can never be changed.

- Terminology

There are some important Redux terms that you'll need to be familiar with

    - Actions : An action is a plain JavaScript object that has a type field

    - Action Creators : An action creator is a function that creates and returns an action object.

    - Reducers : A reducer is a function that receives the current `state` and an `action` object, decides how to update the state if necessary, and returns the new state: (`state`, `action`) => newState.

    - Store : The store is created by passing in a reducer, and has a method called `getState` that returns the current state value

    - Dispatch : The only way to update the state is to call `store.dispatch()` and pass in an action object

    - Selectors : Selectors are functions that know how to extract specific pieces of information from a store state value
