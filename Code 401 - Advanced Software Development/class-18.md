# AWS: API, Dynamo, and Lambda

## Review, Research, and Discussion

1. **What’s the difference between a FIFO and a standard queue?**

FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing and ensure the order in which messages are sent and received is strictly preserved (source: [Medium](https://medium.com/awesome-cloud/aws-difference-between-sqs-standard-and-fifo-first-in-first-out-queues-28d1ea5e153))

2. **How can the server be assured a message was properly received?**

By having the client emit a "received" event back to the server upon receipt of the message

3. **What classic design pattern is best represented by event driven programming?**

Observer design pattern, an object (subject) maintains a list of its dependents (observers) and notifies them automatically of any state changes usually by calling one of their methods (source: [Wikipedia](https://en.wikipedia.org/wiki/Observer_pattern))

4. **How do you test an event driven system?**

With unit tests which test individual components of the system, as well as tests for verifying the server and clients are communicating back and forth

## Vocabulary Terms
- **Serverless Functions**: programmatic function written by a software developer for a single purpose, which is then hosted and maintained on infrastructure by cloud computing companies that take care of code maintenance and execution so that developers can deploy new code faster and easier (source: [Hubspot](https://blog.hubspot.com/website/serverless-functions))
- **Cloud Storage**: cloud computing model that stores data on the internet through a cloud computing provider who manages and operates data storage as a service (source: [AWS](https://aws.amazon.com/what-is-cloud-storage/))
- **CDN**: content delivery network, a geographically distributed group of servers that work together to provide fast delivery of internet content (source: [Cloudflare](https://www.cloudflare.com/learning/cdn/what-is-a-cdn/))


## AWS API Gateway

- Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic
- Also handles authentication, access control, monitoring, and tracing of API requests
- API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends
- It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services
- Can also generate API references from your definitions and make them available to your users as API documentation
- Integrates with many other AWS services, which allows for fully managed authentication and authorization layers as well as detailed metrics and tracing for API requests

## AWS DynamoDB

- DynamoDB is a hosted NoSQL database offered by AWS
- It offers a reliable performance even as it scales, a managed experience so you don't need to be SSH-ing into servers, a small and simple API allowing for simple key-value access as well as more advanced query patterns
- Particularly good fit for:
  - Applications with large amounts of data and strict latency requirements
  - Serverless applications using AWS Lambda
  - Data sets with simple, known access patterns

## Dynamoose

- Modeling tool for DynamoDB, heavily inspired by Mongoose
- Key features: type safety, high level API, easy to use syntax, ability to transform data before saving or retrieving documents, strict data modeling (validation, required attributes, and more), support for DynamoDB transactions, powerful conditional/filtering support, callback and promise support
