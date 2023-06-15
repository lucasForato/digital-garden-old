# DEFINITION
An event channel acts as a central hub or intermediary, where components can publish events and subscribe to events of interest. When a component publishes an event to the event channel, it becomes available for consumption by other interested components that have subscribed to that particular event. the component that publishes the event is called [[Event Mediator]], the components that are subscribed are called [[Event Processors]].

---
## HOW THEY WORK
The event channel operates based on a [[Pub-Sub Pattern|publish-subscribe mechanism]]. Components can publish [[Event|events]] to the channel without needing to know which specific components will receive them. Similarly, components interested in specific types of events can subscribe to the channel without needing to know which components will publish those events.

---
## KEY CONCEPTS
**Decoupling** -> Event channels decouple the sender of an event from its receivers. Components only need to be aware of the event channel and the events they are interested in, rather than having direct knowledge of other components.

**Flexibility** -> The use of event channels allows components to dynamically join or leave the communication network without impacting the overall system. Components can subscribe to new event types or unsubscribe from existing ones based on their changing requirements.

**Scalability** -> Event channels can handle a large number of events and distribute them efficiently to the subscribed components. This scalability ensures that as the system grows, the communication infrastructure can handle the increased event traffic.

---
### EXAMPLE IMAGE:
![[Request Example Image.png]]

---
## REVIEWS
#⭐  