---
title: "Event-driven Architecture"
---
# Definition

In this architecture, the system is built around handling and responding to [[Event|events]]. Instead of executing a predefined sequence of steps, the system listens for [[Event|events]] and reacts accordingly. Events propagate in the system through the [[Pub-Sub Pattern]]

## When to use?

- The project constantly needs to swap services.
- The project needs Asynchronous Communication between services.
- Performance and scalability are key factors to the project.

## When not to use?

- The project has a simple and linear workflow.
- Single service applications -> don't spread services if it does not make sense.
- Lack of Event-Driven infrastructure such as a Messaging service like [[RabbitMQ]]

## Topologies

The event-driven architecture has two very distinct topologies, we must study them separately:

[[Mediator Topology]] => topology for requests that have many steps to complete its job.

[[Broker Topology]] => fewer steps to complete its job.

#work-in-progress 