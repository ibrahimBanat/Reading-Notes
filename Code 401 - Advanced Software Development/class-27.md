# Props and State

Applications are comprised of many components, usually working together to perform a higher level task. As such, they'll all need access to state, methods to read/modify state, and an ability to respond to triggered actions in other, related components. Today, we'll explore how React applications do this, using JSX attributes, better known as `props`.

## Review, Research, and Discussion

1. Does a deployed React application require a server?

You don't necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app.

2. Why do we prefer to test a React application at the behavior rather than the unit level?

When it comes to React components you want to check how your component is rendered and if all props you pass to the component influence the behavior of your component as expected.

Some tools offer a very quick feedback loop between making a change and seeing the result, but don’t model the browser behavior precisely. Other tools might use a real browser environment, but reduce the iteration speed and are flakier on a continuous integration server.

3. What does npm run build do?

runs the script "build" and created a script which runs your application

4 - Describe the actual composition / architecture of a React application

- The actual composition

The key feature of React is composition of components. Components written by different people should work well together. It is important to us that you can add functionality to a component without causing rippling changes throughout the codebase.

- Architecture

Unlike other UI libraries and frameworks, Reactjs doesn’t enforce an architecture pattern. It is just a view that caters to the user interface.

## Vocabulary Terms

| Term             | Defintion                                                                                                                                                                                        |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BDD              | behavior-driven development (BDD) is an Agile software development process that encourages collaboration among developers, QA, and non-technical or business participants in a software project. |
| Acceptance Tests | is a formal description of the behavior of a software product, generally expressed as an example or a usage scenario.                                                                            |
| mounting         | This method is called just before a component mounts on the DOM or the render method is called. After this method, the component gets mounted.                                                   |
| build            | It saves you from time-consuming setup and configuration. You simply run one command and create react app sets up the tools you need to start your React project.                                |

### React SetState

React components with state render UI based on that state. When the state of components changes, so does the component UI.

`setState()` is the only legitimate way to update state after the initial state setup.

## Handling Events

- React events are named using camelCase, rather than lowercase.

- With JSX you pass a function as the event handler, rather than a string.

## React Forms

Just like in HTML, React uses forms to allow users to interact with the web page.

Handling Forms

- Handling forms is about how you handle the data when it changes value or gets submitted.

- In React, form data is usually handled by the components.

- When the data is handled by the components, all the data is stored in the component state

## React State

- React components has a built-in state object.

- The state object is where you store property values that belongs to the component.

- When the state object changes, the component re-renders.

## React Lifecycle

Lifecycle of Components

- Each component in React has a lifecycle which you can monitor and manipulate during its three main phases.
- The three phases are: Mounting, Updating, and Unmounting.

Mounting

- Mounting means putting elements into the DOM.
  React has four built-in methods that gets called, in this order, when mounting a component:

- `constructor()`
- `getDerivedStateFromProps()`
- `render()`
- `componentDidMount()`

The `render()` method is required and will always be called, the others are optional and will be called if you define them.

### React Components

Components are independent and reusable bits of code. They serve the same purpose as JavaScript functions, but work in isolation and return HTML via a render() function.

Components come in two types, Class components and Function components, in this tutorial we will concentrate on Class components.

### React Props

React Props are like function arguments in JavaScript and attributes in HTML.

### React Testing Library

React Testing Library builds on top of DOM Testing Library by adding APIs for working with React components.
