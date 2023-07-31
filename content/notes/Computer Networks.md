---
title: "Computer Networks"
---

# Transmission Technologies

There are two types of transmission technologies:

[[Broadcast]]

[[Point-to-point transmission]]

## Scale

Networks can also be classified by their effectiveness by the distance they cover. Different technologies are used at different scales.

### Examples:

[[Personal Area Network]]

[[Local Area Network]]

[[Metropolitan Area Network]]

[[Wide Area Network]]

![networks_by_scale](notes/images/networks_by_scale.png)

## How to connected different types of networks together

The general name for a machine that makes a connection between two or more networks and provides the necessary translation, both in terms of hardware and software, is a **gateway**.

## [[Protocol Hierarchies]]

To reduce their design complexity, most networks are organized as a stack of layers or levels, such as in a [[Layered Architecture]], each one built upon the one below it. The number of layers, the name of each layer, the contents of each layer, and the function of each layer differ from network to network. The purpose of each layer is to offer certain services to the higher layers while shielding those layers from the details of how the offered services are actually implemented. In a sense, each layer is a kind of virtual machine, offering certain services to the layer above it.

## [[Network Software]]

Network software refers to a collection of programs and applications designed to facilitate communication and data exchange between devices within a computer network. It plays a crucial role in performing connections and dealing with the unreliable environment which is the internet through the use of layers of abstraction.

## [[OSI model]]

The **OSI (Open Systems Interconnection)** model is an international conceptual framework that standardizes the functions of computing system into seven distinct layers. Developed by the **International Organization for Standardization (ISO)**, it serves as a guideline to facilitate communication between different hardware and software components within a networked system.