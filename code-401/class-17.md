# Reading Notes 17: AWS: S3 and Lambda

This topic is important because it introduces new tools that AWS offers.

## AWS S3

What is Amazon S3?

- Amazon S3 is object storage built to retrieve any amount of data from anywhere.

Name some use cases for Amazon S3.

- Some use cases for Amazon S3 are running cloud-native applications, archiving data at the lowest cost, and building a data lake.

Name some benefits of using Amazon S3.

- Some benefits of using Amazon S3 are cloud storage, high performance, and security.

Source: <https://aws.amazon.com/s3/>

## AWS Lambda Basics

What is AWS Lambda?

- "AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner. The Lambda functions can perform any kind of computing task, from serving web pages and processing streams of data to calling APIs and integrating with other AWS services." ~ [serverless.com](https://www.serverless.com/aws-lambda)

Name some use cases for AWS Lambdas.

- Making scalable APIs.
- Data processing. "you could employ Lambda to do some work every time an item in DynamoDB is created or updated, thus making it a good fit for things like notifications, counters and analytics." ~ [serverless.com](https://www.serverless.com/aws-lambda)

Describe “serverless” to a non-technical friend.

- "Serverless", in this case, means that the server is being managed by AWS rather than the AWS users themselves.

Source: <https://www.serverless.com/aws-lambda>

## CDN

What is a CDN?

- "A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos."

How does a CDN work with relation to the website visitor?

- "CDNs work through servers nearest to the website visitor respond to the request. The content delivery network copies the pages of a website to a network of servers that are spread out at geographically different locations, caching the contents of the page. When a user requests a webpage that is part of a content delivery network, the CDN will redirect the request from the originating site’s server to a server in the CDN that is closest to the user and deliver the cached content. CDNs will also communicate with the originating server to deliver any content that has not been previously cached. In turn, the speed is improved by distributing content closer to the website visitors by using a nearby CDN server, causing visitors to experience faster page loading times."

What are the benefits of employing a CDN?

- The benefits of employing a CDN is faster loading speeds. If you are in a location far from the server for the site you are trying to access, you can access the site from a server in the CDN that is nearby instead (which will improve loading times). Another benefit is bandwidth saving because they cache the content that they serve locally.

Source: <https://cyberhoot.com/cybrary/content-delivery-network-cdn/>

## Reflection

What are your learning goals after reading and reviewing the class README?

- My learning goal is to learn how to use a Lambda with AWS.

## Thing I want to know more about
