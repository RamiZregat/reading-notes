# AWS: API, Dynamo and Lambda

# Review, Research, and Discussion

- What are serverless functions? Functions that you don’t care of any things related to server just write the code

- If you were to create a system that emulated Lambda functions, how would you do it? Lambda runs your function only when needed and scales automatically

- Describe how a CDN works? is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user

---

## **Terms**

> Serverless Functions: are single-purpose, programmatic functions that are hosted on managed infrastructure

> Cloud Storage: It is storage model Over internet where data is stored on multiple virtual servers, rather than being hosted on a specific server.

> CDN: refers to a geographically distributed group of servers which work together to provide fast delivery of Internet.
---

## **Preparation Materials**

## AWS API Gateway

- What is Amazon API Gateway?

  - is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

- How does API Gateway work?

  - API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

- what are the benefits of Amazon API getaway?

  - Efficient API development Performance at any scale Cost savings at scale Easy monitoring mongodb Flexible security controls RESTful API options

- How does API Gateway integrate with other AWS services?

  - Many AWS services support integration with Amazon API Gateway, including:

    - AWS Lambda: run Lambda functions to generate HTTP API responses.
    - AWS SNS: publish SNS notifications when an HTTP API endpoint is accessed.
    - Amazon Cognito: provide authentication and authorization for your HTTP APIs.

## AWS DynamoDB

Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.

Many Serverless applications use Amazon API Gateway, which conveniently replaces the API servers with a managed serverless solution.

## Dynamoose

Dynamoose is a modeling tool for Amazon’s DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

**Key Features**

- Type safety
- High level API
- Easy to use syntax
- Ability to transform data before saving or retrieving documents
- Strict data modeling (validation, required attributes, and more)
- Support for DynamoDB Transactions
- Powerful Conditional/Filtering Support
- Callback & Promise support
