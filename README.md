# Implementation of WAN PPP and Enterprise Network Technologies Using EVE-NG

## 📄 Overview
This project simulates the deployment of an enterprise-level network using **EVE-NG (Emulated Virtual Environment - Next Generation)**. It includes a full implementation of **WAN PPP**, advanced **switching and routing technologies**, **security features**, and **network services**.

The lab replicates a real-world enterprise environment for testing, training, and proof-of-concept purposes, using Cisco IOS devices in a virtual setting.

---

## 🎯 Objectives
- Build a full enterprise network architecture using EVE-NG.
- Implement WAN PPP links with authentication protocols.
- Configure Layer 2 and Layer 3 technologies including VLANs, BGP, and inter-VLAN routing.
- Apply network security and optimization features.
- Deploy DHCP and Web network services.

---

## 🧰 Technologies Implemented

### 📡 WAN & Routing
- **WAN PPP Configuration** (with PAP/CHAP authentication)
- **BGP (Border Gateway Protocol)**
- **HSRP (High Availability Routing)**

### 🔌 Switching & Layer 2
- **VLAN Configuration** (Access and Trunk ports)
- **VTP (VLAN Trunking Protocol)**
- **PAgP (Port Aggregation Protocol)**
- **SVI (Switch Virtual Interface)**

### 🔐 Security Features
- **DHCP Snooping**
- **ARP Inspection (DAI)**
- **ACLs (Access Control Lists)**
- **Port Security**

### 🌐 Network Services
- **NAT (Network Address Translation)**
- **DHCP Server Implementation**
- **Web Server Configuration (Basic HTTP Service)**

### ⚙️ Performance Optimization
- **QoS (Quality of Service)**
- Interface Settings: Bandwidth, Delay, Clock Rate

---

## 🏗️ Network Topology
- Cisco routers connected over serial WAN links (PPP)
- Layer 2/3 switches for campus and data center simulation
- PCs and servers for service testing
- Internet simulation via NAT and web server

> *Add topology diagram here if available*

---

## ✅ Sample Configurations

### PPP with CHAP
```bash
interface Serial0/0
  encapsulation ppp
  ip address 10.10.10.1 255.255.255.252
  clock rate 64000
  ppp authentication chap
