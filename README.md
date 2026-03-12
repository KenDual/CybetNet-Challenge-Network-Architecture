# Smart Campus Network Simulation

## Overview

The goal is to design and simulate a secure campus network infrastructure for an e-learning environment that supports multiple laboratories and departments.

The system models the network architecture of a university campus including administrative offices, classrooms, and library services. The project focuses on network design, segmentation, and security in an enterprise-like environment.

The simulation was implemented using Cisco Packet Tracer.

## Objectives

* Design a scalable campus network architecture.
* Implement a hierarchical network model (Core – Distribution – Access).
* Configure network services such as DHCP, DNS, VLAN, VPN, and routing.
* Improve network security using segmentation and layered protection.
* Practice network management and troubleshooting skills.

## Network Architecture

The network follows a hierarchical model:

Core Layer
Handles routing, DHCP services, and inter-VLAN communication.

Distribution Layer
Manages traffic between access switches and the core network.

Access Layer
Connects end devices such as PCs and lab machines.

The architecture allows centralized control, scalability, and easier management.

## Key Technologies

### DHCP

Dynamic Host Configuration Protocol is used to automatically assign IP addresses and network configuration to devices.

Benefits:

* Automatic IP allocation
* Reduced configuration errors
* Easier network management
* Better scalability for large networks

The Core Switch acts as the DHCP server for VLANs in the system.

### VLAN

Virtual Local Area Network is used to logically segment the network into different departments.

Benefits:

* Reduces broadcast traffic
* Improves security by isolating departments
* Simplifies network management
* Optimizes bandwidth usage

### Routing

Routers and Layer-3 switches are used to allow communication between VLANs and external networks.

Routing operates at Layer 3 of the OSI model and determines the best path for data packets between networks.

### NAT

Network Address Translation allows private IP addresses inside the campus network to access the public internet.

Benefits:

* Saves IPv4 addresses
* Hides internal network structure
* Improves security

## Implementation

The system includes:

* Multiple VLANs for different departments
* A Core Layer-3 switch acting as DHCP server
* Access switches configured with trunk and access ports
* Inter-VLAN routing
* NAT configuration on the edge router
* Network verification using ping and IP configuration checks

## Testing

Network functionality was tested by:

* Automatically assigning IP addresses via DHCP
* Verifying gateway connectivity
* Testing communication between VLANs
* Testing external connectivity through NAT

Commands such as `ipconfig`, `show ip dhcp binding`, and `show ip dhcp pool` were used to validate the configuration.

## Tools Used

* Cisco Packet Tracer
* Networking protocols (DHCP, VLAN, NAT, Routing)

## Author

Mai Phu Hai  
Email: maiphuhai123@gmail.com  
Phone: +84 348043061
