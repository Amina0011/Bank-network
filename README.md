# Bank Network Simulation

## 📋 Project Overview

This project demonstrates the design and implementation of a secure, scalable banking network infrastructure using Cisco Packet Tracer. The simulation implements a multi-branch banking system with centralized data management, departmental segmentation, and robust security measures to reflect real-world enterprise banking network architecture.

## 🎯 Objectives

- Design a hierarchical network topology for a multi-branch banking institution
- Implement VLANs for network segmentation and security
- Configure dynamic routing protocols for efficient data transmission
- Set up centralized DHCP, DNS, and email services
- Ensure secure remote access and inter-branch communication
- Demonstrate network scalability and reliability

## 🏗️ Network Architecture

### Topology Structure
The network follows a hierarchical three-tier design:
- **Core Layer**: High-speed backbone connecting main branches
- **Distribution Layer**: Routing and policy enforcement
- **Access Layer**: End-user device connectivity

### Branch Structure
- **Main Branch**: Central headquarters with all departments and server infrastructure
- **Regional Branches**: Connected via WAN links with local departments
- **ATM Network**: Distributed ATM machines across locations

## 🔧 Technologies Used

- **Simulation Software**: Cisco Packet Tracer 7.0+
- **Routing Protocol**: OSPF (Open Shortest Path First)
- **Network Devices**: Routers, Multilayer Switches, Access Switches, Access Points
- **Servers**: DHCP, DNS, HTTP, Email, FTP
- **Security**: Port Security, VLANs, SSH, ACLs

## 📊 Network Components

### VLANs Configuration
| VLAN ID | Department | Network Address | Subnet Mask | Users |
|---------|------------|-----------------|-------------|-------|
| 10 | Management | 192.168.10.0 | 255.255.255.192 | 60 |
| 20 | IT/Server Room | 192.168.10.64 | 255.255.255.192 | 20 |
| 30 | Human Resources | 192.168.10.128 | 255.255.255.192 | 60 |
| 40 | Accounts | 192.168.10.192 | 255.255.255.192 | 60 |
| 50 | Customer Service | 192.168.11.0 | 255.255.255.192 | 60 |
| 60 | Finance | 192.168.11.64 | 255.255.255.192 | 60 |

### Server Infrastructure
- **DHCP Server**: Automatic IP address allocation for all departments
- **DNS Server**: Name resolution services
- **HTTP/HTTPS Server**: Internal web portal and banking application
- **Email Server**: Internal communication system
- **FTP Server**: File transfer and document management

## 🔒 Security Implementation

### Network Security Features
1. **VLAN Segmentation**: Isolated broadcast domains for each department
2. **Access Control Lists (ACLs)**: Traffic filtering and department isolation
3. **Port Security**: MAC address filtering on switch ports
4. **SSH Configuration**: Secure remote administration
5. **Password Encryption**: Enable secret and line passwords
6. **Banner Messages**: Login warnings and security notices

### Security Policies
- Console and VTY password protection
- Encrypted password storage
- Restricted inter-VLAN communication
- Firewall rules for server protection

## ⚙️ Configuration Details

### Router Configuration
```
- OSPF routing protocol (Process ID: 10)
- Inter-VLAN routing
- SSH enabled for remote access
- NAT/PAT for internet connectivity
- Static routes for WAN links
```

### Switch Configuration
```
- VLAN creation and assignment
- Trunk ports between switches
- Port security implementation
- Spanning Tree Protocol (STP)
- DHCP snooping
```

### Wireless Network
- Wireless Access Points in each department
- WPA2-PSK security
- SSID per department
- Guest network isolation

## 🧪 Testing & Validation

### Connectivity Tests
- [x] Ping test between departments
- [x] Inter-VLAN routing verification
- [x] DHCP address allocation
- [x] DNS resolution testing
- [x] HTTP/HTTPS server access
- [x] Email server functionality
- [x] Wireless connectivity

### Security Tests
- [x] VLAN isolation verification
- [x] ACL rule testing
- [x] SSH access authentication
- [x] Port security validation

## 📈 Features

- ✅ Hierarchical network design
- ✅ Multiple VLAN implementation
- ✅ OSPF dynamic routing
- ✅ Centralized DHCP services
- ✅ Web and email servers
- ✅ Wireless network integration
- ✅ WAN connectivity between branches
- ✅ SSH secure access
- ✅ Network redundancy
- ✅ Scalable architecture
-

⭐ If you found this project helpful, please consider giving it a star!
