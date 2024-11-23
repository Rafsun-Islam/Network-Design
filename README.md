# Network Design for Apex University

This project demonstrates the design and implementation of a complex network infrastructure for Apex University, featuring multiple subnets, dynamic routing, DHCP, DNS, and web server configuration using Cisco Packet Tracer.

**Note: This project is for educational purposes only.**

## Project Overview

Apex University requires a full-fledged network infrastructure to support its academic and administrative operations. This project involves the creation of a network model that reflects the university's multi-campus structure with interconnected subnets and essential features such as:

- A web server hosting the university's website (`http://www.apex.edu.bd`).
- A single DNS server for resolving the university's domain.
- Automatic IP assignment using a centralized DHCP server.
- Seven LANs with a mix of wired and wireless hosts, each representing a campus.
- Dynamic routing using OSPF.
- Serial connections between campus routers.

## Features

1. **DNS and Web Server**:
   - A single DNS server is configured to resolve the university's domain.
   - A web server hosts the university's website accessible from any campus.

2. **Centralized DHCP**:
   - A single DHCP server assigns IP addresses dynamically to all devices across campuses.
   - Future scalability is considered for subnet configurations.

3. **Multi-campus LANs**:
   - Seven LANs represent the university's campuses.
   - Each LAN contains wired and wireless devices for comprehensive connectivity.

4. **Routing and Connectivity**:
   - OSPF is used for dynamic routing across all campuses.
   - Serial connections are used between campus routers, adhering to the given topology.

## Network Topology

The network follows the predefined topology provided in the project guidelines. Seven routers connect the campuses, with each router managing a dedicated LAN.

## Configuration Details

### Dynamic Routing
- **Protocol**: OSPF
- Configuration commands:
  ```bash
  router ospf 1
  network [network-address] [wildcard-mask] area 0
  ip dhcp pool [pool-name]
  network [network-address] [subnet-mask]
  default-router [default-gateway]
  dns-server [DNS-server-IP]

- DNS configuration
   ```bash
   ip dns server
   ip host www.apex.edu.bd [Web-server-IP]
## Wireless and Wired Hosts
  - Wireless Access Points are included in each LAN.
  - IPs are assigned dynamically by the DHCP server.

## Tools Used
  - Cisco Packet Tracer: For network modeling and simulation.
  - Text Editor: For documentation and configuration scripts.
