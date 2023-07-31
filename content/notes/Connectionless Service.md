---
title: "Connectionless Service"
---

# Connectionless Service

A connectionless service is modeled after the postal service. Messages have a **sender** and a **destination**. The message is then passed down from node to node until the destination receives it. Good examples of connectionless services are:

- **Domain Name System (DNS)**: DNS is a fundamental service that translates human-readable domain names (e.g., [www.example.com](http://www.example.com/)) into IP addresses. DNS uses connectionless protocols like User Datagram Protocol (UDP) to quickly respond to queries without establishing a connection.
- **Voice over IP (VoIP) - Signaling**: While VoIP for actual voice transmission prefers a connection-oriented approach for better quality, the signaling part of VoIP (e.g., SIP - Session Initiation Protocol) often uses connectionless UDP for faster call setup and teardown.
- **IoT (Internet of Things) Devices**: Many IoT devices use connectionless networks to efficiently exchange data with central servers or cloud services without the need for maintaining a continuous connection.

![connectionless_service](notes/images/connectionless_service_example.png)