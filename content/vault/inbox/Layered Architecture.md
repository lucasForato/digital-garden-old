---
alias: layered architecture
---
# DEFINITION
This pattern is the de facto standard for most Java EE applications and therefore is widely known by most architects, designers, and developers.

A layered architecture has <u>many horizontal layers</u> that each take care of <u>one specific task</u>, this makes it possible to isolate changes to specific components.

---
## LAYERS
[[Transport Layer]] -> responsible for interacting with the user, listening for requests and delivering responses.
[[Presentation layer]] -> responsible for displaying the result and processing user requests.
[[Business layer]] -> entities, use cases.
[[Persistence layer]] -> responsible for talking to the database layer.

---
## OPEN LAYERS
An open layer is a layer that is open to be accessed by any layer, requests can bypass this layer since it is open. There should be some to no open layers in an application, only layers like service workers that have the task to help the entire application. In [[NestJS]], we call these layers [[Global Modules]].

---
## WHEN TO USE?
You should use a layered architecture as a <u>good solid starting point for an application</u>, mostly when you don't have an architecture to follow yet. But it usually leads to a monolithic application and can have issues with performance.

---
## PATTERN ANALYSIS
[[Architecture Patterns Analysis]]

---
## REVIEWS
#⭐⭐⭐⭐⭐