# DEFINITION
The broker topology differs from the mediator topology in that there is no central [[Event Mediator]]; rather, the message flow is distributed across the [[Event Processors]] components in a chain-like fashion through a lightweight [[Message Broker]].

---
## EXAMPLE BY OREILLY
[[Relay Race Example]]

---
## CONSIDERATIONS
The [[Event-driven Architecture]] pattern is a relatively complex pattern to implement, primarily due to its asynchronous distributed nature. When implementing this pattern, you must address various distributed architecture issues, such as [[remote process availability]], lack of responsiveness, and [[Message Broker]] reconnection logic in the event of a broker or [[Mediator]] failure.

---
### EXAMPLE IMAGE
![[Broker topology Image.png]]

---
### EXAMPLE IMAGE
This is how a chain of event processors is executed:
![[Event processor Image.png]]

---
## REVIEWS
#⭐