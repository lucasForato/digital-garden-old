---
title: "Microservices Architecture"
---

> **Font:** Software Architecture Patterns - Mark Richards

# Definition

This pattern consists of separated units of deployment that are each responsible for one service of the application. The microservices pattern allows businesses to use different languages, frameworks, and architectures for each service, providing more efficiency for the specific needs of each feature. 

## Service Components

The most important concept of a microservices pattern is the notion of *service components* that each perform a defined action across the application. Let's imagine an example below:

You have an E-learning platform that serves content to users based on their needs. The content is curated for each user and is sent via e-mail and other notification systems. This system might have the services below:

- **CMS Service:** This service will be responsible for holding the content that will be shared with users.
- **Recommender Service:** The recommender will be responsible for uniting the *CMS Service* with user needs, providing algorithms for choosing content based on the user profile.
- **Notifications Service:** This service will send notifications to users on a regular basis with content that they should study.

Each service from the list above might use a different language that better fits their needs, like python for recommendation, Java for CMS, and Go for Notifications. The services also use different architectures on their own, providing flexibility for developers to use the best fit for each service.

## Pattern Topologies

There are dozens of ways to implement a *microservices architecture*, but there are *three ways* that are mostly used by companies:

### API-REST based topology

The API-REST-based topology is a way of building websites where each small piece of the website does its own thing, like separate little workers. They have a special way of talking to each other through APIs. These workers are really good at just one or two tasks, and they don't need to know much about the other workers. This helps the website work smoothly and efficiently.

![api_rest_based_topology.png](api_rest_based_topology.png)

### Application REST based topology

In the REST-based application topology, things work a bit differently compared to the *API REST-based* approach. Instead of using a simple API layer, requests from users come through regular web screens.

In this setup, the business functionalities are a bit bigger and handle more things at once. This kind of setup is common for simple applications, like smaller or medium-sized businesses.

![rest_based_application](rest_based_application.png)

### Centralized Messaging topology

In microservices architecture, another common setup is the centralized messaging approach. This is like the previous REST-based setup, but instead of using REST for remote connections, it relies on a lightweight message broker, like [[RabbitMQ]].

This setup is often used in bigger apps or when you need more control over how things travel between the user interface and the services. The benefits include *advanced queuing*, *asynchronous messaging*, and better handling of errors and balance.

![centralized_messaging_topology](centralized_messaging_topology.png)


## Disadvantages

In a microservices architecture, developers need to worry about two major problems that might arise due to the distributed nature of this pattern, they are:

### Network

In the microservices architecture, network issues might arise, for microservices are distributed and communicate over the internet using protocols such as HTTP. Since the internet is not completely reliable, things might go wrong and developers need to worry about these problems. Pub-Sub and Messaging queues are a good choice for solving those problems and ensuring that users get error-free features.

### Granularity

Developers also need to worry about the granularity of services. If a service is too granular, it might need to communicate with other services for pretty much everything, leading to *dependency between services*, which is something to be avoided in this architecture pattern.
## Conclusion

The microservices architecture pattern is a good choice for scaling services with bigger teams and bigger demands, but it is not always the best choice for every company and scenario. It is important for engineers know the drawbacks of choosing this pattern and operate against these drawbacks. 