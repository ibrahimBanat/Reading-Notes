# `<Login />` and `<Auth />`

we will combine Authentication (valid user is logged in) and Authorization (what permissions does the user have) to create a UI that ensures that users only have access to content and functionality that they're granted access to.

## Review, Research, and Discussion

1. Why is the Context API useful?

   The Context API is useful because it can change important values for many components at once from a centralized location, without all of the values having to be passed through many layers of props.

2. Can a component outside of a provider get its context?

   No, it's need to be wrapped between the provider.

3. What are some common use cases for using the Context API?

   Change the theme and as the profile data for the user to be access in any where inside the components

4. Describe `Context Hell`

   Without useContext, you may need to pass or drilling props to each components in the app to be access for the components that will consume it.

## Vocabulary Terms

| Word           | Definition                                                                                                                               |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| global state   | This is the state of the entire React application that located in the context.                                                           |
| global context | This is context that affects the entire application, and it will share data to everything in the React component tree.                   |
| provider       | The context provider accepts a value that will be passed to its children. All children components will re-render when the value changes. |
| consumer       | This is a React component that subscribes to context changes in value of the Provider.                                                   |
