---
title: "Elastic Container Service (ECS)"
---

# Definition

Amazon Elastic Container Service, as the name implies, is a service offered by amazon to orchestrate containers, usually [[Docker]] containers. ECS sits on top of [[notes/Elastic Compute Cloud (EC2)|Elastic Compute Cloud (EC2)]] or [[AWS Fargate]] as the machines in which containers are going to run. 

## How does it work?

First of all, we need a dockerfile from which the application will be built. The dockerfile will be responsible for starting up the application.

After the dockerfile is created, we have to deploy it to [[Elastic Container Repository (ECR)]] which is a registry owned by Amazon to hold images.

Then, you can define a <u>task</u> using ECS. A task definition is an abstraction that is responsible for starting containers and dealing with ports for communication between containers. For instance, you might have a task that is responsible for two containers, a database container and an NodeJS application container.


## What is a cluster?

A cluster is a group of machines that will be used to execute tasks. You can use both [[notes/Elastic Compute Cloud (EC2)|Elastic Compute Cloud (EC2)]] or [[notes/AWS Fargate|AWS Fargate]] as machines. When tasks are executed, they are hosted on machines inside a cluster of choice.

