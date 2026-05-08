<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,50:1BA0D7,100:06B6D4&height=220&section=header&text=E-Commerce%20Network&fontSize=60&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Secure%20Enterprise%20Network%20with%20AAA%20Security&descAlignY=58&descSize=18" width="100%" />
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3500&pause=800&color=06B6D4&center=true&vCenter=true&width=800&height=45&lines=Enterprise-Grade+Network+Architecture;Load-Balanced+Web+Servers+%2B+AAA+Security;VLAN+Segmentation+%2B+Layer-2+Protection;Built+with+Cisco+Packet+Tracer" alt="Typing SVG" />
</div>

<div align="center">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status" />
  <img src="https://img.shields.io/badge/Cisco-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white" alt="Cisco" />
  <img src="https://img.shields.io/badge/Network_Security-FF6B6B?style=for-the-badge" alt="Network Security" />
  <img src="https://img.shields.io/badge/AAA-4CAF50?style=for-the-badge" alt="AAA" />
  <img src="https://img.shields.io/badge/VLAN-2196F3?style=for-the-badge" alt="VLAN" />
  <img src="https://img.shields.io/badge/Team_Project-9C27B0?style=for-the-badge" alt="Team Project" />
</div>

---

## Overview

A secure, highly available enterprise network simulation built in **Cisco Packet Tracer**, designed for an e-commerce company. The network demonstrates real-world enterprise networking practices including **load balancing**, **VLAN segmentation**, **AAA authentication**, and advanced **Layer 2 security mechanisms**.

This project simulates a complete production-ready network architecture, addressing key business requirements such as high availability, network segmentation, secure internet access, and centralized management. Built as a team project under the Computer Networks course at Namal University.

---

## Project Scenario

An online e-commerce company requires a network that fulfills the following demands:

| Requirement | Description |
|-------------|-------------|
| High Availability | Uninterrupted access to website and services |
| Network Segmentation | Secure separation of internal departments |
| Internet Access | Controlled and safe outbound connectivity |
| Centralized Management | Unified authentication and network monitoring |

This project addresses all these requirements using enterprise-level networking concepts.

---

## Key Features

### 1. Load-Balanced Web Servers
- Two web servers deployed for redundancy and fault tolerance
- DNS-based load balancing ensures continuous availability
- Automatic traffic distribution between servers
- Eliminates single points of failure

### 2. FTP Server
- Dedicated FTP server for internal file management
- Secure product and content uploads
- Accessible only by authorized internal users

### 3. AAA-Based Router Authentication
- Full Authentication, Authorization, and Accounting on all routers
- Centralized authentication prevents unauthorized access
- Role-based authorization controls user privileges
- Every login attempt is tracked and logged

### 4. VLAN Segmentation
The network is logically divided into separate VLANs for each department:

| VLAN ID | Department |
|---------|------------|
| VLAN 10 | Development (Dev) |
| VLAN 20 | Human Resources (HR) |
| VLAN 30 | Sales |
| VLAN 40 | Support |

**Benefits:**
- Enhanced security between departments
- Reduced broadcast traffic
- Logical network separation

### 5. DHCP Snooping and Dynamic ARP Inspection
- DHCP Snooping prevents rogue DHCP servers
- Dynamic ARP Inspection (DAI) prevents ARP spoofing attacks
- Forms a strong Layer 2 security foundation

### 6. Network Address Translation (NAT)
- Configured for secure outbound internet traffic
- Internal private IPs translated to public IPs
- Hides internal network structure
- Enables secure outbound connectivity

### 7. Additional Features
- Port Security on switches
- Email server for internal communication
- Syslog server for centralized logging and real-time monitoring

---

## Network Topology

```
                    Internet
                       |
                       v
                  Edge Router
                  (NAT + AAA)
                       |
                       v
                  Core Switch
                  (Layer 3)
                       |
        +--------------+---------------+
        |              |               |
        v              v               v
   VLAN 10         VLAN 20          VLAN 30/40
   (Dev)           (HR)             (Sales/Support)
        |              |               |
        v              v               v
   Access Switch  Access Switch   Access Switch
   (Port Security)(Port Security) (Port Security)
        |              |               |
        v              v               v
    End Users      End Users        End Users

                Server Farm:
   +----------------+----------------+
   |                |                |
   v                v                v
Web Server 1   Web Server 2     FTP Server
(Load Bal.)    (Load Bal.)
   |                |                |
   v                v                v
Email Server   Syslog Server   Authentication
                                  Server
```

---

## Technologies Used

