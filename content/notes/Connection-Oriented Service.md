---
title: "Connection-Oriented Service"
---

# Connection-Oriented Service

A connection oriented service works like a telephone service, they **establish** a connection, **use** the connection, and **end** the connection. Connection-oriented networks are generally used in scenarios where data integrity and reliability are critical for the application, such as:

- **Online Gaming**: Many online multiplayer games utilize connection-oriented networks to maintain a reliable and low-latency connection between players, reducing lag and ensuring a smoother gaming experience.
- **Video Streaming Services**: Connection-oriented networks are essential for video streaming platforms like Netflix and YouTube to deliver high-quality video content without buffering or interruptions.
- **Email Services**: SMTP (Simple Mail Transfer Protocol) is commonly used for sending emails. SMTP establishes a connection between the mail client and the mail server to ensure that emails are reliably delivered and received.
- **Voice over IP:** Voice over IP uses connection-oriented networks because the conversation must follow the flow, a receiver must not wait for a response and maybe never get it, reliability is extremely important for this use case.

## Primitives (operations)

The connection-oriented service is specified by a set of primitives (operations) that are performed during a connection. Let's illustrate this interaction:

- **LISTEN**: The server executes this operation to establish that it is ready to receive connections.
- **CONNECT:** A client sends a packet to the server and waits for it to respond, this packet tells the server that the machine is trying to establish a connection.
- **ACCEPT**: The server accepts the connection.
- **RECEIVE:** The server performs this operation to be ready to receive messages by the client.
- **SEND:** The client sends a message and waits for a response using RECEIVE.
- **DISCONNECT:** The client terminates the connection after the communication.

![connection_oriented_primitives](connection_oriented_primitives.png)


