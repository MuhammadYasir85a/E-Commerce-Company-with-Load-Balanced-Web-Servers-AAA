# E-Commerce-Company-with-Load-Balanced-Web-Servers-AAA
Project Overview
This project demonstrates the design and implementation of a secure, highly available enterprise network for a simulated e-commerce company. Built following real-world networking practices, the network incorporates high availability, network segmentation, centralized authentication, and comprehensive monitoring.

Developed as part of the Computer Networks course at Namal University, under the guidance of Sir Shehzad Arif.

Project Scenario
An online e-commerce company requires:

High availability for its website and services
Secure internal network segmentation
Controlled and safe internet access
Centralized authentication and network monitoring
This project fulfills all these requirements using enterprise-level networking concepts and configurations.

Core Features Implemented
Load-Balanced Web Servers
Two web servers deployed for redundancy and fault tolerance
DNS-based load balancing ensures continuous high availability
Automatic traffic distribution between servers prevents single points of failure
FTP Server
Dedicated FTP server for secure product and content uploads
Accessible only by authorized internal users
Enforces controlled file management across the organization
AAA-Based Router Authentication
Full Authentication, Authorization, and Accounting (AAA) implemented on routers
Centralized authentication prevents unauthorized administrative access
Every login attempt is tracked and logged for accountability
VLAN Segmentation
Separate VLANs created for different departments:

VLAN	Department
VLAN 10	Development (Dev)
VLAN 20	Human Resources (HR)
VLAN 30	Sales
VLAN 40	Support
Benefits:

Enhanced security between departments
Reduced broadcast traffic
Logical and clean network separation
DHCP Snooping & Dynamic ARP Inspection (DAI)
DHCP Snooping prevents rogue DHCP servers from distributing malicious configurations
Dynamic ARP Inspection (DAI) protects against ARP spoofing and poisoning attacks
Together these significantly strengthen Layer 2 security
Network Address Translation (NAT)
Internal private IP addresses translated to public IPs for internet access
Hides the internal network structure from external entities
Enables secure and controlled outbound internet connectivity
Additional Features
Feature	Purpose
Port Security	Limits unauthorized device connections on switch ports
Email Server	Handles internal and external organizational communication
Syslog Server	Centralized logging for real-time monitoring and auditing
Technologies & Concepts Used
VLANs & Inter-VLAN Routing
DNS-Based Load Balancing
FTP Services
AAA — Authentication, Authorization & Accounting
DHCP Snooping
Dynamic ARP Inspection (DAI)
Network Address Translation (NAT)
Port Security
Syslog & Email Services
Cisco IOS Configuration
Team Members
Name	Role
Muhammad Yasir	Network Design, Security Implementation & Configuration
Rehan Ali	Network Design, Services Configuration & Testing
Academic Information
Course	Computer Networks
Institution	Namal University
Instructor	Sir Shehzad Arif
Project Status
Task	Status
All services implemented	Complete
Full network testing	Verified
Security mechanisms validated	Verified
All project requirements met	Confirmed
Learning Outcomes
Through this project, we gained:

Hands-on experience with enterprise network design
Practical implementation of real-world security mechanisms
Deep understanding of high-availability systems
Real-world exposure to network monitoring and management
Proficiency in Cisco IOS configuration and troubleshooting
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

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the project.

THE PROJECT IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
