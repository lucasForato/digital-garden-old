# DEFINITION
In a microservices architecture, we deploy separated [[Service Components]] that act as building blocks that together can perform all the actions of the application.

---
## EXAMPLE IMAGE
![[Microservices Architecture Pattern Image.png]]

---
## LINKS TO
a Microservices Architecture was an evolution of the [[Monolithic Application]]

---
## TOPOLOGIES
There are three main ways to develop a microservices architecture.
- [[API REST-based topology]]
- [[Application REST-based topology]]
- [[Centralized Messaging topology]]

---
# CONSIDERATIONS
One of the main challenges of the microservices architecture pattern is determining the correct **level of granularity** for the service components. If service components are too coarse-grained you may not realize the benefits that come with this architecture pattern (deployment, scalability, testability, and loose coupling). However, service components that are too fine-grained will lead to service [[Orchestration|orchestration]] requirements, which will quickly turn your lean microservices architecture into a heavyweight service-oriented architecture, complete with all the complexity, confusion, expense, and fluff typically found with SOA based applications.

It is always a good idea to apply the [[DRY]] principal, but sometimes you can repeat code from one [[Service Components|service component]] in another in order to avoid dependency between [[Service Components|service components]].

You should usually avoid dependency between [[Service Components|service components]] in a request, meaning a request should activate 1 [[Service Components|service component]], no more than that.

---
## PATTERN ANALYSIS
[[Architecture Patterns Analysis]]

---
## REVIEWS
#⭐