# E-Commerce Enterprise Network

### Load-Balanced Web Servers & AAA Security

A secure, highly available enterprise network simulation built in Cisco Packet Tracer, featuring load balancing, VLAN segmentation, AAA authentication, and advanced Layer 2 security mechanisms.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Project Scenario](#project-scenario)
3. [Core Features](#core-features)
4. [Additional Features](#additional-features)
5. [Technologies Used](#technologies-used)
6. [Team Members](#team-members)
7. [Academic Information](#academic-information)
8. [Project Status](#project-status)
9. [Learning Outcomes](#learning-outcomes)
10. [License](#license)

---

## Project Overview

This project demonstrates the design and implementation of a secure, highly available enterprise network for a simulated e-commerce company.

Built following real-world networking practices, the network incorporates:

- High availability through redundant systems
- Secure network segmentation
- Centralized authentication and monitoring
- Comprehensive Layer 2 and Layer 3 security

Developed as part of the **Computer Networks** course at **Namal University**, under the guidance of **Sir Shehzad Arif**.

---

## Project Scenario

An online e-commerce company requires a network that fulfills the following demands:

| Requirement | Description |
|-------------|-------------|
| High Availability | Uninterrupted access to website and services |
| Network Segmentation | Secure separation of internal departments |
| Internet Access | Controlled and safe outbound connectivity |
| Centralized Management | Unified authentication and network monitoring |

This project fulfills all these requirements using enterprise-level networking concepts.

---

## Core Features

### 1. Load-Balanced Web Servers

Two web servers are deployed to ensure redundancy and fault tolerance.

- DNS-based load balancing ensures continuous availability
- Automatic traffic distribution between servers
- Eliminates single points of failure

### 2. FTP Server

A dedicated FTP server handles all internal file management.

- Used for secure product and content uploads
- Accessible only by authorized internal users
- Enforces controlled file management

### 3. AAA-Based Router Authentication

Full Authentication, Authorization, and Accounting implemented across all routers.

- Centralized authentication prevents unauthorized access
- Role-based authorization controls user privileges
- Every login attempt is tracked and logged

### 4. VLAN Segmentation

The network is logically divided into separate VLANs for each department.

| VLAN ID | Department |
|---------|------------|
| VLAN 10 | Development (Dev) |
| VLAN 20 | Human Resources (HR) |
| VLAN 30 | Sales |
| VLAN 40 | Support |

**Key Benefits:**

- Enhanced security between departments
- Reduced broadcast traffic
- Logical network separation

### 5. DHCP Snooping & Dynamic ARP Inspection

Layer 2 security is enforced through two complementary mechanisms.

- **DHCP Snooping** prevents rogue DHCP servers
- **Dynamic ARP Inspection (DAI)** prevents ARP spoofing attacks
- Forms a strong Layer 2 security foundation

### 6. Network Address Translation (NAT)

NAT is configured to manage outbound internet traffic securely.

- Internal private IPs translated to public IPs
- Hides internal network structure
- Enables secure outbound connectivity

---

## Additional Features

| Feature | Description |
|---------|-------------|
| Port Security | Restricts switch ports to authorized devices only |
| Email Server | Manages internal and external communication |
| Syslog Server | Centralized logging and real-time monitoring |

---

## Technologies Used

| Category | Technology |
|----------|-----------|
| Network Segmentation | VLANs & Inter-VLAN Routing |
| High Availability | DNS-Based Load Balancing |
| File Transfer | FTP Services |
| Access Control | AAA (Authentication, Authorization, Accounting) |
| Layer 2 Security | DHCP Snooping & Dynamic ARP Inspection |
| Internet Access | Network Address Translation (NAT) |
| Port Control | Port Security |
| Monitoring | Syslog & Email Services |
| Configuration | Cisco IOS |

---

## Team Members

| Name | Contribution |
|------|-------------|
| **Muhammad Yasir** | Network Design, Security Implementation & Configuration |
| **Rehan Ali** | Network Design, Services Configuration & Testing |

---

## Academic Information

| Field | Detail |
|-------|--------|
| Course | Computer Networks |
| Institution | Namal University |
| Instructor | Sir Shehzad Arif |

---

## Project Status

| Task | Status |
|------|--------|
| All services implemented | Completed |
| Full network testing | Verified |
| Security mechanisms validated | Verified |
| All project requirements met | Confirmed |

---

## Learning Outcomes

Through this project, we gained practical understanding of:

- Enterprise-level network design and architecture
- Real-world security mechanisms implementation
- High-availability systems and redundancy planning
- Network monitoring and centralized management
- Cisco IOS configuration and troubleshooting

---

## License

This project is licensed under the **MIT License**.
