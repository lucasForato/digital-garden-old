---
title: "OSI model"
---

![OSI_model.png](OSI_model.png)

# OSI model

The **OSI (Open Systems Interconnection)** model is an international conceptual framework that standardizes the functions of computing system into seven distinct layers. Developed by the **International Organization for Standardization (ISO)**, it serves as a guideline to facilitate communication between different hardware and software components within a networked system. Let's discuss each layer:

## The Physical Layer

The **physical layer** is responsible for sending bits over wire from one machine to another. This layer is concerned about guaranteeing that every single bit is received the same, without inversion.

## The Data Link Layer

The main responsibility of the **data link layer** is to guarantee that messages are received free of errors, it does that by breaking messages into **data frames** and sending them separately. When a data frame is lost, the **data link layer** is smart enough to send another data frame until the message is completely received by the client.

## The Network Layer

The **network layer** is concerned about routing packets from the origin to the destination. The **network layer** creates the routes and it also deals with connection between different networks that might follow different protocols.

## The Transport Layer

The **transport layer** is responsible for receiving a message from the layers above it and splitting the message into packets. The transport layer also guarantees that end-to-end communication works smoothly in the network.

## The Session Layer

The **session layer** allows users on different machines to establish sessions between them.

## The Presentation Layer

The **presentation layer** looks at the packets and ensures that computers of different types can understand the message being sent. It functions as a sort of translator that helps computers understand each other regardless of their language.

## The Application Layer

The **application layer** holds protocols that will be used by users, such as the [[HTTP]].