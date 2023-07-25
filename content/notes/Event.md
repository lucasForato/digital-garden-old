---
title: "Event"
---

## Definition

>An event is something that happens, especially when it is unusual or important.

An event can be thought of as something that *has happened and the organisation cares about*. Events represent the past and they are immutable by nature, meaning they cannot be changed once they are created.

## Examples

There are some possible examples of events that might happen:

- An event is sent when a user performs a login.
- An event is sent when a user changes a record in a database.
- An event is sent when a record is deleted from a database.

## Event notification

Event notifications are sent from a system as simple notifications to other systems. The sender does not care about the response that other systems have to that event, the only thing it cares about is sending the notification.

## Event-Carried State Transfer

These types of events carry state and are meant to be processed by other systems without the need of contacting the sender. A good example of this pattern being used is sending an event of a database change so that other systems can also change the same record on their databases.