# DEFINITION
In this architecture, the system is built around handling and responding to [[Event|events]]. Instead of executing a predefined sequence of steps, the system listens for [[Event|events]] and reacts accordingly. Events propagate in the system through the [[Pub-Sub Pattern]]

---
## WHEN TO USE?
- The project constantly needs to swap services.
- The project needs [[Asynchronous Communication]] between services.
- Performance and scalability are key factors to the project.

---
## WHEN NOT TO USE?
- The project has a simple and linear workflow.
- Single service applications -> don't spread services if it does not make sense.
- Lack of Event-Driven infrastructure such as a Messaging service like [[RabbitMQ]]

---
## TOPOLOGIES
The event-driven architecture has two very distinct topologies, we must study them separately:
[[Mediator Topology]] => topology for requests that have many steps to complete its job.
[[Broker Topology]] => fewer steps to complete its job.

---
## EXAMPLE IMAGE
![[Event-driven architecture Image.png]]

---
## PATTERN ANALYSIS
[[Architecture Patterns Analysis]]

---
## REVIEWS
#⭐⭐⭐