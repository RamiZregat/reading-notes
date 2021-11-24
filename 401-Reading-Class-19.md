# AWS: Events

## Review, Research, and Discussion

- Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

  - Amazon’s API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.
  - With a few clicks you can create an API that acts as a “front door” for applications to access data, business logic, or functionality from your back-end services, such as workloads running on Amazon Elastic Compute Cloud (Amazon EC2), code running on AWS Lambda, or any Web application. Amazon API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, authorization and access control, monitoring, and API version management.
  - Express Gateway is an API Gateway that can sit at the heart of any micro-services architecture, regardless of what language or platform you’re using. Express Gateway secures your micro-services and exposes them through APIs using Node.js, ExpressJS and Express middleware.

- List the AWS Database offerings and talk about the pros and cons of each

  - Relational ----> Traditional applications, ERP, CRM, e-commerce
  - Key-value ----> High-traffic web apps, e-commerce systems, gaming applications
  - In-memory ----> Caching, session management, gaming leaderboards, geospatial applications
  - Document -----> Content management, catalogs, user profiles
  - Wide Column ----> High scale industrial apps for equipment maintenance, fleet management, and route optimization.
  - Graph ---->Fraud detection, social networking, recommendation engines.
  - Time Series ----> IoT applications, DevOps, industrial telemetry
  - Ledger -----> Systems of record, supply chain, registrations, banking transactions.

- What’s the difference between a FIFO and a standard queue?  
  FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers.

- How can the server be assured a message was properly received?  
  By having the client emit a ‘received’ event back to the server upon receipt of the message.

---

## Terms

> Serverless API: using API Gateway you can create RESTful APIs that enable real-time two-way communication applications, API Gateway supports containerzied and serverless workloads as well as web applications.
> Triggers: An event triggers that will invoke the function handler in the event listener.
> Dynamo vs Mongo:
- MongoDB is vendor agnostic, Open Source, and can be deployed anywhere. DynamoDB is only available on AWS.
- DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas.
- DynamoDB as an integrated AWS service makes it easier to develop end to end solutions.
- DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents. -DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions.

> Dynamoose vs Mongoose: Dynamoose is a modeling tool for Amazon’s DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.
---

## Preparation Materials

### SQS and SNS Basics

- Amazon Simple Queue Service (SQS) and Amazon SNS are both messaging services within AWS, which provide different benefits for developers. Amazon SNS allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, eliminating the need to periodically check or “poll” for updates
- Amazon SQS is a message queue service used by distributed applications to exchange messages through a polling model, and can be used to decouple sending and receiving components.
- SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS

### AWS SQS vs SNS

AWS SNS is a publisher subscriber network, where subscribers can subscribe to topics and will receive messages whenever a publisher publishes to that topic. AWS SQS is a queue service, which stores messages in a queue.

