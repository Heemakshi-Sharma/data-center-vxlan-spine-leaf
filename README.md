# Project Overview

This project demonstrates the design of a modern data center network using a Spine-Leaf architecture.

The topology was created in Cisco Packet Tracer to understand how modern enterprise data centers are designed for scalability, redundancy, and low-latency communication.

Although Cisco Packet Tracer does not support native VXLAN EVPN implementation, this project focuses on understanding the architecture and networking concepts behind modern data center deployments.

# Business Scenario

A growing enterprise is expanding its private data center to host business-critical applications.

The existing three-tier network architecture has become difficult to scale and introduces unnecessary latency for east-west server communication.

To address these challenges, the organization plans to adopt a Spine-Leaf architecture inspired by VXLAN-based data center designs.

The new design aims to provide:

- High availability
- Horizontal scalability
- Redundant paths
- Low latency
- Simplified expansion
- Better east-west traffic performance

# Objectives

- Design a Spine-Leaf topology
- Understand Underlay networking
- Study VXLAN architecture concepts
- Learn VTEP and VNI concepts
- Configure Layer 3 connectivity
- Practice OSPF routing
- Verify end-to-end communication
- Understand enterprise data center architecture

# Network Topology

The network consists of:

- 2 Spine Routers
- 2 Leaf Routers
- 2 Access Switches
- 4 Servers
- 1 Management Router

Each Leaf Router is connected to both Spine Routers, creating redundant Layer 3 paths throughout the data center.

The complete topology is available in the **Topology** folder.

# Technologies Used

- Cisco Packet Tracer
- Cisco IOS
- OSPF
- IP Routing
- Spine-Leaf Architecture
- VXLAN Concepts
- Underlay Networking
- TCP/IP

# Architecture Components

## Spine Layer

The Spine Layer provides high-speed Layer 3 forwarding between Leaf devices.

Devices:

- Spine1
- Spine2

## Leaf Layer

Leaf Routers connect servers and access switches to the Spine Layer.

Devices:

- Leaf1
- Leaf2

## Access Layer

Access switches connect end devices to the data center network.

Devices:

- AccessSW1
- AccessSW2

## Server Layer

Four servers simulate workloads hosted inside the data center.

- Server1
- Server2
- Server3
- Server4

## Management Network

A dedicated Management Router provides administrative connectivity to the network.

# Features Demonstrated

- Spine-Leaf architecture
- Layer 3 Underlay
- OSPF Routing
- Redundant paths
- High availability concepts
- Enterprise topology design
- East-West traffic concepts
- End-to-end connectivity

# Project Limitations

Cisco Packet Tracer does not support:

- VXLAN tunnels
- VTEP configuration
- EVPN
- MP-BGP EVPN
- VXLAN encapsulation

These technologies were studied conceptually while implementing the Layer 3 underlay topology.

# Skills Demonstrated

- Data Center Networking
- Cisco Routing
- OSPF
- Enterprise Network Design
- High Availability Concepts
- Layer 3 Routing
- Underlay Networking
- Data Center Architecture

# Verification

The following tests were performed:

- OSPF neighbor verification
- Routing table verification
- Loopback reachability
- End-to-end ping tests
- Interface verification
- Underlay connectivity

# Folder Structure

data-center-spine-leaf-vxlan-design/

│── README.md

│── DataCenter-SpineLeaf.pkt

├── Topology/

├── Configurations/

├── Screenshots/

├── Documentation/

├── Troubleshooting/

# Lessons Learned

This project improved my understanding of:

- Modern Data Center Architecture
- Spine-Leaf Topology
- Underlay Routing
- High Availability
- East-West Traffic
- Network Scalability
- Enterprise Data Center Design

# Future Enhancements

Future improvements include:

- Cisco Nexus switches
- VXLAN implementation
- EVPN
- MP-BGP
- VTEP configuration
- Multi-site VXLAN
- EVE-NG implementation
