# Networking Lab - OSPF, Static Route, Default Route, EIGRP (Packet Tracer)

## Overview
This repository contains a Packet Tracer lab setup for testing and configuring various routing protocols and techniques, including **OSPF (Open Shortest Path First)**, **EIGRP (Enhanced Interior Gateway Routing Protocol)**, **Static Routes**, and **Default Routes**. The configurations in this lab are designed to provide hands-on experience with these routing concepts using Cisco Packet Tracer.

## Table of Contents
- [Lab Topology](#lab-topology)
- [OSPF Configuration](#ospf-configuration)
- [Static Routes](#static-routes)
- [Default Route](#default-route)
- [EIGRP Configuration](#eigrp-configuration)
- [How to Use the Packet Tracer Lab](#how-to-use-the-packet-tracer-lab)
- [License](#license)

## Lab Topology
This lab contains a simple network topology designed to demonstrate OSPF, EIGRP, static routes, and default routes. The network consists of routers, switches, and PCs, interconnected as follows:

- **Topology Details**: 
  - Multiple routers connected in either a hub-and-spoke or full mesh configuration.
  - Each router is configured to test and compare different routing protocols.
  - PCs are used as endpoints to test connectivity across the network.

*(You can include a diagram of your topology here or describe how each device is connected.)*

## OSPF Configuration
Open Shortest Path First (OSPF) is configured in this lab to establish routing between routers.

- **Purpose**: To simulate dynamic routing and observe how OSPF operates across multiple routers.
- **Use in Lab**: This section of the lab demonstrates how OSPF propagates routing information across the network and adapts to topology changes.

## Static Routes
Static routes are configured to manually route traffic to specific networks.

- **Purpose**: To show how manual routing can be used for simple and controlled network environments.
- **Use in Lab**: Static routes are set up between the routers to ensure that specific traffic follows predefined paths.

## Default Route
The default route is configured to ensure that any traffic destined for unknown networks is forwarded to a specific gateway.

- **Purpose**: To route any unmatched traffic to a central router or gateway.
- **Use in Lab**: The default route ensures that traffic without an explicit route is forwarded correctly, simulating a real-world gateway setup.

## EIGRP Configuration
Enhanced Interior Gateway Routing Protocol (EIGRP) is used in this lab to demonstrate a more advanced routing protocol.

- **Purpose**: To observe EIGRP’s faster convergence and better scalability compared to traditional distance-vector protocols.
- **Use in Lab**: EIGRP configurations allow for quick path selection and optimal routing within the lab’s network.

## How to Use the Packet Tracer Lab
Follow these instructions to set up and use the lab in Cisco Packet Tracer:

1. **Download Packet Tracer**:
   - If you don't have Cisco Packet Tracer, download it from Cisco’s website or access it through Cisco Networking Academy.
   
2. **Clone or Download the Repository**:
   - Clone or download this repository to access the Packet Tracer file and any necessary documentation.
   
3. **Open the Packet Tracer File**:
   - Open the `.pkt` (Packet Tracer) file included in this repository. It contains the network topology with pre-configured devices.
   
4. **Verify the Configuration**:
   - Check that all routers, switches, and PCs are connected correctly as per the topology.
   - Verify that each router has the appropriate routing protocol (OSPF, EIGRP, Static, and Default Routes) configured.
   
5. **Test Connectivity**:
   - Use `ping` or `traceroute` commands from PCs to test if the network routes are functioning correctly.
   - Observe the routing tables in the routers to ensure that routes are learned correctly.

6. **Modify the Network**:
   - Feel free to make changes, such as modifying IP addresses, adding new routers or switches, or altering the routing configurations to test how the network adapts to these changes.

## License
This repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
