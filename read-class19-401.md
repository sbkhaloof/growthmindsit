# AWS: Events
## Review, Research, and Discussion
+ Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server
#### AWS API Gateway and Lambda functions together can work almost exactly like an express server. In an express server, you make routes and then you fire them with functions. In AWS, you make routes in API Gateway and they trigger a Lambda function to run
+ List the AWS Database offerings and talk about the pros and cons of each
#### AWS database offerings include:

1. RDS
2. DynamoDB
3. ElastiCache
4. Neptune
5. Amazon QLDB
6. Amazon DocumentDB
7. Amazon Keyspaces
8. Amazon Timestream
#### They are each comparable to different db services. RDS is similar to oracle SQL, DynamoDB is similar to MongoDB, Aurora is MySQL, postrgeSQL compatible, etc.
#### Pros: They are scalable, managed, secure, easy to work with, and scalable Cons: The only major con I can see is the cost.
+ What’s the difference between a FIFO and a standard queue?
#### A FIFO queue is first in, first out. A standard queue is more randomized, but guarantees that an item is only ‘delivered’ once, meaning if an item leaves the queue it is now gone from the queue.
+ How can the server be assured a message was properly received?
#### Logging and using timestamps and checking whether it was delivered based on the response sent from the endpoint.
## Document the following Vocabulary Terms
* Serverless API: An API that lives in the cloud and is created using cloud services.
* Triggers: Triggers are stored programs, which are automatically executed or fired when some events occur.
* Dynamo vs Mongo : (1) DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas. (2) DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents. (3) DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions. Xplenty (L
* Dynamoose vs Mongoose: Both are modeling/schema tools for their corrosponding databases (Dynamo and Mongo). Dynamoose is heavily inspired by Mongoose

## Preparation Materials
### SQS and SNS Basics 
#### SNS (Simple Notification Service)
![](https://miro.medium.com/max/502/1*mdUPKzrfJFuXa4d43KhKUQ.png)
#### Amazon SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. Amazon SNS makes it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services.
#### SQS (Simple Queue Service)
![](https://miro.medium.com/max/700/1*7eL3udb6Cto4I9Ly1sN8oA.jpeg)
####  is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can’t be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. Other receivers do not receive the same message later.


[Github view](https://github.com/sbkhaloof/growthmindsit)