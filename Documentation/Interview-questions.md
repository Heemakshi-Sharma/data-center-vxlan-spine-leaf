## 1. What is a Spine-Leaf Architecture?

A Spine-Leaf architecture is a two-tier Layer 3 network design in which every Leaf switch connects to every Spine switch. This provides predictable latency, redundancy, and scalability.

## 2. Why is Spine-Leaf preferred over a traditional three-tier architecture?

Because it offers:

- Better scalability
- Lower latency
- Redundant paths
- Improved east-west traffic performance

## 3. What is East-West Traffic?

East-West traffic refers to communication between servers within the data center.

Example:

Server → Server

## 4. What is North-South Traffic?

North-South traffic refers to communication between users outside the data center and internal servers.

Example:

User → Web Server

## 5. What is the Underlay Network?

The Underlay Network is the physical IP network connecting Spine and Leaf devices.

## 6. What is the Overlay Network?

The Overlay Network is a virtual network built on top of the Underlay Network to carry Layer 2 traffic across a Layer 3 infrastructure.

## 7. What is VXLAN?

VXLAN (Virtual Extensible LAN) is a Layer 2 overlay technology that extends Layer 2 networks across Layer 3 networks.

## 8. What is a VTEP?

A VXLAN Tunnel Endpoint (VTEP) encapsulates and decapsulates VXLAN traffic between the Overlay and Underlay networks.

## 9. What is a VNI?

A VXLAN Network Identifier (VNI) is a 24-bit identifier used to uniquely identify VXLAN segments.

## 10. Why is OSPF used in this project?

OSPF provides dynamic routing between the Spine and Leaf devices, enabling efficient Layer 3 connectivity within the Underlay Network.
