---
title: "Broker Topology"
---

# DEFINITION

The broker topology differs from the mediator topology in that there is no central [[notes/Mediator|Mediator]]; rather, the message flow is distributed across the [[Event Processors]] components in a chain-like fashion through a lightweight [[Message Broker]].

## CONSIDERATIONS

The [[Event-driven Architecture]] pattern is a relatively complex pattern to implement, primarily due to its asynchronous distributed nature. When implementing this pattern, you must address various distributed architecture issues, such as [[remote process availability]], lack of responsiveness, and [[Message Broker]] reconnection logic in the event of a broker or [[Mediator]] failure.

#work-in-progress
