# Networking Lab - CCNA 200-301 (Packet Tracer)

## Overview
This repository contains a Packet Tracer lab setup for testing and configuring various concepts of the CCNA 200-301 exam. <br>

Networking is the backbone of the modern world, enabling the internet and making data accessible globally in seconds. It has shaped the world as we know it today. In this repository, I will showcase various routing and switching technologies, demonstrating my knowledge, skills, and passion for networking.




## Table of Contents
- [Lab Topology](#lab-topology)
-  [Static Routes](#static-routes)
-  [Default Route](#default-route)
- [RIP Configuration](#rip-configuration)
- [OSPF Configuration](#ospf-configuration)
- [EIGRP Configuration](#eigrp-configuration)
- [BGP](BGP)
- [VLAN](#vlan)
- [Inter VLAN](#inter-vlan)
- [VTP](#vtp)
- [STP](#stp)
- [ACL](#acl)
- [NAT](NAT)




## Routing
Routing is like finding the best path for data to travel from one place to another. It enables data to travel from the North Pole to the South Pole and beyond. Routing protocols such as OSPF, RIP, EIGRP, BGP, Static Routing, and Default Routing determine the most efficient route for data to reach its destination.
<sub>
## RIP

<b><u>RIPv2</u></b><br>
<p align="center">
  <img src="https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/img/RIPv2.png" alt="Let's Get Started">
</p>
## 📁Download Topology :   [Click Here](https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/RIPv2/RIPv2.pkt)  🔫<br>
<br>


## Static Route
Static routes are manually configured and are commonly used for routing traffic between remote networks or in simpler network setups.

Key Features: Static routes require the manual addition of each route into the routing table. They do not change unless manually reconfigured.
Common Use Cases: Useful for smaller networks or when precise control over routing is needed.
Lab Focus: Implementing static routes to control traffic flow to specific destinations.
 **Use in Lab**: Static routes are set up between the routers to ensure that specific traffic follows predefined paths.<br>
 <p align="center">
  <img src="https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/img/Static%20route.png">
</p>
## 📁Download Topology :   [Click Here](https://github.com/satabdisaha/CCNA-200-301/tree/main/CCNA_200-301/STATIC)  🔫<br>
<br>


## OSPF Configuration
OSPF (Open Shortest Path First)<br>
<b>Overview:</b> OSPF is a link-state routing protocol that uses the Dijkstra algorithm to find the shortest path. It is commonly used in larger networks due to its scalability and fast convergence.<br>
<b>Key Concepts:</b>
<b>LSAs (Link-State Advertisements):</b> These are used to share routing information between routers.
<b>Usage:</b> Best for larger networks due to its ability to scale with multiple areas and compllex topologies.<br>

## OSPFv2

<p align="center">
  <img src="https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/img/OSPFv2.png" alt="Let's Get Started">
</p>
## 📁Download Topology :   [Click Here](https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/OSPFv2/OSPFv2.pkt)  🔫<br>
<br>



## Multiarea OSPFv2

<p align="center">
  <img src="https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/img/multiarea%20ospf.png" alt="Let's Get Started">
</p>
## 📁Download Topology :   [Click Here](https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/Multiarea%20OSPF/multiarea%20ospf.pkt)  🔫<br>

## OSPFv3
<p align="center">
  <img src="https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/img/OSPFv3.png" alt="Let's Get Started">
</p>
## 📁Download Topology :   [Click Here](https://github.com/satabdisaha/CCNA-200-301/tree/main/CCNA_200-301/OSPF%20IPV6)  🔫<br>
<br>

## EIGRP (Enhanced Interior Gateway Routing Protocol)
Overview: EIGRP is a hybrid protocol, combining the advantages of both distance-vector and link-state protocols. It is faster and more efficient than RIP (Routing Information Protocol) due to its use of Diffusing Update Algorithm (DUAL).
Key Concepts:
Metric: EIGRP uses bandwidth, delay, load, and reliability to calculate the best path.
Feasible Successor: A backup route stored in the routing table for quicker recovery.
Authentication: EIGRP supports MD5 authentication to secure routing information.
Usage: EIGRP is ideal for medium-to-large-sized networks with fast convergence and low overhead.
<br>
<b><u>OSPFv2</u></b>
<p align="center">
  <img src="https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/img/EIGRP.png" alt="Let's Get Started">
</p>
## 📁Download Topology :   [Click Here](https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/EIGRP.pkt)  🔫<br>



## Default Route
The default route is used when the router cannot find a more specific match for the destination in the routing table. It provides a path for "unknown" or unspecified destinations.
The default route is configured to ensure that any traffic destined for unknown networks is forwarded to a specific gateway.

- **Purpose**: To route any unmatched traffic to a central router or gateway.
- **Use in Lab**: The default route ensures that traffic without an explicit route is forwarded correctly, simulating a real-world gateway setup.
- 
- <p align="center">
  <img src="https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/img/Default%20Route.png" alt="Let's Get Started">
</p>
## 📁Download Topology :   [Click Here]( https://github.com/satabdisaha/CCNA-200-301/tree/main/CCNA_200-301/default%20route)  🔫<br>

## BGP(Border Gateway Protocol)
BGP is a border gateway protocol that enables the internet to exchange routing information between autonomous systems (AS).



<p align="center">
  <img src="https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/img/BGP.png" alt="Let's Get Started">
</p>
## 📁Download Topology :   [Click Here]( https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/BGP/BGP.pk)  🔫<br>
</sub>
## Switching
Switching, or Layer 2 networking, is crucial for managing the data flow within a local area network (LAN). Switches work by learning and storing the MAC addresses of devices connected to them. They utilize technologies like VLANs, Inter-VLAN Routing, STP, RSTP, PortFast, EtherChannel, and Trunking. The MAC Address Table helps in making forwarding decisions for network traffic.<br>

## VLANs (Virtual Local Area Networks)
Overview: VLANs are used to logically segment networks into different broadcast domains. VLANs improve security, performance, and network management.
Key Concepts:
Trunking: switchport mode trunk, switchport trunk encapsulation dot1q
VTP (VLAN Trunking Protocol): Helps manage VLANs across multiple switches. It can operate in Server, Client, and Transparent modes.
Usage: VLANs enhance network performance and segmentation. Trunk links allow multiple VLANs to be transmitted over a single physical link.

<p align="center">
  <img src="https://github.com/satabdisaha/CCNA-200-301/blob/main/CCNA_200-301/img/VLAN.png" alt="Let's Get Started">
</p>
## 📁Download Topology :   [Click Here]( https://github.com/satabdisaha/CCNA-200-301/tree/main/CCNA_200-301/VLAN)  🔫<br>


##  STP (Spanning Tree Protocol)
Overview: STP is used to prevent loops in a switched network by blocking redundant paths. The protocol uses the Bridge Protocol Data Units (BPDU) to elect the root bridge and determine which paths to block.
Key Concepts:
Port States: Blocking, Listening, Learning, Forwarding
Root Bridge Election: The switch with the lowest bridge priority or MAC address becomes the root bridge.
RSTP (Rapid Spanning Tree Protocol): An enhanced version of STP that converges faster.
Usage: STP prevents broadcast storms and network loops in Layer 2 networks.

## EtherChannel (Link Aggregation)
Overview: EtherChannel combines multiple physical links into a single logical link to increase bandwidth and provide redundancy.
Key Concepts:
Protocols: PAgP (Port Aggregation Protocol), LACP (Link Aggregation Control Protocol)

Usage: EtherChannel is used to increase bandwidth and provide redundancy between switches and routers.

## VPN and Tunneling
To maintain the confidentiality, integrity, and authenticity of data, configuring IPSec VPN is crucial. This protocol encrypts the data, transforming it into ciphertext to ensure its security during transmission.
When transferring data across different locations, creating a secure tunnel is essential. A tunnel provides a virtual point-to-point connection while ensuring data security. Technologies like GRE Tunnels and IPSec VPN Tunnels are used to achieve this. In fact, there are combinations of these two, such as IPSec VPN over GRE and GRE over IPSec VPN, which offer both encryption and encapsulation.<br>
Key Concepts:<br>
IPsec: Provides encryption and secure tunneling for VPNs.<br>
GRE Tunnels: Used to create point-to-point connections over IP networks.

## Network Security
Data is one of the most important assets for any individual or organization, making it essential to protect it. One key security feature is ACL (Access Control Lists), which ensures that only authorized users and devices can access specific resources or visit certain websites.<br>

Physical layer security also requires the proper configuration of network devices, such as switch port security, syslog, password policies, and device protection to prevent unauthorized access.

## ACL (Access Control Lists)
Overview: ACLs are used to filter network traffic based on source IP, destination IP, or other attributes. They provide security by controlling which traffic is allowed or denied to/from a network.
Key Concepts:
Standard ACLs: Filter traffic based on the source IP address only.
Extended ACLs: Filter based on source/destination IP, protocol, or port.
Named ACLs: Easier to manage and troubleshoot.
Numbered ACLs: Easier to manage and troubleshoot.
Usage: ACLs are essential for securing network devices and controlling traffic flow.

## NAT (Network Address Translation)
Overview: NAT allows a single public IP address to represent multiple private IP addresses. This helps conserve public IP addresses and adds a layer of security by masking internal IP addresses.
Key Concepts:
Static NAT: A one-to-one mapping of private and public IP addresses.
Dynamic NAT: Maps private IPs to a pool of public IPs.
PAT (Port Address Translation): A form of dynamic NAT where multiple priCommand: ip nat inside source list [ACL] interface [interface] overload
Usage: NAT is used extensively in home and corporate networks to provide internet access to devices with private IPs.

## DHCP and DNS
DHCP (Dynamic Host Configuration Protocol) automates the process of assigning IP addresses to devices, reducing the need for manual IP configuration and saving time. <br>
DNS (Domain Name System) translates domain names to IP addresses, making it easier for users to access websites without needing to remember complex numerical IP addresses.

## Remote Access
In the year 2025, working from home has become a popular concept. To make networking devices accessible from anywhere, protocols like Telnet and SSH are essential. These technologies allow for remote management of network devices, ensuring that they can be accessed securely from any location.


