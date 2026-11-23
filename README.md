# 🌐 SMART UNIVERSITY NETWORK SYSTEM
### Multi-Campus Network Design, Implementation & Simulation Using Cisco Packet Tracer

![Project](https://img.shields.io/badge/Project-Network%20Design-blue)
![Tool](https://img.shields.io/badge/Tool-Cisco%20Packet%20Tracer-orange)
![Networking](https://img.shields.io/badge/Domain-Computer%20Networking-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview

The **Smart University Network System** is a comprehensive multi-campus network design and simulation project developed using Cisco Packet Tracer. The project focuses on designing and implementing a secure, scalable, and reliable network infrastructure for a modern university environment consisting of multiple academic and administrative buildings, departments, and a geographically separated branch campus.

The proposed network architecture connects different university departments through a structured network infrastructure while maintaining departmental isolation, controlled communication, centralized IP address management, and secure external connectivity.

The system incorporates VLAN segmentation, inter-VLAN routing, dynamic routing, DHCP services, Network Address Translation (NAT), Access Control Lists (ACLs), wireless network integration, external email services, and an IoT-based fire detection and alert system.

The project also demonstrates how networking technologies can be integrated to improve communication, resource sharing, network security, and emergency response capabilities across a distributed university environment.

## 🎯 Project Objectives

The primary objectives of this project are:

- Design a structured and scalable multi-campus university network infrastructure.
- Establish reliable communication between the main campus and branch campus.
- Implement VLAN-based network segmentation for different departments.
- Configure inter-VLAN routing for controlled communication between network segments.
- Implement dynamic routing using RIPv2.
- Configure DHCP services for automatic IP address assignment.
- Apply ACLs to restrict unauthorized communication between selected VLANs.
- Configure NAT to provide external internet connectivity.
- Integrate wireless connectivity with the existing wired network.
- Configure DNS, HTTP, and external email connectivity.
- Integrate an IoT-based fire detection and notification system.
- Test network connectivity, routing, security policies, and network services.

## 🏗️ Network Architecture

The network follows a hierarchical campus network design consisting of core routing, distribution switching, and access-layer connectivity.

The proposed infrastructure includes:

### 1. Main Campus Network

The main campus acts as the central network infrastructure connecting three primary buildings:

**Building A – Administration and Business**
- VLAN 10 – Administrative Staff
- VLAN 20 – Business Faculty
- Layer 3 and Layer 2 switching infrastructure
- Wireless Access Point integration

**Building B – Engineering and Art/Design**
- VLAN 30 – Engineering and Computing Faculty
- VLAN 40 – Art and Design Faculty
- Department-based network segmentation

**Building C – Student Services and IT**
- VLAN 50 – Student Labs
- VLAN 60 – IT Department
- IT server infrastructure
- Email and network service connectivity

The report also defines VLAN 70 for Health and Sciences and VLAN 80 for reserved or special-purpose services.

### 2. Branch Campus Network

A separate branch campus is connected to the main campus through a WAN link.

The branch campus contains:

- VLAN 90 – Branch Campus Staff
- VLAN 100 – Branch Campus Students
- Dedicated branch campus router
- Independent VLAN structure
- RIPv2-based dynamic routing
- ACL-based traffic restrictions

This architecture allows the branch campus to maintain its local network operations while communicating with authorized main campus resources.

### 3. Internet Connectivity

The network includes an ISP/cloud router to provide external connectivity.

Key components include:
- ISP router integration
- Network Address Translation (NAT)
- Public IP-based external email server
- External network communication
- WAN connectivity between network routers

## 🧰 Technologies & Networking Concepts Used

| Technology | Implementation |
|---|---|
| Cisco Packet Tracer | Network design and simulation |
| VLAN | Department-based network segmentation |
| Inter-VLAN Routing | Communication between VLANs |
| RIPv2 | Dynamic routing |
| DHCP | Automatic IP address assignment |
| ACL | Network access control and traffic filtering |
| NAT | Private-to-public IP translation |
| DNS | Domain name resolution |
| HTTP | Web service connectivity |
| SMTP | Email transmission |
| WAN | Main and branch campus connectivity |
| WLAN | Wireless network integration |
| IoT | Fire detection and alert integration |
| IPv4 | Network addressing and subnetting |
| 802.1Q | VLAN trunking |

## 🔐 Network Security Implementation

Network security is an important part of this project.

The following security mechanisms are implemented:

**1. VLAN Segmentation**
- Separates university departments into logical network segments.
- Reduces unnecessary broadcast traffic.
- Provides departmental network isolation.

**2. Access Control Lists (ACLs)**
- Controls traffic between selected VLANs.
- Blocks unauthorized communication.
- Implements specific inbound traffic restrictions.
- Maintains controlled access between main and branch campus networks.

**3. NAT**
- Translates private IP addresses for external connectivity.
- Allows multiple internal devices to share external connectivity.
- Hides the internal addressing structure from external networks.

**4. Wireless Security**
- WPA2 wireless security configuration.
- Access Point mode integration.
- Wireless clients follow the security policies of the connected VLAN.

## 🤖 IoT-Based Fire Detection System

One of the major features of this project is the integration of an IoT-based fire detection and alert system.

The system includes:

- Fire Sensor
- Fire Monitor
- Single Board Computer (SBC)
- Speaker
- Wireless Network Connectivity

### Working Process

1. The fire sensor detects a fire-related event.
2. The fire monitor receives the detection signal.
3. The SBC processes the fire detection information.
4. The system generates an alert message.
5. The alert is transmitted through the university network.
6. Administrative computers in VLAN 10 receive the notification.
7. The speaker provides an audible warning.

This implementation demonstrates how IoT devices can be integrated into a campus network to support emergency monitoring and improve safety response.

## 🌍 IP Addressing & VLAN Configuration

The project uses a structured IPv4 addressing scheme based on private IP subnets.

| VLAN ID | Department / Purpose | Network Address |
|---|---|---|
| VLAN 10 | Administrative Staff | 192.168.1.0/24 |
| VLAN 20 | Business Faculty | 192.168.2.0/24 |
| VLAN 30 | Engineering & Computing | 192.168.3.0/24 |
| VLAN 40 | Art & Design | 192.168.4.0/24 |
| VLAN 50 | Student Labs | 192.168.5.0/24 |
| VLAN 60 | IT Department | 192.168.6.0/24 |
| VLAN 70 | Health & Sciences | 192.168.7.0/24 |
| VLAN 80 | Reserved / Special Purpose | 192.168.8.0/24 |
| VLAN 90 | Branch Campus Staff | 192.168.9.0/24 |
| VLAN 100 | Branch Campus Students | 192.168.10.0/24 |

**Addressing Details:**
- Subnet Mask: 255.255.255.0 (/24)
- Default Gateway: .1 address of each VLAN subnet
- WAN point-to-point connections: /30 subnet
- External Email Server IP: 200.0.0.90

## ⚙️ Major Implementation Tasks

The project implementation was completed through the following stages:

1. Network requirement analysis and topology planning.
2. Network device selection and connection establishment.
3. Main campus and branch campus router configuration.
4. VLAN creation and switch port assignment.
5. Trunk port configuration using 802.1Q.
6. Inter-VLAN routing configuration.
7. DHCP pool configuration for automatic IP allocation.
8. RIPv2 dynamic routing configuration.
9. ACL implementation and security policy testing.
10. NAT configuration for external connectivity.
11. DNS, HTTP, and email service configuration.
12. Wireless Access Point integration.
13. IoT fire detection and alert system integration.
14. Network connectivity and functionality testing.

## 🧪 Testing & Validation

After implementation, different network components and services were tested to verify the system's functionality.

The testing process included:

- Ping testing between different network devices.
- VLAN connectivity verification.
- Inter-VLAN communication testing.
- DHCP automatic IP assignment verification.
- RIPv2 routing table and route exchange verification.
- ACL traffic restriction testing.
- NAT and external server connectivity testing.
- Main and branch campus communication testing.
- Wireless client connectivity testing.
- IoT fire detection and alert notification testing.

### Reported Testing Results

According to the project report:

- VLAN segmentation and inter-VLAN routing operated as designed.
- Devices received IP addresses automatically through DHCP.
- RIPv2 exchanged routing information between routers.
- ACL policies restricted selected network traffic.
- NAT provided external connectivity.
- The branch campus communicated with the main campus.
- Wireless clients integrated with the wired infrastructure.
- The IoT fire detection system transmitted alerts to administrative personnel.
- External email server connectivity was verified.

The report also records DHCP address assignment under 5 seconds and fire alert transmission under 2 seconds during the described simulation testing.

## 📸 Project Screenshots

### Network Topology & Architecture

![Smart University Network Topology](Screenshots/Network-Topology.jpg)

### Project Configuration

The complete network configuration, router settings, VLAN implementation, routing configuration, and testing screenshots are documented in the project report.

For detailed implementation evidence, please check the Documentation folder.

## 📂 Project Repository Structure

```text
Smart-University-Network-System/
│
├── README.md
│
├── Packet-Tracer/
│   └── Smart-University-Network-System.pkt
│
├── Documentation/
│   └── Project-Report.pdf
│
└── Screenshots/
    └── Network-Topology.jpg
```

## 🚀 How to Open the Project

To explore and simulate this network project:

1. Download or clone this GitHub repository.
2. Install Cisco Packet Tracer on your computer.
3. Open the Packet-Tracer folder.
4. Locate the Smart-University-Network-System.pkt file.
5. Open the file using Cisco Packet Tracer.
6. Explore the network topology, routers, switches, VLANs, and connected devices.
7. Use the CLI of network devices to inspect their configurations.

## 📚 Learning Outcomes

Through this project, I gained practical knowledge and experience in:

- Computer networking fundamentals.
- Network topology design and implementation.
- IPv4 addressing and subnetting.
- VLAN creation and management.
- Router and switch configuration.
- Inter-VLAN routing.
- Dynamic routing using RIPv2.
- DHCP configuration and troubleshooting.
- ACL-based network security.
- NAT configuration.
- WAN connectivity.
- Wireless network integration.
- Network service configuration.
- IoT integration in networking.
- Network connectivity testing and troubleshooting.

## 👨‍💻 Project Information

**Project Name:** Smart University Network System

**Developed By:** MD Faisal Mahmud

**Institution:** Premier University, Chattogram

**Department:** Computer Science & Engineering (CSE)

**Course:** Computer Network Laboratory

**Course Code:** CSE 3568

**Project Type:** Academic Networking Project

**Development Tool:** Cisco Packet Tracer

**Project Date:** November 30, 2025

## 🎓 Final Remarks

The Smart University Network System demonstrates the design and simulation of a secure, scalable, and interconnected multi-campus network infrastructure using Cisco Packet Tracer.

By combining VLAN segmentation, dynamic routing, network security, automated IP management, wireless connectivity, external network services, and IoT-based fire detection, this project illustrates the practical application of computer networking concepts in a modern educational environment.

This project strengthened my practical understanding of network design, router and switch configuration, network security, connectivity management, and troubleshooting.

---

**Thank you for visiting my project repository!**

If you find this project interesting, feel free to explore the repository and review the network simulation and documentation.
