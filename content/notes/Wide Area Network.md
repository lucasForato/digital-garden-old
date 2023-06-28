---
title: "Wide Area Network"
---
# Definition
**WANs** consist of networks that span across a country.

## Hosts

Hosts are computers that are connected to the subnet and need to communicate with each other or run applications. 

## Subnet

Can be simply perceived as a collection of lines and routers that connect computers.

The WAN as we have described it looks similar to a large wired LAN. There are some differences, the most important of them being that LANs are a bunch of computers connected to each other, in WANs, you might have computers connected to each other or even LANs connected to each other.

The job of the subnet is carrying messages from host to host. The subnet consists of two distinct components:

[[Transmission Lines]]

[[Routers]]

WANs can be connected to each other through a cable, like the image below:

![[notes/images/wide_area_network.png]]

Or they can be connected through the internet and a [[VPN]], as shown in the image below:

![[notes/images/wide_area_network_internet.png]]

If two routers that are not directly connected to each other wish to communicate, they have to do it indirectly through other routers, creating a path of communication that is the shortest and most effective. The path is determined by a **routing algorithm**.


#work-in-progress 