# 🌐 Enterprise Network Infrastructure – Cisco Packet Tracer Project
This repository contains a complete Cisco Packet Tracer simulation project created for an academic infrastructure assignment. The project demonstrates a secure, scalable enterprise network using real-world design principles, incorporating multiple sites, dynamic routing, VLAN segmentation, tunneling, and network services.

## 🧰 Project Summary
The network is designed to simulate a small-to-medium-sized organization with three physical locations:

🏢 Main Office

🏢 Branch A

🏢 Branch B

Each site includes its own Layer 2 and Layer 3 infrastructure, user endpoints, and core services. The locations are interconnected using secure GRE over IPsec tunnels and configured under a unified routing domain using OSPF (Single Area).

## 🗺️ Topology Overview

![Network Topology](topology.png)

Physical Topology
🔹 Three enterprise sites (1 main, 2 branches)

🔹 Main Site contains:

1 Layer 3 switch (Distribution layer)

2 Access switches

2 VLANs 

1 PC per VLAN

🔹 Each branch contains:

1 Layer 3 switch (Distribution layer)

2 VLANs 

1 PC (Dev VLAN`s)

🔹 Each Distribution switch connects to the internet

🔹 All sites linked via Layer 3 routed ports

🔹 Proper port assignments and naming conventions used

## Logical Topology
## 🔐 Hub-and-Spoke GRE over IPsec Tunnels between the main office (hub) and branches (spokes)

## 🛰️ OSPF Single Area Routing for internal dynamic routing

## 🌐 Internet simulation via an L3 device (not used for OSPF)

## 🧩 VLAN segmentation per site, including an IT department VLAN

## 🔐 SSH access configured for remote management

## 🧠 DHCP configured per site to auto-assign IP addresses to clients

## ⚙️ Best practices implemented according to cybersecurity and networking standards taught in the course

## 🔐 Security Implementation
Security configurations follow industry best practices covered in the curriculum, such as:

Encrypted remote access using SSH

IPsec tunnel encryption for secure WAN communication

VLAN segmentation for isolating departments

Minimal open ports and secure device configurations

## 📂 Project Files
enterprise_network.pkt – Main Cisco Packet Tracer file

## 🔧 How to Use
First password to enter the user mode:Aa123456
Second password to access the privilege mode:Bb123456
Open the .pkt file using Cisco Packet Tracer 8.2 or later
Observe the topology and explore each device’s CLI
The lab itself might not work properly due to bugs, but all configurations were tested and worked successfully before publishing.
