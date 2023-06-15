---
alias: persistence layer
---
# DEFINITION
The persistence layer is responsible for saving and retrieving data, it sits after the [[Business layer]] and talks to an ORM or directly to a database in order to persist data. By using the persistence layer, we promote <u>decoupling</u> and <u>flexibility</u>, since we can always swap the database and only the persistence layer has to be changed.

---
## REVIEWS
#⭐