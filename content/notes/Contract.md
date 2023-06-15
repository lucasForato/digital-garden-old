# DEFINITION

A group of rules that are usually used by the API.

---

## EXAMPLE

There are some contracts being established below. Contracts represent the way the API will transfer data. What you have to send and what you get from it.

```graphql
type User {
  email: String
  name: String
}

type Query {
  user(id: String!): User
}
```

---
## REVIEWS
#⭐ 