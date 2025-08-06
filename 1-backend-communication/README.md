# Backend Communication Design Patterns, Protocols, Execution, and Proxying

This chapter covers fundamental backend communication concepts that every developer should understand when building distributed systems and APIs.

## Topics Covered

### [Request/Response](./request-response.txt)
The most basic communication pattern where a client sends a request to a server and waits for a response. This synchronous pattern forms the foundation of HTTP and most API interactions.

### [Synchronous vs Asynchronous](./synchronous-asynchronous.txt)
Understanding the difference between blocking (synchronous) and non-blocking (asynchronous) operations, and how they impact application performance and scalability.

### [Push](./push.txt)
A communication pattern where the server initiates data transmission to clients without the client explicitly requesting it. Common in real-time applications and notifications.

### [Polling](./polling.txt)
A technique where clients repeatedly request data from a server at regular intervals to check for updates. Simple but can be inefficient for real-time data.

### [Long Polling](./long-polling.txt)
An improved polling technique where the server holds the client's request open until new data is available or a timeout occurs, reducing unnecessary requests.

### [Server Sent Events](./server-sent-events.txt)
A web standard that allows a server to push data to a client over a single HTTP connection, enabling real-time updates in web applications.

### [Publish/Subscribe](./publish-subscribe.txt)
A messaging pattern where publishers send messages to topics/channels, and subscribers receive messages from those topics, enabling loose coupling between components.

### [Multiplexing vs Demultiplexing](./multiplexing-vs-demultiplexing.txt)
Techniques for efficiently handling multiple connections and requests, including HTTP/2 multiplexing and connection pooling strategies for improved performance.

### [Stateful vs Stateless](./stateful-vs-stateless.txt)
Understanding the fundamental difference between services that maintain client state between requests versus those that treat each request independently.

### [Sidecar Pattern](./sidecar-pattern.txt)
A deployment pattern where auxiliary functionality (like logging, monitoring, or proxying) is deployed alongside the main application in a separate container or process.