| Category | Technology |
|----------|------------|
| Network Simulation | Cisco Packet Tracer |
| Network Segmentation | VLANs and Inter-VLAN Routing |
| High Availability | DNS-Based Load Balancing |
| File Transfer | FTP Services |
| Access Control | AAA (Authentication, Authorization, Accounting) |
| Layer 2 Security | DHCP Snooping, Dynamic ARP Inspection |
| Internet Access | Network Address Translation (NAT) |
| Port Control | Port Security |
| Monitoring | Syslog and Email Services |
| Configuration | Cisco IOS |

---

## Security Mechanisms Implemented

### Authentication, Authorization, and Accounting (AAA)
- Centralized authentication on all routers
- Role-based authorization for different user privileges
- Comprehensive logging of all access attempts

### Layer 2 Security
- **DHCP Snooping** — Filters DHCP messages to prevent rogue servers
- **Dynamic ARP Inspection** — Validates ARP packets against trusted database
- **Port Security** — Restricts switch ports to authorized MAC addresses

### Network Segmentation
- VLAN isolation between departments
- Inter-VLAN routing with access control lists
- Reduced attack surface through segmentation

### Edge Security
- NAT hides internal network structure
- Outbound traffic filtering
- DMZ for public-facing services

---

## Project Structure

```
E-Commerce-Company-with-Load-Balanced-Web-Servers-AAA/
│
├── network_topology.pkt        # Cisco Packet Tracer file
├── configurations/             # Router and switch configs
│   ├── edge_router.txt
│   ├── core_switch.txt
│   └── vlan_configs.txt
├── documentation/              # Network design docs
│   └── architecture.md
└── README.md                   # Project documentation
```

---

## Installation and Setup

### Prerequisites

- Cisco Packet Tracer 8.0 or higher
- Basic understanding of networking concepts
- Familiarity with Cisco IOS commands

### Setup Steps

1. Clone the repository:

```bash
git clone https://github.com/MuhammadYasir85a/E-Commerce-Company-with-Load-Balanced-Web-Servers-AAA.git
```

2. Open Cisco Packet Tracer

3. Open the `.pkt` file from the repository

4. Power on all devices and observe the simulation

5. Test connectivity using ping commands across VLANs

6. Verify AAA authentication by attempting router access

---

## Verification and Testing

### Tests Performed

1. **Connectivity Testing** — Ping tests across all VLANs
2. **Load Balancing Verification** — Traffic distribution between web servers
3. **AAA Authentication** — Login attempts logged and verified
4. **VLAN Isolation** — Confirmed inter-department traffic restrictions
5. **DHCP Snooping** — Tested rogue DHCP server prevention
6. **NAT Translation** — Verified internal-to-external IP mapping
7. **Syslog Logging** — Confirmed centralized log collection

### Test Results

All services were fully implemented, rigorously tested, and verified, resulting in a secure, reliable, and highly available enterprise-level network setup.

---

## Use Cases

- E-commerce platforms requiring high availability
- Multi-department enterprise networks
- Educational reference for network security implementation
- Template for Cisco-based enterprise deployments
- Demonstration of layered security architecture

---

## Learning Outcomes

Through this project, the team gained practical understanding of:

- Enterprise-level network design and architecture
- Real-world security mechanism implementation
- High-availability systems and redundancy planning
- Network monitoring and centralized management
- Cisco IOS configuration and troubleshooting
- Team collaboration on complex networking projects

---

## Project Status

**Status:** Completed

| Task | Status |
|------|--------|
| All services implemented | Completed |
| Full network testing | Verified |
| Security mechanisms validated | Verified |
| All project requirements met | Confirmed |

---

## Academic Information

| Field | Detail |
|-------|--------|
| Course | Computer Networks |
| Institution | Namal University Mianwali |
| Instructor | Sir Shahzad Arif |
| Project Type | Team Project |

---

## Contributors

| Name | Contribution |
|------|--------------|
| **Muhammad Yasir** | Network Design, Security Implementation, Configuration |
| **Rehan Ali** | Network Design, Services Configuration, Testing |

---

## Author

**Muhammad Yasir**

Computer Science Undergraduate at Namal University Mianwali  
Aspiring AI and Computer Vision Engineer

<div>
  <a href="https://www.linkedin.com/in/muhammad-yasir-6a9500343/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:muhammadyasir85a@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://github.com/MuhammadYasir85a">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</div>

---

## Acknowledgments

- **Sir Shahzad Arif** for excellent guidance and mentorship throughout the project
- **Namal University Mianwali** for academic resources and learning environment
- **Rehan Ali** for outstanding teamwork and collaboration
- **Cisco Networking Academy** for foundational networking education

---

## License

This project is licensed under the MIT License.

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:06B6D4,50:1BA0D7,100:0F172A&height=120&section=footer" width="100%" />
</div>
