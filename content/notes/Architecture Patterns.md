---
title: "Architecture Patterns"
---

> **Font:** Software Architecture Patterns - Mark Richards

# Introduction

Recently, I've dedicated myself to a comprehensive study of architecture patterns, recognizing their importance within the realm of backend software engineering. I embarked on this journey by exploring relevant content on [roadmap.sh](https://roadmap.sh/backend). Then I came across a great book on the topic entitled **"Software Architecture Patterns - Mark Richards"**. I'm here to share some of the key takeaways from my studies. Feel free to explore the links if you wish to dive into other topics.

## Layered Architecture

[[Layered Architecture]]

The first pattern I want to talk about is the **layered architecture** pattern. This pattern is the standard for most Java E.E. applications and therefore is widely known by most architects, designers, and developers.

A layered architecture consists of many **horizontal layers** that each take care of one specific task, this makes it possible to isolate changes to specific components in the architecture.

## Event-driven Architecture

[[Event-driven Architecture]]

In this architecture, the system is built around handling and responding to [[Event|events]]. Instead of executing a predefined sequence of steps, the system listens for [[Event|events]] and reacts accordingly. Events propagate in the system through the [[Pub-Sub Pattern]]

## Microkernel Architecture

[[Microkernal Architecture]]

The microkernel architecture pattern is a good choice for products that are meant to have plugins by default, such as operating systems, third-party products, and others. This pattern allows products to have extensions and plug them in easily to the main application.

## Microservices Architecture

[[Microservices Architecture]]

This pattern consists of separated units of deployment that are each responsible for one service of the application. The microservices pattern allows businesses to use different languages, frameworks, and architectures for each service, providing more efficiency for the specific needs of each feature. 

## Space-based Architecture

[[Space-based Architecture]]

The space-based pattern (also called cloud architecture) is all about making applications really good at handling lots of work without slowing down. Instead of relying on one central database, it uses copies of data stored in memory across many computers. This makes it super fast and can handle a huge amount of work.
## Conclusion

There is no architecture pattern that serves all business purposes. Each pattern will be better for certain scenarios and the job of a software engineer is measuring their efficiency for their business needs. The image below shows a comparison between the patterns presented, exposing their pros and cons in an illustrative way.  

![pattern_analysis](notes/images/pattern_analysis.png)
