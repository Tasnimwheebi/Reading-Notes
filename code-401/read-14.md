# Event Driven Architecture
## Review, Research, and Discussion

### **What’s the difference between a FIFO and a standard queue?**

**Standard queues** guarantee that a message is delivered at least once and duplicates can be introduced into the queue. 

**FIFO queues** ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.

### **How can the server be assured a message was properly received?**

The client (usually a browser) opens a connection to the server and sends a request. The server processes the request, generates a response, and closes the connection if it finds a Connection: Close header.

### **What classic design pattern is best represented by event driven programming?**

In software engineering, a design pattern is a general repeatable solution to a commonly occurring problem in software design. A design pattern isn't a finished design that can be transformed directly into code. It is a description or template for how to solve a problem that can be used in many different situations.

### **How do you test an event driven system?**
Basically, an event-driven application architecture is one in which services (aka functions) within an application input data and output data via messages that are stored in a message queue. This differs from a synchronous architecture, in which data is passed straight to a service by making a direct call.

# **Term**

* **FIFO Queue**
A FIFO queue is a queue that operates on a first-in, first-out (FIFO) principle. This means that the request (like a customer in a store or a print job sent to a printer) is processed in the order in which it arrives. A first-come, first-served line is the most common type of queue that we join in our everyday lives and is generally accepted as the fairest way to operate a queue.

* **Pub/Sub**

Pub/sub is shorthand for publish/subscribe messaging, an asynchronous communication method in which messages are exchanged between applications without knowing the identity of the sender or recipient.