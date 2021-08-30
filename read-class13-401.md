# Message Queues
## Review, Research, and Discussion
+ What does it mean that web sockets are bidirectional? Why is this useful?
### it mean you can transfer  the data from client to sever and from server to client  so they allow real-time data transfer.
+ Does socket.io use HTTP? Why?
### Yes it’s use it but it doesn’t need an HTTP server to regular websockets,but it is used to allow HTTP and websocket servers to co-exist on the same TCP port.
+ What happens when a client emits an event?
### The event gets passed to the server through websockets. Its a tcp connection from the client to the server. The connection meaning the server can send real time data to the client and vise versa.
+ What happens when a server emits an event?
### will run the event in the client that was listinig for this event.
+ What happens if a client “misses” an event?
### The events will be ignored
+ How can we mitigate this?
### using queues
## Document the following Vocabulary Terms
- Socket:is a software structure within a network node of a computer network that serves as an endpoint for sending and receiving data across the network.
- Web Socket: The WebSocket API is an advanced technology that makes it possible to open a two-way interactive communication session between the user's browser and a server. With this API, you can send messages to a server and receive event-driven responses without having to poll the server for a reply.
- Socket.io :is a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of:a Node.js server and Javascript client library for the browser (which can be also run from Node.js
- Client: is a computer or a program that, as part of its operation, relies on sending a request to another program or a computer hardware or software that accesses a service made available by a server 
- Server:is a piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients".
- OSI Model:  (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. 
- TCP Model:TCP model defines how devices should transmit data between them and enables communication over networks and large distances. The model represents how data is exchanged and organized over networks.
- TCP: stands for Transmission Control Protocol a communications standard that enables application programs and computing devices to exchange messages over a network.
![](https://www.researchgate.net/publication/327483011/figure/fig2/AS:668030367436802@1536282259885/The-logical-mapping-between-OSI-basic-reference-model-and-the-TCP-IP-stack.jpg)
- UDP: UDP (User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet. It speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party. As a result, UDP is beneficial in time-sensitive communications,
- Packets : is a small segment of a larger message. Data sent over computer networks*, such as the Internet, is divided into packets. These packets are then recombined by the computer or device that receives them.
## Preparation Materials
![](data:image/png;base64,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)



### Rooms and Namespaces
#### Rooms :is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients:
![](https://socket.io/images/rooms.png)
##### Please note that rooms are a server-only concept ( the client does not have access to the list of rooms it has joined).
### With multiple Socket.IO servers Like global broadcasting, broadcasting to rooms also works with multiple Socket.IO servers.You just need to replace the default Adapter by the Redis Adapter.
![](https://socket.io/images/rooms-redis.png)
### Room events : Starting with socket.io@3.1.0, the underlying Adapter will emit the following events:

- create-room (argument: room)
- delete-room (argument: room)
- join-room (argument: room, id)
- leave-room (argument: room, id)


















[Github view](https://github.com/sbkhaloof/growthmindsit)
