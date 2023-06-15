# DEFINITION

The messaging grid manages input request and session information. When a request comes into the [[Virtualized Middleware]] component, the messaging-grid component determines which active [[Processing Unit]] components are available to receive the request and forwards the request to one of those processing units. The complexity of the messaging grid can range from a simple [[round-robin algorithm]] to a more complex [[next-available algorithm]] that keeps track of which request is being processed by which processing unit.

---

## EXAMPLE IMAGE

![[Messaging-grid component.png]]

---
## REVIEWS
#⌛