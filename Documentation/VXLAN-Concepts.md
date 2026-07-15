# VXLAN and Spine-Leaf Architecture Concepts

## Introduction

Modern enterprise data centers require networks that are scalable, highly available, and capable of supporting large amounts of east-west traffic between servers.

Traditional three-tier network architectures often face scalability limitations and increased latency. To overcome these challenges, modern data centers commonly adopt a Spine-Leaf architecture with VXLAN.

Although Cisco Packet Tracer does not support native VXLAN implementation, this project was designed to understand the architecture, traffic flow, and concepts used in real-world data center networks.

# Traditional Three-Tier Architecture

A traditional enterprise data center typically consists of:

- Core Layer
- Distribution Layer
- Access Layer

### Limitations

- Higher latency
- Multiple forwarding hops
- Limited scalability
- Spanning Tree blocking links
- Difficult expansion

These limitations led to the adoption of Spine-Leaf architecture.

# Spine-Leaf Architecture

The Spine-Leaf architecture is a two-tier Layer 3 network design used in modern data centers.

It consists of:

## Spine Layer

The Spine Layer forms the backbone of the data center.

Responsibilities:

- Connect all Leaf devices
- Provide high-speed Layer 3 forwarding
- Maintain redundant paths
- Ensure predictable latency

In this project:

- Spine1
- Spine2

represent the Spine Layer.

## Leaf Layer

Leaf devices connect servers, storage devices, and access switches.

Responsibilities:

- Connect end devices
- Route traffic toward the Spine Layer
- Act as access points for workloads

In this project:

- Leaf1
- Leaf2

represent the Leaf Layer.

# Underlay Network

The Underlay Network is the physical IP network that connects all Spine and Leaf devices.

Characteristics:

- Layer 3 routing
- OSPF used for routing
- Provides IP connectivity between devices
- Supports the Overlay network

In this project, OSPF was configured to establish connectivity between the Spine and Leaf routers.

# Overlay Network

The Overlay Network is a virtual network built on top of the Underlay Network.

Responsibilities:

- Connect workloads across the data center
- Extend Layer 2 networks
- Isolate tenant traffic

VXLAN operates within the Overlay Network.

# What is VXLAN?

VXLAN (Virtual Extensible LAN) is a Layer 2 overlay technology that allows Ethernet frames to be transported across a Layer 3 network.

VXLAN provides:

- Layer 2 extension
- Large network scalability
- Support for multi-tenant environments
- Efficient virtual machine mobility

VXLAN is commonly used in cloud data centers and enterprise networks.

# What is a VTEP?

A VXLAN Tunnel Endpoint (VTEP) is a network device responsible for:

- Encapsulating Ethernet frames into VXLAN packets
- Sending VXLAN traffic across the Underlay Network
- Decapsulating VXLAN packets at the destination

Cisco Nexus switches commonly perform the VTEP function.

Cisco Packet Tracer does not support VTEP configuration.

# What is a VNI?

A VXLAN Network Identifier (VNI) is a 24-bit identifier used to distinguish different VXLAN segments.

Benefits include:

- Up to 16 million logical networks
- Better scalability than traditional VLANs
- Tenant isolation

Unlike VLAN IDs, which are limited to 4094, VNIs provide significantly larger address space.


# East-West vs North-South Traffic

## East-West Traffic

Communication between servers within the data center.

Examples:

- Server to Server
- Virtual Machine to Virtual Machine
- Database synchronization

Spine-Leaf architecture is optimized for East-West traffic.

## North-South Traffic

Communication between users outside the data center and servers inside the data center.

Examples:

- User accessing a website
- Client connecting to an application server

# Equal-Cost Multi-Path (ECMP)

Spine-Leaf networks often use Equal-Cost Multi-Path (ECMP) routing.

Benefits:

- Load balancing
- Multiple active forwarding paths
- Better bandwidth utilization
- Higher availability

Although ECMP was not implemented in Cisco Packet Tracer, understanding the concept is essential for modern data center networking.

# Project Limitations

Cisco Packet Tracer does not currently support:

- VXLAN encapsulation
- VTEP configuration
- MP-BGP EVPN
- EVPN control plane
- VXLAN tunnel creation
- Cisco Nexus features

Therefore, this project focuses on the Layer 3 Underlay network while studying VXLAN concepts theoretically.


# Key Learning Outcomes

Through this project, I developed an understanding of:

- Spine-Leaf architecture
- Modern data center design
- Underlay and Overlay networking
- VXLAN fundamentals
- VTEP concepts
- VNI concepts
- East-West traffic optimization
- Enterprise data center scalability
- OSPF-based Underlay routing
- 
# Conclusion

This project provided practical exposure to modern data center design principles using Cisco Packet Tracer. While the platform does not support full VXLAN implementation, it served as an effective environment for understanding the architecture, traffic flow, routing, and design concepts that form the foundation of enterprise VXLAN-based data center networks.
