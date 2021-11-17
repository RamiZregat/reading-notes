# Event Driven Architecture


### - What’s the difference between a FIFO and a standard queue?   
Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.  

### - How can the server be assured a message was properly received?  
Through  `socket.io`’s acknowledgements.  

### - What classic design pattern is best represented by event driven programming?  
Event-driven from end to end.  

### - How do you test an event driven system?  
First we have to understand, what an event-driven application architecture is. Second, allot of logging is required, because the only way to really figure out what’s going on in terms of application behavior is to make sure that all information relevant to application performance is being logged, with timestamping being the no-brainer requirement.  

## Terms  


**FIFO Queue**:  
  > The operations of a queue make it a first-in-first-out (FIFO) data structure. In a FIFO data structure, the first element added to the queue will be the first one to be removed. … A queue is an example of a linear data structure, or more abstractly a sequential collection.  


**Pub/Sub**  
  > an asynchronous messaging service that decouples services that produce events from services.  
## Preparation Materials  


### SNS vs SQS Comparison  


subject | SNS | SQS
---- | ---- | ----  
term | Simple Notification Service | Simple Queue Service  
base | Publisher / Subscriber System | Queueing service for message processing  
how it work | Publishing messages to a topic can deliver to many subscribers of different types(SQS, Lambda, email) | a system must pull the queue to discover new events. Also, messages in the queue are typically processed by a single consumer.  
Events interactions | with other systems | within the system 