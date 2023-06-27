---
title: "Event Processors"
---
# Definition

The event processor is responsible for executing the logic. The event processor uses modules to execute business logic. The event processors are <u>self-contained, meaning they cannot use other event processors to execute their logic.</u>

## How granular can they be?

Event processors need to be able to execute their task without depending on other event processors. If they can be split without creating dependency between the services, they should be split.

#work-in-progress 