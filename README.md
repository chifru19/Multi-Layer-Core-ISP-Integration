
# Corporate Network Lab V1

## Project Overview
This project demonstrates a secure corporate network design using Cisco Packet Tracer.

## Security Features Implemented
* **Secret Passwords**: Encrypted privileged access.
* **Routing**: Static routing configured between corporate subnets.
* **Configuration Backups**: Plain-text configuration files stored for auditing purposes.

## Folder Structure
* `/Topology`: Cisco Packet Tracer (.pkt) source files.
* `/Configs`: Exported device configurations.
* `/Docs`: Technical documentation and proof of connectivity.
=======
# Corporate-Network-Lab: Multi-Layer Core & ISP Integration

A full-stack enterprise network simulation built in Cisco Packet Tracer featuring a redundant core, wireless segmentation, and external web services.

## 🚀 Features
* **Redundant Core:** Two 3650 Multilayer Switches connected via EtherChannel (LACP) for high-speed link aggregation.
* **VLAN Segmentation:**
    * VLAN 10 (Wired): 10.1.10.0/24
    * VLAN 20 (Wired): 10.1.20.0/24
    * VLAN 30 (Wireless): 10.1.30.0/24 (DHCP served by Core Switch)
* **Layer 3 Routing:** Inter-VLAN routing configured on the Core Switch using SVIs.
* **Edge Connectivity:** Routed port connection to a 2911 Edge Router using a /30 subnet.
* **Public Services:** Simulated Internet hosting a Web Server (8.8.8.8) with DNS resolution (www.lab.com).
* **Hardened Security:** SSHv2 management, encrypted passwords, and protected 'Enable' secrets.

## 🛠️ Key Commands
### Password Encryption
```bash
service password-encryption  # Scrambles plain-text passwords in config
>>>>>>> 58e3f12ed92dee21d97bb27e0353637f3e0d38aa
