# Reading Notes 12: Socket.io

This topic is important to create custom events that add extra functionality to our web pages like sending notifications or having a chat feature.

## Web Sockets

What is a Web Socket?

- "WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request." ~ <https://www.educba.com/websocket-vs-socket-io/>

Describe the Web Socket request/response handshake and what happens once the connection is established.

- The Web Socket request/response handshake is when the client and the server agree to switch to the Web Socket protocol. The client sends an HTTP GET request with an Upgrade header and then if the server agrees with it, it responds with an HTTP 101 status code (Switching Protocols) along with the "Upgrade" header and the "Connection" header set to "Upgrade". Source: ChatGPT.

Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client.

- a request from the client. Both the client and server can send stuff to each other without either needing a request from the client.

## Socket.io Tutorial

What does the event handler io.on() do?

- It handles the connections and disconnections to Socket.io.

Describe some possible proof of life or proof that the code works as expected

- Setting up the io.on() and socket.on() event listeners and handlers for connections and disconnections and making sure you get an expected message for both in the console.

What does socket.emit() do?

- Creates a custom event.

## Socket.io vs Web Sockets

What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

- WebSocket is the communication protocol and Socket.IO is a library that uses WebSocket.

When would you use Socket.IO?

- You would use Socket.IO when you want to use the WebSocket protocol and create events between a client and a server.
- "Socket.IO is ideal for any application that requires real-time, event-driven communication between clients and servers, offering a convenient and efficient way to implement such functionality in web applications." ~ ChatGPT

When would you use WebSockets?

- "WebSockets are used in scenarios where real-time, bidirectional communication is needed between a client and a server." ~ ChatGPT

## OSI Model Explained

What are a couple of key takeaways from this video?

- Better understanding of protocols
- What the different layers of the OSI model are (application, presentation, session, transport, network, data link, physical).
- Different network applications (applications that use the internet) use different protocols.

## TCP Handshakes Explained

Translate the gist of this video to a non-technical friend

- The video explains what TCP is. It stands for transmission control protocol. A client requests to the server for a connection. The server accepts the request and then asks the client to open a connection too. The client accepts. Now there's a two-way connection established between them.

## Reflection

My learning goal is to be able to utilize and understand Socket.IO in a project.

## Things I want to know more about
