# Express REST API

reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

## Review, Research, and Discussion

1. Name 3 real world use cases where you’d want to change the request with custom middleware

   - Handling Authentication/Authorization/Auditing.
   - Custom CSRF middleware to skip/check on specific requests.
   - forcing users to use Https.

2. True or false: The route handler is middleware?

   - false

3. In what ways can a middleware function end the process and send data to the browser?

   - must call `next()` to pass control to the next middleware

4. At what point in the request lifecycle can you “inject” middleware?

   - in the requests and responses

5. What can cause express to error with “Request headers sent twice, cannot start a second response”

   - The problematic middleware sets the response header without calling response.end() and calls next(), which confuses connect's server.

## Vocabulary Terms

|        **word**         |                                                                         **definition **                                                                          |
| :---------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|       Middleware        | functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. |
|     Response object     |                               The res object represents the HTTP response that an Express app sends when it gets an HTTP request.                                |
| Application Middleware  |                                                 Middleware that plays a role in the function of the application.                                                 |
|   Routing Middleware    |                                                        a middleware that works on router level router.use                                                        |
| Test Driven Development |                        is software development approach in which test cases are developed to specify and validate what the code will do.                         |
|   Behavioral Testing    |                                                         Testing of the external behavior of the program.                                                         |
|     Request Object      |              The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on               |
