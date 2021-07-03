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
