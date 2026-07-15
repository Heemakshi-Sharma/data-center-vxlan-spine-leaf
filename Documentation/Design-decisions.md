## Introduction

This document explains the design choices made while building the Data Center Spine-Leaf Network.

# Why Spine-Leaf Architecture?

Traditional three-tier architectures become difficult to scale as the number of servers increases.

A Spine-Leaf architecture was selected because it provides:

- Predictable latency
- High bandwidth
- Better scalability
- Multiple redundant paths
- Simplified network expansion

# Why Two Spine Devices?

Two Spine devices provide:

- Redundancy
- Multiple forwarding paths
- High availability
- No single point of failure

If one Spine device becomes unavailable, traffic can continue through the remaining Spine.

# Why Two Leaf Devices?

Leaf devices act as access points for servers.

Each Leaf connects to every Spine to ensure:

- Redundant connectivity
- Consistent latency
- Equal forwarding opportunities

# Why Access Switches?

Access switches aggregate server connections.

Benefits include:

- Easy device management
- VLAN support
- Scalable server connectivity

# Why OSPF?

OSPF was selected because it is:

- A dynamic routing protocol
- Widely used in enterprise environments
- Fast to converge
- Suitable for Layer 3 underlay networks

# Why Layer 3 Links Between Spine and Leaf?

Layer 3 links eliminate many Layer 2 limitations.

Advantages include:

- No Spanning Tree dependency
- Better scalability
- Faster convergence
- Improved routing efficiency

# Why a Management Router?

A dedicated Management Router was included to simulate administrative access to the data center.

This reflects real enterprise environments where management traffic is separated from production traffic.

# Why Cisco Packet Tracer?

Cisco Packet Tracer provides a practical environment for learning network design and routing concepts.

Although it does not support VXLAN or EVPN, it is useful for understanding:

- Spine-Leaf topology
- Underlay routing
- OSPF
- IP addressing
- Enterprise network design principles
# Conclusion

The selected design provides a simplified representation of a modern enterprise data center while demonstrating the concepts behind scalable and resilient network architectures.
