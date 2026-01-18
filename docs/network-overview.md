# Network Overview


This project demonstrates a multi subnet network built in Cisco Packet Tracer using VLSM subnetting, VLAN segmentation, inter-VLAN routing, DHCP relay, and wireless client integration.

The goal of this network is to simulate a small enterprise style environment where different device groups are logically separated into subnets while still being able to communicate through a central routing device.


## Logical Network Design

The network is divided into multiple subnets using Variable Length Subnet Masking (VLSM) to efficiently allocate IP address space based on the size and purpose of each network segment.

Each subnet represents a different functional group within the network, such as servers, wired clients, and wireless clients. VLANs are used to logically separate these groups at Layer 2, improving security, reducing broadcast traffic, and making the network easier to manage.

Inter-VLAN routing is handled by a router, allowing controlled communication between subnets while maintaining logical separation. This design reflects a common enterprise network architecture where segmentation and routing are used together to balance security and connectivity.


## Subnetting & Addressing Strategy

Variable Length Subnet Masking (VLSM) is used in this network to allocate IP address space efficiently based on the number of required hosts in each subnet.

Each subnet was sized according to its role within the network. Server and wired client networks were allocated larger address blocks, while the wireless subnet was allocated a smaller block due to having fewer devices.

Subnet 4 was assigned the network address `220.240.60.24/29`. This provides a total of 6 usable IP addresses, which is sufficient for the access point and associated wireless clients.

The router interface for Subnet 4 uses the first usable address (`220.240.60.25`) as the default gateway. Wireless clients are dynamically assigned IP addresses starting from `220.240.60.26` via DHCP.

This addressing approach ensures efficient IP utilization while maintaining clear separation between network segments.

