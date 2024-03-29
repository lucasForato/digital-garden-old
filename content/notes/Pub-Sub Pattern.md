---
title: "Pub-Sub Pattern"
---

# Definition

This pattern works much like the [[Observer Pattern]], events are **published (pub)** by a service and other services can **subscribe (sub)** to the events that interest them. When an event is created, it is sent to all subscribers and then they perform their actions subsequently.

## What is the topic queue?

In pub-sub systems, a topic represents a specific **category or subject of events**. Publishers generate events and assign them to specific topics, while subscribers express their interest in **receiving events from specific topics**.The [[Topic Queue]] acts as an intermediary between publishers and subscribers.

#work-in-progress
