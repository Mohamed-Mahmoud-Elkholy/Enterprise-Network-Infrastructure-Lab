# Enterprise Network Infrastructure Lab

## Overview

This project demonstrates the design and implementation of a complete Enterprise Network Infrastructure using Cisco IOS devices in GNS3 and Windows Server 2019.

The lab simulates a real-world enterprise environment with multiple departments, dynamic routing, gateway redundancy, centralized DHCP services, network security policies, and Internet connectivity.

---

# Network Topology

![Topology](Topology/Topology.png)

---

# Technologies Used

- Cisco IOS
- GNS3
- VMware Workstation
- Windows Server 2019

---

# Implemented Features

- VLAN Segmentation
- Inter-VLAN Routing
- VTP
- Spanning Tree Protocol (STP)
- EtherChannel
- HSRP
- OSPF
- NAT Overload (PAT)
- Windows Server DHCP
- DHCP Relay (IP Helper)
- Extended ACLs

---

# VLAN Information

| VLAN | Name | Subnet |
|------|------|---------|
|10|HR|192.168.0.0/26|
|20|Finance|192.168.0.64/27|
|30|IT|192.168.0.96/28|
|40|Servers|192.168.0.112/28|
|50|Wireless|192.168.0.128/29|
|60|Management|192.168.0.136/29|

---

# High Availability

Implemented using **HSRP** between two Multilayer Switches.

Features:

- Active / Standby Gateway
- Gateway Redundancy
- Automatic Failover
- Preemption

---

# Dynamic Routing

Configured using **OSPF**.

Features:

- Dynamic Route Exchange
- Fast Convergence
- Redundant Paths

---

# DHCP

Windows Server 2019 provides:

- Centralized DHCP Service
- Multiple DHCP Scopes
- DHCP Relay using IP Helper Address

---

# NAT

Configured PAT (NAT Overload) to provide Internet connectivity for all internal VLANs.

---

# Security

Implemented Extended ACLs to control communication between departments while allowing access to required enterprise services.

---

# Validation

The following tests were successfully completed:

- DHCP Lease Assignment
- Inter-VLAN Routing
- HSRP Failover
- OSPF Neighbor Adjacency
- NAT Internet Access
- ACL Verification

---

# Project Structure

```
Configurations/
GNS3-Project/
Topology/
Verification/
Windows-Server/
```

---

# Author

**Mohamed Mahmoud Elkholy**

Aspiring Network Engineer
