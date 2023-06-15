---
alias: topic queue
---

# DEFINITION

The topic queue acts as an **intermediary** between publishers and subscribers, ensuring that events are properly delivered to the interested parties.

---

## KEY CONCEPTS

**Event Distribution**: The topic queue serves as a central hub for events of a particular topic. It acts as a [[buffer]] or storage where events are temporarily held until they can be delivered to the subscribers. This allows for decoupling between publishers and subscribers since publishers don't need to know the specific subscribers or how many of them exist.

**Scalability and Load Balancing**: The topic queue can be designed to support multiple instances or partitions to handle high event throughput and distribute the load across different nodes. This enables [[Horizontal Scalability]], ensuring efficient handling of events even in large-scale systems with a high volume of publishers and subscribers.

**Guaranteed Delivery**: The topic queue can provide reliability and durability by persisting events even if subscribers are temporarily offline or unable to process events. This guarantees that events won't be lost and can be delivered to subscribers when they come back online.

**Filtering and Routing**: Topic queues often provide filtering capabilities, allowing subscribers to specify criteria for the types of events they are interested in. Subscribers can subscribe to specific topics or apply filters based on event attributes, ensuring they only receive relevant events.

---

## EXAMPLE IMAGE

![[Pub-sub pattern image.png]]

---
## REVIEWS
#⌛