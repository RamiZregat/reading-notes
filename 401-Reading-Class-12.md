# Socket.io

## Review, Research, and Discussion  
#### What is the benefit of transforming data into packets?  
To meet the demands of pervasive data-centric applications and services. Packet-based networks not only enable new innovations, services, and business opportunities, they are also the most cost-effective, efficient, and scalable networks for content delivery.  

### UDP is often refereed to as a connectionless protocol. Why is this?  
Because no connection needs to be established between the source and destination before data transmission.  

### Can a socket server application have multiple socket connections?  
 A port of a server can be used by many clients (connections). A port of a client can be used by a single connection. The reason is a port can be used by a single process, which allocates the port (doing "bind" as a server that will listen to that port for incoming connections, or doing a sort of "open" as a client wanting to do outbound connections from that port out). Sometimes the notions of "server socket" and "client socket" are used for these, and in fact the Java ServerSocket creates a connection specific socket for each accepted inbound connection, which will represent a file descriptor on its own. 

### Can a socket connection application be connected to multiple socket servers?  
Yes, as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

### Can an application be both a socket server and a socket connection?  
Yes, if the user is using two different ports. Or if the sockets won't be using the same port at the same time.  



## Term  



Term | Definition
--- | ---
Observer Pattern | The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.  
Listener | waiting on something to happen (a press of a mouse or a link to be pressed) to trigger a course of actions.  
Event | An action that will cause a function to start if it was listened on.  
Event Driven Programming | event-driven programming is when a program is designed to respond to user engagement in various forms. It is known as a programming paradigm in which the flow of program execution is determined by “events.” Events are any user interaction, such as a click or key press, in response to prompt from the system.  
Event Loop | The Event Loop has one simple job — to monitor the Call Stack and the Callback Queue. If the Call Stack is empty, the Event Loop will take the first event from the queue and will push it to the Call Stack, which effectively runs it. Such an iteration is called a tick in the Event Loop.
Event Queue | An event queue is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system
Call Stack | call stack is a stack data structure that stores information about the active subroutines of a computer program
Emit/Raise/Trigger | The trigger() method triggers the specified event and the default behavior of an event (like form submission) for the selected elements. The emit method (the publish method), allows you to "emit" an event, which causes all callbacks registered to the event to 'fire', (get called). Short: Emit's job is to trigger named event(s) which in turn cause functions called listeners to be called. Raise (I think it's related to throwing errors)  
Subscribe | This is a JavaScript object that defines the handlers for the notifications you receive. The subscribe() call returns a Subscription object that has an unsubscribe() method, which you call to stop receiving notifications.
database | A database is a data structure that stores organized information like SQL and noSQL


## Preview  
1. Which 3 things had you heard about previously and now have better clarity on?  
SQL and Role Based Access Control.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
Event Driven Programming 
1. What are you most excited about trying to implement or see how it works?
Events.  


## Preparation Materials  
`Socket.IO` is a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of:  
- a `Node.js` server
- a `Javascript` client library for the browser (which can be also run from Node.js)    

### `Socket.IO` Features:  
- reliability (fallback to HTTP long-polling in case the WebSocket connection cannot be established)
- automatic reconnection
- packet buffering
- acknowledgments
- broadcasting to all clients or to a subset of clients (what we call “Room”)
- multiplexing (what we call “Namespace”)  
### Compatibility
`Socket.IO` is implemented in many languages like:  
- java
- C++
- Swift
- Dart
- Python
- .Net
- Golang
- Rust 