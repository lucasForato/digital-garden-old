---
title: "Layered Architecture"
---

# Layered Architecture

Layered Architectures are widely used in software development in many fields, such as: networking, database systems, operating systems, web development, and many more. It is highly popular for its simplicity yet effectiveness for solving problems.

![layered_architecture](notes/images/layered_architecture.png)

When a request is being processed, it acts as a needle, piercing through the layers until it reaches the bottom one, then coming back with a response.

We are going to continue talking about layered architectures in the context of a backend applications since they are widely used there.

## Interface Layer

The interface layer is responsible for receiving requests an returning responses to the client. The interface layer normally follows some type of protocol, such as [[GraphQL]], [[REST]], [[gRPC]], or any other. 

## Domain Layer

It is also called "business logic layer" and it is responsible for applying business logic to the request through modules and [[Use Cases]].  The domain layer is also responsible for: verifying the data sent by the request, dealing with errors, talking to the persistence layer, and managing state.

## Persistence Layer

The persistence layer is responsible for communicating with the database layer. The persistence layer forms an API of operations that the domain layer can use to communicate with the database. The advantage of having a persistence layer is that the database layer is free to be swapped whenever the system requires and it also brings security to the database layer.

## Database Layer

The only responsibility of this layer is storing data, it does not apply business logic or deals with state.

## Helper Layer

This layer serves every other layer and offers some functionality, such as math functions, array manipulation, and other basic features that do not represent any other layer.

## Infrastructure Layer

This layer also servers other layers and it responsible for offering fundamental functionality to the application, such as HTTP clients, dealing with environment variables, dealing with middlewares and configuration of external services.

## When to use and not to use

Layered architectures are the most widely spread architecture pattern in software development, they are very good for projects that are starting and do not have a clear perspective of which architecture pattern that they are going to use.

The downside with layered architectures is that they are usually slow in terms of processing requests, so an application that needs to be super fast might not use them. The image below shows some other aspects of layered architectures compared to other architecture patterns.

![pattern_analysis](notes/images/pattern_analysis.png)
