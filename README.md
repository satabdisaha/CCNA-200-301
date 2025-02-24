# Networking Lab - CCNA 200-301 (Packet Tracer)

## Overview
This repository contains a Packet Tracer lab setup for testing and configuring various routing, switching, VPN, security protocols and techniques, including **OSPF (Open Shortest Path First)**, **EIGRP (Enhanced Interior Gateway Routing Protocol)**, **Static Routes**, and **Default Routes**. The configurations in this lab are designed to provide hands-on experience with these routing concepts using Cisco Packet Tracer.

## Table of Contents
- [Lab Topology](#lab-topology)
- [OSPF Configuration](#ospf-configuration)
- [Static Routes](#static-routes)
- [Default Route](#default-route)
- [EIGRP Configuration](#eigrp-configuration)


## Lab Topology
This lab contains a simple network topology designed to demonstrate OSPF, EIGRP, static routes, and default routes. The network consists of routers, switches, and PCs, interconnected as follows:

- **Topology Details**: 
  - Multiple routers connected in either a hub-and-spoke or full mesh configuration.
  - Each router is configured to test and compare different routing protocols.
  - PCs are used as endpoints to test connectivity across the network.

*(You can include a diagram of your topology here or describe how each device is connected.)*


##Static Route
Static routes are manually configured and are commonly used for routing traffic between remote networks or in simpler network setups.

Key Features: Static routes require the manual addition of each route into the routing table. They do not change unless manually reconfigured.
Common Use Cases: Useful for smaller networks or when precise control over routing is needed.
Lab Focus: Implementing static routes to control traffic flow to specific destinations.
 **Use in Lab**: Static routes are set up between the routers to ensure that specific traffic follows predefined paths.


## OSPF Configuration
Open Shortest Path First (OSPF) is configured in this lab to establish routing between routers.

- **Purpose**: To simulate dynamic routing and observe how OSPF operates across multiple routers.
- **Use in Lab**: This section of the lab demonstrates how OSPF propagates routing information across the network and adapts to topology changes.



## Default Route
The default route is configured to ensure that any traffic destined for unknown networks is forwarded to a specific gateway.

- **Purpose**: To route any unmatched traffic to a central router or gateway.
- **Use in Lab**: The default route ensures that traffic without an explicit route is forwarded correctly, simulating a real-world gateway setup.

## EIGRP Configuration
Enhanced Interior Gateway Routing Protocol (EIGRP) is used in this lab to demonstrate a more advanced routing protocol.

- **Purpose**: To observe EIGRP’s faster convergence and better scalability compared to traditional distance-vector protocols.
- **Use in Lab**: EIGRP configurations allow for quick path selection and optimal routing within the lab’s network.


