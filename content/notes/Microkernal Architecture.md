---
title: "Microkernal Architecture"
---

> **Font:** Software Architecture Patterns - Mark Richards

# Introduction

The Microkernel architecture pattern consists of two main components, the _core system_ and the _plugins_. The _core system_ is responsible for providing the main functionality of the application, whereas the _plugins_ are responsible for extending the application with new features that are completely isolated from the _core system_ as illustrated in the following image.

![microkernel_architecture](microkernel_architecture.png)

## The VSCode Code Editor

A good example of an application that uses this pattern is the **VSCode Code Editor**. Once you download it, you are presented with the _core functionality_ that every code editor should provide. Once you start adding _plugins_, the editor starts taking another shape that is completely customized for your needs.

## Market Advantages

A good advantage of writing software using the _Microkernel Pattern_ is that you can leverage the creation of _plugins_ to third party companies, only providing them with documentation and frameworks on how to connect with the main application, building an ecosystem of plugins for every type of user.
