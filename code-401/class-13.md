# Reading Notes 13: Message Queues

This topic is important because it goes over Socket.IO functionality to be able to add common features to our applications like chats.

## Socket.io Chat Example

Explain to a non-technical recruiter what the Chat Example (above) does.

- In the example, a server is being created that uses Socket.IO (a library for two-way communication between a server and client). It then listens for a socket connection from a client. On the client side, a user can input some text and send it. Once the server gets the message, it logs the message. Then the server relays that message to whoever is listening. When the client(s) who is/are listening receive the message, it displays it on the page. All-in-all, this creates a chat where people can send messages to each other.

What proof of life are we getting on the backend from the above app?

- Logging the socket connection and disconnection.

Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?

- socket.broadcast.emit()

Source: <https://socket.io/get-started/chat/>

## Rooms

What is a room and how might a room be useful?

- "A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients" ~ [socket.io](https://socket.io/docs/v4/rooms). It could be useful for making sure messages/events get sent only to certain clients instead of all of them.

How do you join a room?

- You join a room using socket.join()

```javascript
io.on("connection", (socket) => {
  socket.join("some room");
});
```

how do you leave a room?

- You leave a room using socket.leave() in the same fashion as above.

Source: <https://socket.io/docs/v4/rooms>

## Namespaces

What is a Namespace and what does it allow you to do?

- A namespace allows users to group connections and events in Socket.IO. This way you have have different socket connections that create separate communication channels. Events emitted in one namespace are only received by sockets that are connected to that namespace. It allows you to organize events.

Each namespace potentially has its own what? (hint: 3 things)

- Event handlers, rooms, and middlewares.

Discuss a possible use case for separate namespaces

- A possible use case for seperate namespaces is having one namespace for a chat and another for sending/receiving real-time notifications. Another use case is if you want to create a namespace that only authorized users have access to.

Sources: <https://socket.io/docs/v4/namespaces/> and ChapGPT

## Reflection

My learning goal is to be able to implement a message queue using Socket.IO.
