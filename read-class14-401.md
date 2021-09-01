# Event Driven Architecture
#### Event-Driven Architecture definition:Event-driven architecture (EDA) is a software design pattern in which decoupled applications can asynchronously publish and subscribe to events via an event broker (modern messaging-oriented-middleware).Event-driven architecture is a way of building enterprise IT systems that lets information flow between applications, microservices and connected devices in a real-time manner as events occur throughout your business, instead of periodically polling for updates.
## Review, Research, and Discussion
- What’s the difference between a FIFO and a standard queue?
#### FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing and ensure that the order in which messages are sent and received is strictly preserved.
- How can the server be assured a message was properly received?
#### by receiving response from the client .
- What classic design pattern is best represented by event driven programming?
#### The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods
- How do you test an event driven system?
#### There are multiple levels of tests you will typically write for your system. In the most canonical case, you will write unit tests, service tests, and end-to-end tests. In each of these cases, your System Under Test (SUT, what is actually being tested) comprises a different part of your application.
## Document the following Vocabulary Terms
* FIFO Queue : FIFO is an abbreviation for first in, first out. It is a method for handling data structures where the first element is processed first and the newest element is processed last
* Pub/Sub :Publish/Subscribe is a simple messaging pattern where a publisher sends messages to a channel without the knowledge of who is going to receive them. Then it is the responsibility of the channel to deliver a copy of the messages to each subscriber. This messaging model enables creation of loosely coupled and scalable systems.
## Preparation Materials 
### (SNS (Simple Notification Service)and SQS(Simple Queue Service))

![](https://miro.medium.com/max/502/1*mdUPKzrfJFuXa4d43KhKUQ.png)
#### Amazon SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. Amazon SNS makes it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services.

![](https://miro.medium.com/max/700/1*7eL3udb6Cto4I9Ly1sN8oA.jpeg)
#### is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can’t be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. Other receivers do not receive the same message later.Polling inherently introduces some latency in message delivery in SQS unlike SNS where messages are immediately pushed to subscribers.


![](https://eadn-wc03-4064062.nxedge.io/cdn/wp-content/uploads/2021/03/SNS_vs_SQS.png)























[Github view](https://github.com/sbkhaloof/growthmindsit)