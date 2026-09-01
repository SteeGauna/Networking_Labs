# Network Engineering Labs & Projects

Welcome to my network engineering repository.

This repository contains my hands-on networking labs, configurations, troubleshooting exercises, network automation projects, and technical experiments. It is a collection of practical work that I use to develop and demonstrate my skills in network engineering.

The repository will continue to grow as I progress from foundational networking concepts into advanced routing, switching, automation, and network programmability.

# Purpose

The purpose of this repository is to document my practical development as a network engineer.

Rather than only studying networking concepts theoretically, I use these labs and projects to build, configure, test, break, troubleshoot, and automate networks.

The repository serves as:

* A personal networking laboratory
* A record of my learning and development
* A reference for future projects
* A collection of reusable configurations and scripts
* A portfolio demonstrating practical networking skills

---

# Networking Labs

The networking sections contain simulated network environments and configurations covering a range of networking technologies.

Labs may include:

* IPv4 and IPv6
* VLANs
* 802.1Q trunking
* Inter-VLAN routing
* STP / RSTP
* EtherChannel
* Static routing
* OSPF
* OSPF multi-area
* Route summarization
* Route redistribution
* BGP
* ACLs
* DHCP
* NAT
* Network security
* High availability
* Network troubleshooting

Most labs are built using Cisco Packet Tracer, with additional technologies and platforms added as the laboratory environment develops.

---

# Lab Documentation

Each major lab is documented where possible with:

```text
Lab/
├── lab.pkt
├── README.md
├── topology.png
└── configs/
    ├── R1.txt
    ├── R2.txt
    └── R3.txt
```

The documentation may include:

* Lab objectives
* Network topology
* IP addressing
* Device configurations
* Configuration commands
* Verification commands
* Expected results
* Troubleshooting steps
* Problems encountered
* Solutions
* Lessons learned

---

# Troubleshooting

Networking is not only about configuring devices correctly. A major part of network engineering is understanding what happens when something doesn't work.

The troubleshooting section contains intentionally broken or failed configurations and documents the process used to identify and resolve the problem.

Examples may include:

* OSPF neighbor failures
* Incorrect VLAN configuration
* Trunking problems
* STP issues
* Routing problems
* Incorrect IP addressing
* ACL blocking traffic
* Layer 2 vs Layer 3 connectivity problems
* Interface failures
* Gateway and routing issues

The goal is to document not only **what fixed the problem**, but also **how the problem was identified**.

---

# Network Automation

As my networking knowledge develops, this repository also contains projects focused on network automation and programmability.

Technologies and tools include:

* Python
* Netmiko
* REST APIs
* RESTCONF
* NETCONF
* Ansible
* JSON
* YAML
* Network device APIs

Example automation projects may include:

```text
Network-Automation/
│
├── Python/
│   ├── device_inventory/
│   ├── configuration_backup/
│   └── network_information/
│
├── Netmiko/
│   ├── device_backup/
│   └── configuration_deployment/
│
├── NETCONF/
│
├── RESTCONF/
│
└── Ansible/
```

The objective is to move beyond manually configuring individual network devices and develop systems capable of managing networks programmatically.

---

# Projects

The Projects section contains larger practical implementations that combine multiple networking concepts.

Projects may involve:

* Network design
* Routing and switching
* Network security
* Automation
* Monitoring
* Configuration management
* APIs
* Infrastructure management

These projects are intended to demonstrate how individual networking concepts can be combined into a complete solution.

---

# Learning Progression

This repository represents an ongoing learning journey.

The progression is broadly:

```text
Networking Fundamentals
        ↓
CCNA-Level Networking
        ↓
Advanced Routing & Switching
        ↓
CCNP-Level Technologies
        ↓
Network Automation
        ↓
Network Programmability
        ↓
Advanced Network Engineering
```

New labs and projects will be added as new technologies and concepts are studied and implemented.

---

# Technologies

### Networking

* Cisco IOS
* Cisco Packet Tracer
* IPv4
* IPv6
* VLAN
* STP / RSTP
* OSPF
* BGP
* ACL
* DHCP
* NAT
* EtherChannel

### Automation & Programming

* Python
* Netmiko
* NETCONF
* RESTCONF
* REST APIs
* Ansible
* JSON
* YAML

### Tools

* Git
* GitHub
* Visual Studio Code
* Cisco Packet Tracer

---

# Documentation Philosophy

For each lab, I aim to document three things:

### 1. Build

How the network was designed and configured.

### 2. Verify

How the configuration was tested and how successful operation was confirmed.

### 3. Troubleshoot

What happened when something didn't work, how the problem was investigated, and how it was resolved.

This approach is intended to develop practical troubleshooting and engineering skills rather than relying solely on memorizing configuration commands.

---

# Future Development

This repository will continue to evolve as I develop my networking and automation skills.

Future areas may include:

* Advanced BGP
* Advanced OSPF
* Network security
* Network monitoring
* Infrastructure automation
* Configuration management
* SD-WAN
* Network programmability
* Linux networking
* Virtual networking
* Network APIs
* Cloud networking
* Infrastructure as Code

---

## Disclaimer

The configurations and topologies in this repository are primarily created for educational, laboratory, and testing purposes.

Configurations should be reviewed and adapted before being used in production environments.

---

## About

This repository represents my ongoing practical development in network engineering, with an emphasis on networking fundamentals, advanced routing and switching, troubleshooting, automation, and network programmability.

**This is a living repository and will continue to evolve as I learn, build, troubleshoot, and automate.**
