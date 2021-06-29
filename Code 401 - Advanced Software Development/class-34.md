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

## Preview

- What is Role-Based Access Control (RBAC) ?

  In computer systems security, role-based access control or role-based security is an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees, and can implement mandatory access control or discretionary access control.

  BENEFITS OF RBAC

        - Reducing administrative work and IT support
        - Maximizing operational efficiency
        - Improving compliance

- React-cookies

  Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.

  To set or remove the cookies, we are using a third-party dependency of react-cookie
