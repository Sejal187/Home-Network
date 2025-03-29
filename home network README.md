# Home Network Documentation

This repository contains the documentation for the setup, configuration, and security of my home network.

## Contents:
- Physical Topology
- Logical Topology
- Device Information
- IP Addressing Scheme
- Configuration Backup Methods
- Security Practices for Credential Management

Feel free to explore the sections to understand how the network is structured.

---

# Physical Topology

This section describes the physical setup of the home network.

## Devices and Locations:
1. **Router** (Living Room) - Connected to the internet via WAN port.
2. **Switch** (Home Office) - Connected to the router, providing connections to multiple devices.
3. **Laptop** (Bedroom) - Connected to the router via Wi-Fi.
4. **Printer** (Living Room) - Connected to the switch via Ethernet.

## Cabling:
- **Router to Switch**: Ethernet Cable (Cat6)
- **Switch to Printer**: Ethernet Cable (Cat6)
- **Switch to Laptop**: Wi-Fi (802.11ac)

## Diagram:
![image](https://github.com/user-attachments/assets/0eacf66b-2735-4d25-8d3a-dfdf2172b1a4)


---

# Logical Topology

This section covers the logical network configuration.

## IP Addressing:
- **Router (WAN)**: 192.168.1.1
- **Router (LAN)**: 192.168.0.1
- **Laptop**: 192.168.0.101 (Static IP)
- **Printer**: 192.168.0.102 (Static IP)

## Diagram:
![Screenshot 2025-03-28 201517](https://github.com/user-attachments/assets/d02ff3f0-a5c1-4220-a067-ad6e6f93b969)

## Network Segmentation:
- **Main Network (192.168.0.x)**: Devices like laptop, printer, etc.
- **Guest Network (192.168.1.x)**: Used for guest devices.

## Routing:
- **Inter-VLAN Routing**: Configured to allow communication between main network and guest network.

---

# Device Information

## Router:
- **Model**: TP-Link Archer C7
- **Firmware Version**: 1.5.0
- **Interfaces**: 4x Ethernet, 1x WAN, Wi-Fi
- **IP Address**: 192.168.0.1

## Switch:
- **Model**: Netgear GS108
- **Ports Used**: Ports 1-5 for devices, Port 8 to router

## Laptop:
- **Model**: Dell XPS 13
- **Operating System**: Windows 11
- **IP Address**: 192.168.0.101

---

# Addressing Documentation

## IP Scheme:
- **Router**: 192.168.0.1 (Static)
- **Laptop**: 192.168.0.101 (Static)
- **Printer**: 192.168.0.102 (Static)
- **DHCP Range**: 192.168.0.100 to 192.168.0.199

## Subnet Mask:
- **Subnet**: 255.255.255.0

---

# Configuration Backup

- **Router**: Configurations are backed up to a cloud service (Google Drive).
- **Switch**: No backup necessary as it uses default configurations.
- **Laptop**: Configurations are backed up using Windows File History and OneDrive.

---

# Security

## Password Manager:
- **Tool**: 1Password
- **Encryption**: AES-256 encryption is used to securely store login credentials.

## Two-Factor Authentication:
- **Enabled on Router**: 2FA enabled for router admin interface.
- **VPN**: 2FA is enabled for remote access VPN.

---

# Change Log

- **March 25, 2025**: Updated router firmware to version 1.5.0.
- **March 20, 2025**: Added a printer to the network, assigned IP 192.168.0.102.
