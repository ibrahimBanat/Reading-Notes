# Message Queues

## Review, Research, and Discussion

1 - What does it mean that web sockets are bidirectional? Why is this useful?

    - Because its enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time

2. Does socket.io use HTTP? Why?

   - a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js

3. What happens when a client emits an event?
   - Event will be sent to the server, and start listening for the event when it's connected
4. What happens when a server emits an event?
   - When its listening to the server , so then it will response
5. What happens if a client “misses” an event?
   - Unhandled messages are ignored
6. How can we mitigate this?
   - by always having handlers installed and decalcify what to do whit this message

## Vocabulary Terms

|            |                                                                                                                                                                                                                |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Socket     | is one endpoint of a two-way communication link between two programs running on the network                                                                                                                    |
| Web Socket | is a computer communications protocol, providing full-duplex communication channels over a single TCP connection                                                                                               |
| Socket.io  | is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers.                                                                      |
| Client     | program separate from the server that initiates requests for services or info from the server                                                                                                                  |
| Server     | provides function, info, or service back to the client, acts as the main hub for communication                                                                                                                 |
| OSI Model  | is a conceptual framework used to describe the functions of a networking system                                                                                                                                |
| TCP Model  | is the conceptual model and set of communications protocols used in the Internet and similar computer networks.                                                                                                |
| TCP        | is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data                                                                           |
| UDP        | is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet.                                                         |
| Packets    | is a small amount of data sent over a network, such as a LAN or the Internet. Similar to a real-life package, each packet includes a source and destination as well as the content (or data) being transferred |

## Preview

socket emmiting cheat sheet

```
io.on("connection", (socket) => {

  // basic emit
  socket.emit(/* ... */);

  // to all clients in the current namespace except the sender
  socket.broadcast.emit(/* ... */);

  // to all clients in room1 except the sender
  socket.to("room1").emit(/* ... */);

  // to all clients in room1 and/or room2 except the sender
  socket.to("room1").to("room2").emit(/* ... */);

  // to all clients in room1
  io.in("room1").emit(/* ... */);

  // to all clients in namespace "myNamespace"
  io.of("myNamespace").emit(/* ... */);

  // to all clients in room1 in namespace "myNamespace"
  io.of("myNamespace").to("room1").emit(/* ... */);

  // to individual socketid (private message)
  io.to(socketId).emit(/* ... */);

  // to all clients on this node (when using multiple nodes)
  io.local.emit(/* ... */);

  // to all connected clients
  io.emit(/* ... */);

  // WARNING: `socket.to(socket.id).emit()` will NOT work, as it will send to everyone in the room
  // named `socket.id` but the sender. Please use the classic `socket.emit()` instead.

  // with acknowledgement
  socket.emit("question", (answer) => {
    // ...
  });

  // without compression
  socket.compress(false).emit(/* ... */);

  // a message that might be dropped if the low-level transport is not writable
  socket.volatile.emit(/* ... */);

});
```

- Client-side

```
// basic emit
socket.emit(/* ... */);

// with acknowledgement
socket.emit("question", (answer) => {
 // ...
});

// without compression
socket.compress(false).emit(/* ... */);

// a message that might be dropped if the low-level transport is not writable
socket.volatile.emit(/* ... */);
```

- Reserved events

- `connect`
- `connect_error`
- `disconnect`
- `disconnecting`
- `newListener`
- `removeListener`

```
// BAD, will throw an error
socket.emit("disconnecting");
```
