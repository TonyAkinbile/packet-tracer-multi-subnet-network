# packet-tracer-multi-subnet-network
Cisco Packet Tracer project demonstrating VLSM subnetting, inter VLAN routing, DHCP relay, and wireless network integration.

For a detailed explanation of the network design, subnetting decisions, and routing strategy, see the [Network Overview](docs/network-overview.md).

<img width="1624" height="1019" alt="topology-overview" src="https://github.com/user-attachments/assets/d6838b3a-6359-4942-a7cc-d2315ddbca18" />


## What This Project Demonstrates

- Multi-subnet design using VLSM
- Inter-VLAN routing via a central router
- Centralized DHCP serving multiple subnets
- Wired and wireless client integration
- End-to-end connectivity validation

## Project Walkthrough (Visual)

### Network Topology
![Network Topology](docs/images/topology-overview.png)  
Overall logical topology showing segmented subnets, routing device, DHCP server, and wireless access point.

### DHCP Server Configuration
![DHCP Server Configuration](docs/images/dhcp-server-config.png)  
Central DHCP server configured with multiple address pools to serve different subnets.

### Wired Client DHCP Assignment
![PC DHCP Assignment](docs/images/PC0 DHCP.png)  
Wired client successfully receiving an IP address via DHCP.

### Wireless Client DHCP Assignment
![Wireless DHCP Client](docs/images/wireless-dhcp-client.png)  
Wireless client receiving an IP address through the access point.

### Inter-Subnet Connectivity Test
![Inter-Subnet Ping](docs/images/inter-subnet-ping.png)  
Ping results confirming successful communication between different subnets.

## Design Details
For a deeper explanation of subnetting, routing, and design decisions, see:
👉 [Network Overview](docs/network-overview.md)
