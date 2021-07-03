# Application State with Redux

Managing global state at the application level can definitely be a challenge. While the Context API provides a mechanism to accomplish this very tactically, Redux is a library that specializes in sharing state between components using a global "Store"

## Review, Research, and Discussion

1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”

Cookies are read server-side, and local storage is read client-side, so if the server needs the data, then it is better to use cookies.

2. Explain 3rd party cookies.

Tracked by websites other than the one you are currently visiting.

3. How do pixel tags work?

Pixel tags are typically single pixel, transparent GIF images that are added to a web page. Even though the pixel tag is virtually invisible, it is still served just like any other image you may see online.
