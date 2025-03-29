# Home Network Documentation

- **Date: 29th March 2025**
- **Written by: Sejalpreet Kaur**

This repository contains the documentation for the setup, configuration, and security of my home network.

## Contents:
- Physical Topology
- Logical Topology
- Device Information
- IP Addressing Scheme
- Configuration Backup Methods

Feel free to explore the sections to understand how the network is structured.

---

# Physical Topology

The physical topology represents the actual arrangement of networking devices in the home environment. Below is a detailed layout of device locations, connections, and cabling:

### Devices and Locations:
- **Router (ISR4331)** - Located in Study Room
- **Switch (2960-24TT)** - Connected to the Router, located in Study Room
- **Access Point** - Located centrally for optimal wireless coverage
- **PC (PC-PT)** - Study Room, wired to Switch
- **Laptop (Laptop-PT)** - Study Room, wired to Switch
- **Printer (Printer-PT)** - Study Room, wired to Switch
- **Tablet (TabletPC-PT)** - Wireless connection via Access Point
- **Smartphones (SMARTPHONE-PT)** - Connected wirelessly via Access Point

## Cabling:
- **Router to Switch**: Ethernet Cable (Cat6)
- **Switch to Printer**: Ethernet Cable (Cat6)
- **Switch to Laptop**: Wi-Fi (802.11ac)

## Diagram:
![image](https://github.com/user-attachments/assets/0eacf66b-2735-4d25-8d3a-dfdf2172b1a4)


---

# Logical Topology

The logical topology describes the data flow and network communication structure. Below is the logical representation of the network:

### IP Addressing Scheme:
- **Router (ISR4331)**: `192.168.1.1/24` (Gateway, DHCP Server)
- **Switch (2960-24TT)**: `192.168.1.10/24`
- **Access Point**: `192.168.1.3/24`
- **PC (PC-PT)**: `192.168.1.2/24`
- **Laptop (Laptop-PT)**: `192.168.1.5/24`
- **Printer (Printer-PT)**: `192.168.1.4/24`
- **Tablet (TabletPC-PT)**: DHCP assigned
- **Smartphones (SMARTPHONE-PT)**: DHCP assigned

### DHCP Configuration:
The router is responsible for assigning IP addresses dynamically to wireless devices and other DHCP-configured clients.

### Default Gateway:
All devices use `192.168.1.1` as their default gateway to access external networks.

## Diagram:
![Screenshot 2025-03-28 201517](https://github.com/user-attachments/assets/d02ff3f0-a5c1-4220-a067-ad6e6f93b969)

---

## Device Information

### **Router: Cisco ISR4331**
- **Brand:** Cisco
- **Model:** ISR4331
- **Qualities:**
  - Provides internet access and serves as the network's gateway.
  - Functions as the DHCP server, firewall, and NAT device.
  - Connected to ISP modem and the main switch.
  - Supports advanced security features and VPN connectivity.

### **Switch: Cisco 2960-24TT**
- **Brand:** Cisco
- **Model:** 2960-24TT
- **Qualities:**
  - 24-port managed switch for wired network expansion.
  - Connects wired devices (PC, Laptop, Printer, Access Point).
  - Provides VLAN support and traffic management.

### **Access Point**
- **Brand:** Ubiquiti UniFi AP
- **Model:** UAP-AC-LR
- **Qualities:**
  - Extends Wi-Fi coverage to wireless devices.
  - Uses WPA3 encryption for security.
  - Connected to the switch via Ethernet.

### **PC (PC-PT)**
- **Usage:** Work, gaming, and network administration.
- **Static IP:** `192.168.1.2`

### **Laptop (Laptop-PT)**
- **Usage:** Browsing, remote work, and multimedia tasks.
- **Static IP:** `192.168.1.5`

### **Printer (Printer-PT)**
- **Usage:** Shared across the network for printing needs.
- **Static IP:** `192.168.1.4`

### **Tablet (TabletPC-PT)**
- **Connection:** Wireless via Access Point
- **IP Assignment:** DHCP
- **Usage:** Reading, streaming, and remote access.

### **Smartphones (SMARTPHONE-PT)**
- **Connection:** Wireless via Access Point
- **IP Assignment:** DHCP
- **Usage:** Communication, browsing, and smart home control.

---

## Device Configuration & Security
- **Router and Switch configurations** are backed up regularly.
- **Access credentials** are securely stored in a password manager.
- **Wireless Security:** WPA3 encryption is enabled.
- **MAC Filtering** is enabled for additional access control.

---

## Backup & Maintenance
- Configurations are backed up to a secure cloud repository.
- Regular firmware updates are applied to all devices.
- Logs are monitored for suspicious activity.

---

## Change Log

- **March 25, 2025**: Updated router firmware to version 1.5.0.

