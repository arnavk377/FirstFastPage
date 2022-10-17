---
toc: true
layout: post
description: Watching videos about Collegeboard Big Idea 4, The Internet.
categories: [markdown, week8, csp, ap]
image: 
title: The Internet, Big Idea 4
---

- Computers went from big to small
- People wanted a way for computers to communicate between different systems
- The computers need to send and receive the data
- Computer system: a group of computers which work together for a joint purpose
- Computer network: a group of interconnected computing devices capable of sending or receiving the data
- Packet switching: the file is broken up into packets and are sent in any order. The packets are reassembled in the correct order.
- Routing: the process of finding a path from sender to receiver
- Path on a computing network: between device sending and receiving information, directly connecting the start(sender) to the end(receiver)
- Bandwith: maximum amount of data which can be sent during a fixed time, measured in bits per second

- Protocol: agreed upon set of rules that specify the behavior of systems
- Internet Engineering Task Force: Manages the development of standards and technical discussions concerning the internet in an open and collaborative process
- Transmission Control Panel(TCP): Establishes a common standard for how to send messages between devices on the internet
- Open Systems Interconnect(OCI): The layers you have to go through to communicate

- Network Access Layer: usually has to do with hardware, how the computers use transport
- Examples include: Datalink, Fiber, Ethernet, Wire, 
- Each card has a MAC address, which is unique to each card. Computers use this to send information

- Internet Data Transmission
- Each packet has the data being transported, as well as metadata
- Metadata is the data which contains information for routing information from sender to receiver
- Routers are special purpose computers with a MAC address
- Computers send data, to a router, which will either deliver to final location, or another router which will put on a path to the proper location
- Internet was designed to be able to change in size and scale to meet new demands
- Local Area Network(LAN): physical connections of computers in a close location, 1 - 100s systems
- Intranet: LANs connected by routers in a system, 100s - 1000s systems, usually in an organization
- Autonomous Systems: Larger intranets linked together under the control and policies of major organizations. Large routers link networks with large telecommunications connections, 10s of 1000s of systems. Controlled by internet providers
- The Internet: Autonomous Systems linked together, large routers linking ass via Special Telecomm Means(Fiber, T3 Satellites), Major Infrastructure( DNS, Cyber Operations)

Transport
- TCP: makes sure that receiver has gotten the package, slow but reliable
- UDP: does its best effort to get the package, fast but not guaranteed
- Port: number assigned to application or service
3 targets as defined by IP
- Unicast: a specific device. Internet wide access, TCP is used
- Multicast: a group of devices. Specific range of IP addresses, Internet wide access, UDP is used
- Broadcast: all devices. LAN wide, data stops at router, UDP is used

Application
- Domain Name Service: database which gives names to IPS. There are large servers which manage the name/IP mappings for each domain(.com, .net, .gov)
- Web Servers: programs running on machines connected to the Internet

- The World Wide Web, WWW, is a network of linked data and programs running over the Internet
- http. : how to ask and receive data from servers, usually uses TCP, with Port 80 has the transport layer
- https. : like http., but has security, usually uses TCP Port 443