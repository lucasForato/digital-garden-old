# DEFINITION
This principle says a Class should not be fused with the tool it uses to execute an action. Rather, it should be fused to the interface that will allow the tool to connect to the Class.

It also says that both the Class and the interface should not know how the tool works. However, the tool needs to meet the specification of the interface.

---
## GOAL
This principle aims at reducing the dependency of a high-level Class on the low-level Class by introducing an interface.

---
## EXAMPLE IMAGE
![[Dependency Inversion Image.png]]

---
## REVIEWS
#⌛