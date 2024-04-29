# Reading Notes 18: AWS: API, Dynamo and Lambda

This topic is important because it introduces new tools that AWS offers.

## AWS API Gateway Overview

What is Amazon API Gateway?

- "Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests."

Why is Amazon API Gateway an important part of the Serverless ecosystem?

- "The API Gateway acts as a single entry point for all incoming requests from clients, like web browsers or mobile apps. It then directs these requests to the appropriate services or functions inside your application. It's responsible for managing, routing, and sometimes even transforming requests before they reach the intended destination." ~ ChatGPT. Amazon API Gateway is how you can manage the requests/routes when using a serverless ecosystem because you don't have your own server but still need to direct to the correct routes and/or manage the requests you receive.

How does API Gateway integrate with other AWS services?

- Many AWS services support integration with Amazon API Gateway, including:
  - AWS Lambda: run Lambda functions to generate HTTP API responses.
  - AWS SNS: publish SNS notifications when an HTTP API endpoint is accessed.
  - Amazon Cognito: provide authentication and authorization for your HTTP APIs.

Source: <https://www.serverless.com/guides/amazon-api-gateway>

## AWS API Gateway

What are the some benefits of using Amazon API Gateway?

- Some benefits of using Amazon API Gateway are efficient API development, performance at any scale, and flexible security controls.

What two API types might you choose from?

- RESTful APIs and WEBSOCKET APIs.

Source: <https://aws.amazon.com/api-gateway/>

## AWS DynamoDB Guide

What is DynamoDB?

- DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS).

Under what circumstances would you recommend DynamoDB over MongoDB?

- DynamoDB is better for applications with a lot of data/big databases. It is also best to use for serverless applications using AWS Lambda.

Source: <https://www.dynamodbguide.com/what-is-dynamo-db/>

## AWS DynamoDB

Explain to a non-technical friend how DynamoDB works.

- DynamoDB is a database that can store data for software applications. It is serverless, so AWS takes care of the server managing for it. You can store, modify, and delete data for applications with DynamoDB.

Source: <https://aws.amazon.com/dynamodb/>

## Dynamoose

What is Dynamoose?

- "Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familiar." ~ [dynamoosejs.com](https://dynamoosejs.com/getting_started/Introduction). It is basically the Mongoose to DynamoDB.

What are some key features of Dynamoose?

- Some key features of Dynamoose are:
  - Type safety
  - High level API
  - Easy to use syntax
  - DynamoDB Single Table Design Support
  - Ability to transform data before saving or retrieving items
  - Strict data modeling (validation, required attributes, and more)
  - Support for DynamoDB Transactions
  - Powerful Conditional/Filtering Support
  - Callback & Promise support
  - AWS Multi-region support

Source: <https://dynamoosejs.com/getting_started/Introduction>

## Reflection

What are your learning goals after reading and reviewing the class README?

- My learning goals are to be able to:
  - Create a DynamoDB Table
  - Create a Lambda function that can operate on a DynamoDB Table
  - Use Dynamoose in a NodeJS Lambda Function

## Thing I want to know about more
