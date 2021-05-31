# Socket.io
## WebSocket
**WebSocket** is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.

## Difference Between WebSocket and Socket.io
**WebSocket** is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

**Socket.IO** is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.

### **Key features of WebSocket** 

* WebSocket helps in real-time communication between the Client and the webserver.
* This protocol helps in transforming to cross-platform in a real-time world between the server and the client.
* This also enables the business worldwide for a real-time web application to enhance and increase the feasibility.
* The major advantage it stands over an HTTP connection that it provides full-duplex communication.

### **Key features of Socket.IO**
* It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
* It works on all platform, server or device, ensuring equality, reliability, and speed.
* It automatically upgrades the requirement to WebSocket if needed.
* It is a custom real-time transport protocol implementation on top of other protocols.
* It requires both libraries to be used Client side as well as a server-side library.
* IO works on work-based events. there are some reserved events that can be accessed using the Socket on the server side like Connect, message, Disconnect, Ping and Reconnect.
* There are some Client based reserved events like Connect, connect- error, connect-timeout and Reconnect etc.

# Term
* The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.
* Event handlers, scripts that are automatically executed when an event occurs. Event handlers are embedded in documents as attributes of HTML tags to which you assign JavaScript code to execute.
*  The event could be the DOM is loaded, or an asynchronous request that finishes fetching, or a user clicking an element or scrolling the page, or the user types on the keyboard.
* The event loop is the secret behind JavaScript's asynchronous programming. JS executes all operations on a single thread, but using a few smart data structures, it gives us the illusion of multi-threading. ... The event queue is responsible for sending new functions to the track for processing.
* An event queue is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system.
* A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.
* The subscriber function defines how to obtain or generate values or messages to be published. To execute the observable you have created and begin receiving notifications, you call its subscribe() method, passing an observer. This is a JavaScript object that defines the handlers for the notifications you receive.



## 

### What is the benefit of transforming data into packets?
Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully.

### UDP is often referred to as a connectionless protocol. Why is this?

UDP is a connectionless protocol. It is known as a datagram protocol because it is analogous to sending a letter where you don't acknowledge receipt. Examples of applications that use connectionless transport services are broadcasting and tftp .

### Can a socket server application have multiple socket connections?

 Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.