# Enterprise Multi-Branch Network Design & Security

## Project Overview

This project was developed as part of the **Computer Communication Network Lab (CEL-223)** at Bahria University, Lahore Campus. The primary objective was to design and implement a scalable enterprise network that simulates a real-world organization with a **Head Office (HQ)** and **three remote branch offices** connected through a centralized ISP backbone.

The project demonstrates the practical implementation of key computer networking concepts, including **WAN connectivity, OSPF dynamic routing, VLAN-based network segmentation, DNS/Web services, and firewall-based network security**. Cisco Packet Tracer was used to design, configure, and test the complete network topology.

## Network Architecture

The network consists of four geographical locations:

- **Head Office (HQ)**
- **Branch A**
- **Branch B**
- **Branch C**

All locations are interconnected through a simulated **ISP backbone**, allowing communication between the different branches and the Head Office.

Routers are responsible for establishing communication between the different networks, while switches provide connectivity to end devices within each location. **OSPF (Open Shortest Path First)** was configured as the dynamic routing protocol, allowing routers to exchange routing information and automatically determine suitable paths to remote networks.

## VLAN Segmentation

To improve network organization and traffic management, **VLAN segmentation** was implemented within the enterprise network. VLANs logically divide the network into separate broadcast domains, making it easier to manage different groups of devices while improving scalability and reducing unnecessary broadcast traffic.

The VLAN configuration also demonstrates how an enterprise can separate internal network segments and control communication between them.

## DNS & Web Services

A dedicated **DNS Server** was configured as part of the network infrastructure to provide name-resolution services. This allows network users to access services using domain names instead of relying only on IP addresses.

Web services were also configured to demonstrate how enterprise network infrastructure can support application-level services alongside routing and switching components.

## Firewall & Network Security

Security was a major part of this project. A **Cisco ASA 5506-X Firewall** was implemented to provide perimeter security and control traffic entering or leaving the protected enterprise network.

To simulate a real-world cybersecurity scenario, **PC2 from Branch A was considered a compromised or malicious host** attempting to reach the Head Office network. Firewall rules and **Access Control Lists (ACLs)** were configured on the ASA firewall to block this unauthorized communication.

This demonstrates how firewalls can be used to enforce security policies, restrict suspicious hosts, and protect
