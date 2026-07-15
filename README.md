Enterprise Data Center Network Design demonstrating Spine-Leaf architecture, Underlay/Overlay networking concepts, VXLAN fundamentals, and scalable data center design principles using Cisco Packet Tracer.

# Project Overview
This project demonstrates the design of a modern enterprise data center network based on the Spine-Leaf architecture.

The project focuses on understanding how large-scale data centers achieve scalability, high availability, low latency, and efficient east-west traffic forwarding.

Although Cisco Packet Tracer does not support native VXLAN EVPN implementation, the project was designed to study the architecture, traffic flow, and networking concepts used in production data centers.

# Business Scenario

A rapidly growing enterprise plans to migrate from a traditional three-tier campus network to a modern data center architecture.

The organization requires a network that provides:

- High scalability
- Low latency
- High bandwidth
- Layer 2 extension
- Efficient east-west traffic forwarding
- Simplified expansion
- Redundancy
- High availability

To achieve these objectives, the organization adopts a Spine-Leaf architecture based on VXLAN concepts.

# Project Objectives

- Understand traditional vs Spine-Leaf architecture.
- Design a scalable data center topology.
- Study Underlay and Overlay networking.
- Understand VXLAN fundamentals.
- Learn VTEP concepts.
- Understand VNI mapping.
- Study BGP EVPN concepts.
- Understand east-west traffic flow.
- Learn modern data center design principles.

# Network Architecture

The project consists of:

- Spine Switches
- Leaf Switches
- End Hosts
- Layer 3 Underlay
- VXLAN Overlay (Conceptual)
- Routed Links

The topology represents a simplified enterprise data center.

# Technologies & Concepts

- Cisco Packet Tracer
- Spine-Leaf Architecture
- VXLAN (Conceptual)
- VTEP Concepts
- VNI Concepts
- Underlay Network
- Overlay Network
- Layer 3 Routing
- ECMP Concepts
- TCP/IP

# Concepts Demonstrated

- Spine-Leaf Design
- East-West Traffic
- North-South Traffic
- Underlay Network
- Overlay Network
- VXLAN Fundamentals
- Data Center Scalability
- Network Redundancy
- Modern Data Center Design

# Skills Demonstrated

- Data Center Networking
- Network Architecture Design
- Enterprise Networking
- Cisco Networking
- Layer 3 Routing
- High Availability Concepts
- Network Scalability
- Traffic Engineering Fundamentals

# Project Limitations

Cisco Packet Tracer does not currently support native implementation of:

- VXLAN encapsulation
- EVPN
- VTEP configuration
- MP-BGP EVPN
- VXLAN tunnel creation

These technologies were studied conceptually and reflected in the network design rather than being fully configured.


# Verification

The following aspects were verified during the project:

- Layer 3 connectivity
- Routing verification
- End-to-end connectivity
- Spine-Leaf topology validation
- Underlay routing
- Traffic flow analysis

# Repository Structure

Data-Center-VXLAN/

│── README.md

│── DataCenter-VXLAN.pkt

├── Topology/

├── Configurations/

├── Screenshots/

├── Documentation/

├── Troubleshooting/

└── Verification/

# Challenges Faced

Some challenges encountered during this project included:

- Understanding Spine-Leaf architecture
- Underlay vs Overlay networking
- VXLAN packet forwarding concepts
- Mapping VNIs to VLANs
- Traffic flow visualization
- Packet Tracer platform limitations

These challenges were addressed through design validation, Cisco documentation, and repeated lab exercises.

# Lessons Learned

This project helped strengthen my understanding of:

- Modern data center architecture
- Spine-Leaf topology
- VXLAN fundamentals
- Underlay and Overlay networking
- Data center scalability
- Network redundancy
- East-West traffic optimization
- Enterprise network design principles

# Future Improvements

Future versions of this project will include:

- Cisco Nexus switches
- VXLAN configuration
- EVPN implementation
- MP-BGP
- VTEP configuration
- Multi-site VXLAN
- EVE-NG implementation
- Containerlab implementation
