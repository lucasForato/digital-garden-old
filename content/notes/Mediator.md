---
title: "Mediator"
---

# DEFINITION

The event mediator receives the initial event and **orchestrates** that event by sending additional asynchronous events to [[Event Channels]] to execute each step of the process.

The event mediator is a **core component** of the event driven architecture, it should be designed correctly for a good use of the [[Event-driven Architecture]]

The event mediator can be implemented in **many different ways** including the [[Spring Integration]]

The event mediator is middle man of a request:

[[Initial Event]] => the event before the mediator.

[[Processing Event]] => an event that is being processed by [[Event Processors]]

#work-in-progress
