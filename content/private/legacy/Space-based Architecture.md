---
aliases: cloud architecture, Cloud Architecture, space-based architecture, space based architecture
---
# DEFINITION
The pattern gets its name from [[tuple space]]. The pattern removes the central database to achieve almost infinite scalability, since the biggest issue when it comes to scalability is scaling the database.

---
## COMPONENTS
There are two main components in this [[private/legacy/Architecture Patterns|architecture pattern]], the [[Processing Unit]] and the [[Virtualized Middleware]]

---
## EXAMPLE IMAGE
![[Space-based architecture pattern image.png]]

---
## CONSIDERATIONS
The space-based architecture pattern is a complex and expensive pattern to implement. It is a good architecture choice for smaller web-based applications with variable load (e.g., social media sites, bidding and auction sites). However, it is not well suited for traditional large-scale relational database applications with large amounts of operational data.

---
## THIRD-PARTY SOFTWARE
From a product implementation perspective, you can implement many of the architecture components in this pattern through third-party products such as [[GemFire]], [[JavaSpaces]], [[GigaSpaces]], [[IBM Object Grid]], [[nCache]], and [[Oracle Coherence]]. Because the implementation of this pattern varies greatly in terms of cost and capabilities (particularly data replication times), as an architect, you should first establish what your specific goals and needs are before making any product selections.

---
## PATTERN ANALYSIS
[[Architecture Patterns Analysis]]

---
## REVIEWS
#⌛