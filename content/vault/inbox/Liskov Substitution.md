# DEFINITION
The **child** Class should be able to process the same requests and deliver the same result as the **parent** Class or it could deliver a result that is of the same type.

The picture shows that the **parent** Class delivers Coffee(it could be any type of coffee). It is acceptable for the **child** Class to deliver Cappucino because it is a specific type of Coffee, but it is NOT acceptable to deliver Water.

If the **child** Class doesn’t meet these requirements, it means the **child** Class is changed completely and violates this principle.

---
## GOAL
This principle aims to enforce consistency so that the parent Class or its child Class can be used in the same way without any errors.

---
## EXAMPLE IMAGE
![[Liskov Substitution Image.png]]

---
## REVIEWS
#⌛