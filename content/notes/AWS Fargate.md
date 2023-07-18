---
title: "AWS Fargate"
---

# Definition

Fargate is a service offered by AWS that is responsible for managing infrastructure for the user. When you launch an [[notes/Elastic Compute Cloud (EC2)|Elastic Compute Cloud (EC2)]] instance, you also have to deal with security, patching and many other problems that you might not want to deal with. Fargate will be responsible for managing the infrastructure for you so you don't have to worry about any of those problems.

## When to use Fargate?

Companies should use AWS Fargate when the machine which is hosting the application does not rely on specific configurations. Fargate excels at delivering power with simplicity, but sometimes companies need to have more freedom of configuration.