## Socket.io

1 - What is the benefit of transforming data into packets?
to transfer the file fast and efficient manner over the network and minimize the transmission latency, the data is broken into small pieces of variable length

2 - UDP is often refereed to as a connectionless protocol. Why is this?
No connection needs to be established between the source and destination before you transmit data. UDP does not have a mechanism to make sure that the payload is not corrupted. As a result, the application must take care of data integrity all by itself.

3 - Can a socket server application have multiple socket connections?
server socket listens on a single port. but Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to

4 - Can a socket connection application be connected to multiple socket servers?
it is possible to run out of available ports if you make a lot of connections in a short amount of time.

since clients are different, multiple clients can connect to the same server socket

5 - Can an application be both a socket server and a socket connection?
if you want to use a client socket and a server socket within a single application, then yes! You can do that if you're willing to use two different ports. Or if the sockets won't be using the same port at the same time.

## Vocabulary Terms

| Word                     | Definition                                                                                                                                                                                                                                 |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Observer Pattern         | is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods                    |
| Listener                 | is a procedure in JS that waits for an event to occur                                                                                                                                                                                      |
| Event Handler            | a function that runs when a specific event occurs.                                                                                                                                                                                         |
| Event Driven Programming | is when a program is designed to respond to user engagement in various forms.                                                                                                                                                              |
| Event Loop               | is a programming construct or design pattern that waits for and dispatches events or messages in a program. The event loop works by making a request to some internal or external "event provider", then calls the relevant event handler. |
| Event Queue              | is a repository where events from an application are held prior to being processed by a receiving program or system                                                                                                                        |
| Call Stack               | is a stack data structure that stores information about the active subroutines of a computer program.                                                                                                                                      |
| Emit/Raise/Trigger       | in event-driven programming, emit sends a message to trigger a response and raise an event                                                                                                                                                 |
| Subscribe                | subscribe dom events in browser or node.js events.                                                                                                                                                                                         |
| database                 | is a data structure that stores organized information                                                                                                                                                                                      |

## Preperation

- WebSocket :is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

### Socket.io vs Web Sockets

|                        **Web-Sockets**                         |                                 **Socket.io**                                  |
| :------------------------------------------------------------: | :----------------------------------------------------------------------------: |
| It is the protocol that is established over the TCP connection |                    It is the library to work with WebSocket                    |
|    It provides full-duplex communication on TCP connections    |       Provides the event-based communication between browser and server        |
|     Proxy and load balancer is not supported in WebSocket.     | A connection can be established in the presence of proxies and load balancers. |
|                It doesn’t support broadcasting                 |                           It supports broadcasting..                           |
|               It doesn’t have a fallback option.               |                         It supports fallback options.                          |
