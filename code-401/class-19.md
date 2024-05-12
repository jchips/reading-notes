# Reading Notes 19: AWS: Events

This topic is important because it introduces new tools that AWS offers.

## AWS SQS vs SNS

What is the difference betweeen SQS and SNS?

- SQS stands for Simple Queue Service. It is "a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications." It is a queuing system where messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can be stored in SQS for short duration of time (max 14 days).
- SNS stands for Simple Notification Service. Amazon SNS is a fully managed push notification service that lets users send individual messages or bulk messages to large numbers of recipients. It is a distributed publish-subscribe system. With Amazon SNS, users can push notifications to mobile device users, email recipients or even send messages to other distributed services.

What are some use cases for both SNS and SQS?

- For SNS, some use cases are: "You would like to be able to publish and consume batches of messages, you would like to allow same message to be processed in multiple ways, multiple subscribers are needed, or you want to fan-out messages to a large number of subscribers."
- For SQS, some use cases are: "You need a simple queue with no particular additional requirements, only one subscriber is needed, you need your messages received sequentially and without any loss even if some parts fail or the network experiences disruptions."

Source: <https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5>

## AWS SNS and SQS

Describe how to use SQS and SNS in a “fanout” pattern.

1. Create a SNS topic subscribe a SQS to it (can subscribe more than one)
2. Publish a message to the SNS topic
3. This message will get added to the SQS
4. Recieve messages from the SQS
5. Delete recieved messages from the SQS

Explain how “push notifications” work, using SNS.

1. Create an SNS topic
2. Subscribe your mobile devices or application servers (endpoints) that you want to receive push notifications on to the SNS topic
3. Publish a message to the SNS topic
4. The SNS topic will send the published message to the subscribed endpoints
5. For each subscribed endpoint, SNS will deliver the message using their approciate protocol. For example, there's APNS for IOS, FCM for Android, and SMTP for email addresses.

Source: <https://www.youtube.com/watch?v=mXk0MNjlO7A> and ChatGPT

## SQS and SNS Basics

How might a large scale, distributed application make use of a Queue system like SQS?

- A large scale, distributed application might make use of SQS by decoupling (designing modules and components independent of each other), scaling the application, and processing messages asyncronously.

Source: <https://www.youtube.com/watch?v=UesxWuZMZqI>

## Reflection

My learning goals are to learn how to create a notification topic that triggers an action and to be able to create a Queue that retains messages (both using AWS).

## Things I want to know more about
