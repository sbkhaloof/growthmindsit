# Socket.io
## Review, Research, and Discussion
1. What is the benefit of transforming data into packets? 
+ to meet the demands of pervasive data-centric applications and services
+ A file has to be broken up into small chunks of data

2. UDP is often refereed to as a connectionless protocol. Why is this?
#### UDP(user datagram protocol) A transport layer communication protocol, UDP is a very common protocol for voice and video traffic.
+ It speeds up communications by not formally establishing a connection before data is transferred. This allows data to be transferred very quickly. 
3. Can a socket server application have multiple socket connections?
#### yes, Multiple connections on the same server can share the same server-side IP/Port pair
4. Can a socket connection application be connected to multiple socket servers?
#### A server socket listens on a single port. All established client connections on that server are associated with that same listening port on the server side of the connection. An established connection is uniquely identified by the combination of client-side and server-side IP/Port pairs. Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to
5. Can an application be both a socket server and a socket connection?
#### no
## Document the following Vocabulary Terms
* Observer Pattern: The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.
* Listener: (handler function) : It is function which respond to the event occur.
* Event Handler : code can be made to run when an event is triggered by assigning it to the target element's corresponding onevent property, or by registering the handler as a listener for the element using the addEventListener() method. 
* Event Driven Programming : is a programming paradigm in which the flow of the program is determined by events such as user actions (mouse clicks, key presses), sensor outputs, or message passing from other programs or threads.
* Event Loop :In computer science, the event loop is a programming construct or design pattern that waits for and dispatches events or messages in a program
* Event Queue :An event queue is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system
* Call Stack: The call stack is a LIFO (Last In, First Out) stack. The event loop continuously checks the call stack to see if there’s any function that needs to run. While doing so, it adds any function call it finds to the call stack and executes each one in order.
* Emit/Raise/Trigger:functions called listeners to be called ... raise -->/Fire the event document. dispatchEvent(event) .. trigger-->The trigger() method triggers the specified event and the default behavior of an event (like form submission) for the selected elements. This method is similar to the triggerHandler() method, except that triggerHandler() does not trigger the default behavior of the event

* database:is an organized collection of structured information, or data, typically stored electronically in a computer system.


## Preparation Materials

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRDxW4bH55yGnH1vtJsvSWBqcj3Ff8OBgmC9Q&usqp=CAU)

#### WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.
#### Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.

1. Client-Side: it is the library that runs inside the browser
2. Server Side: It is the library for Node.js

#### WebSocket protocol schema 
![](https://cdn.educba.com/academy/wp-content/uploads/2018/11/WebSocket-protocol-schema.png)
#### Why do we need WebSocket?
+ It provides full-duplex communication, which helps in persisting the connection established between the Client and the Web Server.
+ It also lives up to the standards and provides the accuracy and efficiency stream events to and from with negligible latency.
+ WebSocket removes the overhead and reduce complexity.
+ It makes real-time communication effortless and efficient.








[Github view](https://github.com/sbkhaloof/growthmindsit)
