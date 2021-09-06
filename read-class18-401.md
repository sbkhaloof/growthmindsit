# AWS: API, Dynamo and Lambda
## Review, Research, and Discussion

1. What are serverless functions?
###  is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.
2. If you were to create a system that emulated Lambda functions, how would you do it?
### To create a Lambda function with the console

* Open the Functions page on the Lambda console.

* Choose Create function.

* Under Basic information, do the following:

1.  For Function name, enter my-function.

2.  For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.

* Choose Create function.
3. Describe how a CDN works
### it stands for content delivery network. A CDN is essentially a group of servers that are strategically placed across the globe with the purpose of accelerating the delivery of your static web content.

## Document the following Vocabulary Terms

+ Serverless Functions :is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.
+ Cloud Storage :Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It’s delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure. This gives you agility, global scale and durability, with “anytime, anywhere” data access.

+ CDN :it stands for content delivery network. A CDN is essentially a group of servers that are strategically placed across the globe with the purpose of accelerating the delivery of your static web content.

## Preparation Materials
### Amazon API Gateway
![](https://d1.awsstatic.com/serverless/New-API-GW-Diagram.c9fc9835d2a9aa00ef90d0ddc4c6402a2536de0d.png)
#### Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. APIs act as the "front door" for applications to access data, business logic, or functionality from your backend services. Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.
#### Benefits
+ Efficient API development
+ Performance at any scale
+ Cost savings at scale
+ Easy monitoring
+ RESTful API options

###  DynamoDB
![](https://pattern-match.com/images/services/amazon-dynamodb.png)
#### s a fast and flexible NoSQL database service. It's suitable for any applications that require a stable work with a delay of no more than a few milliseconds at any scale and it's a fully managed database. DynamoDB supports data models like key-value pair and document data structures. DynamoDB is allowed to be used for web apps or mobile apps, games, different platforms and the "Internet of things" and other applications due to it's flexibility and reliability.
### Dynamoose : Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.


[Github view](https://github.com/sbkhaloof/growthmindsit)