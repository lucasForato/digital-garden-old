# DEFINITION
The event queue is the beginning of every request. The queue works in a [[Pub-Sub Pattern|publish-subscribe mechanism]] where an event is published and has to wait until the [[Event Mediator]] can handle the request.

---
## FLOW
Transports the event to the Event Queue. it then transports the request to the [[Event Mediator]] when it is ready to handle the request.

---
## EXAMPLE IMAGE
![[Request Example Image.png]]

---
## REVIEWS
#⭐