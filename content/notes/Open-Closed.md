# DEFINITION
Classes should be open for extension but closed for modification.

## GOAL
This principle aims to extend a Class’s behavior without changing the existing behavior of that Class. This is to avoid causing bugs wherever the Class is being used.

---
## EXAMPLE IMAGE
![[Open-Closed Image.png]]

---
## CONSIDERATIONS
This principle reminds me of a [[Plugins|plugin]] because a plugin is simply an <u>extension</u> of a class. A chrome plugin only respects the interfaces that chrome offers, <u>it does not know anything about chrome, and chrome does not know anything about the plugin</u>, but they can connect with each other because the browser is open to extensibility.

---
## REVIEWS
#⌛