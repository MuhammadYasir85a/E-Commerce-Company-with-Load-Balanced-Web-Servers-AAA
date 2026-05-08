E-Commerce Enterprise Network
Load-Balanced Web Servers & AAA Security
A secure, highly available enterprise network simulation built in Cisco Packet Tracer, featuring load balancing, VLAN segmentation, AAA authentication, and advanced Layer 2 security mechanisms.

<br>
Table of Contents
Project Overview
Project Scenario
Core Features
Additional Features
Technologies Used
Team Members
Academic Information
Project Status
Learning Outcomes
License
<br>
Project Overview
This project demonstrates the design and implementation of a secure, highly available enterprise network for a simulated e-commerce company.

Built following real-world networking practices, the network incorporates:

High availability through redundant systems
Secure network segmentation
Centralized authentication and monitoring
Comprehensive Layer 2 and Layer 3 security
Developed as part of the Computer Networks course at Namal University, under the guidance of Sir Shehzad Arif.

<br>
Project Scenario
An online e-commerce company requires a network that fulfills the following demands:

Requirement	Description
High Availability	Uninterrupted access to website and services
Network Segmentation	Secure separation of internal departments
Internet Access	Controlled and safe outbound connectivity
Centralized Management	Unified authentication and network monitoring
This project fulfills all these requirements using enterprise-level networking concepts and configurations.

<br>
Core Features
<br>
1. Load-Balanced Web Servers
Two web servers are deployed to ensure redundancy and fault tolerance across the network.

DNS-based load balancing ensures continuous high availability
Automatic traffic distribution between servers
Eliminates single points of failure for the web service
<br>
2. FTP Server
A dedicated FTP server handles all internal file and content management.

Used for secure product and content uploads
Accessible only by authorized internal users
Enforces controlled file management across the organization
<br>
3. AAA-Based Router Authentication
Full Authentication, Authorization, and Accounting implemented across all routers.

Centralized authentication prevents unauthorized administrative access
Role-based authorization controls what each user can access
Every login attempt is tracked and logged for full accountability
<br>
4. VLAN Segmentation
The network is logically divided into separate VLANs for each department.

VLAN ID	Department
VLAN 10	Development (Dev)
VLAN 20	Human Resources (HR)
VLAN 30	Sales
VLAN 40	Support
Key Benefits:

Enhanced security between departments
Reduced broadcast traffic across the network
Clean and logical network separation
<br>
5. DHCP Snooping & Dynamic ARP Inspection
Layer 2 security is enforced through two complementary mechanisms.

DHCP Snooping prevents rogue DHCP servers from distributing malicious network configurations
Dynamic ARP Inspection (DAI) protects against ARP spoofing and ARP poisoning attacks
Together these mechanisms form a strong Layer 2 security foundation
<br>
6. Network Address Translation (NAT)
NAT is configured to manage outbound internet traffic securely.

Internal private IP addresses are translated to public IPs for internet access
Hides the internal network structure from external entities
Enables secure and controlled outbound internet connectivity
<br>
Additional Features
<br>
Feature	Description
Port Security	Restricts switch ports to authorized devices only, preventing unauthorized access
Email Server	Manages internal and external organizational communication
Syslog Server	Provides centralized logging for real-time monitoring and auditing
<br>
Technologies Used
<br>
Category	Technology / Concept
Network Segmentation	VLANs & Inter-VLAN Routing
High Availability	DNS-Based Load Balancing
File Transfer	FTP Services
Access Control	AAA — Authentication, Authorization & Accounting
Layer 2 Security	DHCP Snooping & Dynamic ARP Inspection (DAI)
Internet Access	Network Address Translation (NAT)
Port Control	Port Security
Monitoring	Syslog & Email Services
Device Configuration	Cisco IOS
<br>
Team Members
<br>
Name	Contribution
Muhammad Yasir	Network Design, Security Implementation & Configuration
Rehan Ali	Network Design, Services Configuration & Testing
<br>
Academic Information
<br>
Field	Detail
Course	Computer Networks
Institution	Namal University
Instructor	Sir Shehzad Arif
<br>
Project Status
<br>
Task	Status
All services implemented	Completed
Full network testing	Verified
Security mechanisms validated	Verified
All project requirements met	Confirmed
<br>
Learning Outcomes
Through this project, we gained practical and theoretical understanding of the following areas:

Hands-on experience with enterprise-level network design and architecture
Practical implementation of real-world security mechanisms
Deep understanding of high-availability systems and redundancy planning
Real-world exposure to network monitoring and centralized management
Proficiency in Cisco IOS configuration and troubleshooting
<br>
License
text

MIT License

Copyright (c) 2025 Muhammad Yasir & Rehan Ali

Permission is hereby granted, free of charge, to any person obtaining a copy
of this project and associated documentation files, to deal in the project
without restriction, including without limitation the rights to use, copy,
modify, merge, publish, distribute, sublicense, and/or sell copies of the
project, and to permit persons to whom the project is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the project.

THE PROJECT IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE PROJECT OR THE USE OR OTHER DEALINGS
IN THE PROJECT.
This project was developed for academic and learning purposes as part of the Computer Networks curriculum at Namal University.

<br> <br>
