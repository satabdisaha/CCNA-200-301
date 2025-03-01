# Networking Lab - CCNA 200-301 (Packet Tracer)

## Overview
This repository contains a Packet Tracer lab setup for testing and configuring various routing, switching, VPN, security protocols and techniques, including **OSPF (Open Shortest Path First)**, **EIGRP (Enhanced Interior Gateway Routing Protocol)**, **Static Routes**, and **Default Routes**. The configurations in this lab are designed to provide hands-on experience with these routing concepts using Cisco Packet Tracer.

## Table of Contents
- [Lab Topology](#lab-topology)
-  [Static Routes](#static-routes)
-  [Default Route](#default-route)
- [RIP Configuration](#rip-configuration)
- [OSPF Configuration](#ospf-configuration)
- [EIGRP Configuration](#eigrp-configuration)
- [VLAN](#vlan)
- [Inter VLAN](#inter-vlan)
- [VTP](#vtp)
- [STP](#stp)
- [ACL](#acl)
- [NAT](NAT)


- 


## Lab Topology
This lab contains a simple network topology designed to demonstrate OSPF, EIGRP, static routes, and default routes. The network consists of routers, switches, and PCs, interconnected as follows:

- **Topology Details**: 
  - Multiple routers connected in either a hub-and-spoke or full mesh configuration.
  - Each router is configured to test and compare different routing protocols.
  - PCs are used as endpoints to test connectivity across the network.




##RIP

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

## VLANs (Virtual Local Area Networks)
Overview: VLANs are used to logically segment networks into different broadcast domains. VLANs improve security, performance, and network management.
Key Concepts:
Trunking: switchport mode trunk, switchport trunk encapsulation dot1q
VTP (VLAN Trunking Protocol): Helps manage VLANs across multiple switches. It can operate in Server, Client, and Transparent modes.
Usage: VLANs enhance network performance and segmentation. Trunk links allow multiple VLANs to be transmitted over a single physical link.

## Switching and STP (Spanning Tree Protocol)
Overview: STP is used to prevent loops in a switched network by blocking redundant paths. The protocol uses the Bridge Protocol Data Units (BPDU) to elect the root bridge and determine which paths to block.
Key Concepts:
Port States: Blocking, Listening, Learning, Forwarding
Root Bridge Election: The switch with the lowest bridge priority or MAC address becomes the root bridge.
RSTP (Rapid Spanning Tree Protocol): An enhanced version of STP that converges faster.
Usage: STP prevents broadcast storms and network loops in Layer 2 networks.

##ACLs (Access Control Lists)
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

## DHCP (Dynamic Host Configuration Protocol)
Overview: DHCP automatically assigns IP addresses and other network configurations to devices on a network, simplifying network management.
Key Concepts:
DHCP Pool: A range of IP addresses that the DHCP server can assign.
DHCP Relay: Allows DHCP clients to receive configuration information from a remote DHCP server.
DHCPv6: Provides similar functionality for IPv6 addresses.
Usage: DHCP reduces manual configuration and simplifies network management.

## EtherChannel (Link Aggregation)
Overview: EtherChannel combines multiple physical links into a single logical link to increase bandwidth and provide redundancy.
Key Concepts:
Protocols: PAgP (Port Aggregation Protocol), LACP (Link Aggregation Control Protocol)

Usage: EtherChannel is used to increase bandwidth and provide redundancy between switches and routers.

## VPN (Virtual Private Network)
Overview: VPNs provide secure communication over an insecure network (like the internet). VPNs are used to encrypt data and ensure privacy between remote sites or users and the main network.
Key Concepts:
IPsec: Provides encryption and secure tunneling for VPNs.
GRE Tunnels: Used to create point-to-point connections over IP networks.
Usage: VPNs are essential for securely connecting remote users or branch offices to a corporate network.
