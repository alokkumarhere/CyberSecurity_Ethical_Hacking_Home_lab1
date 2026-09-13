# 🏛️ Lab Architecture & Network Topology

## Design Goals
The primary objective of this architecture is to create a closed, safe, and repeatable testing ground for offensive security concepts, network mapping, and endpoint behavior analysis.

## Network Topology & Isolation
* **Hypervisor Layer:** Oracle VirtualBox running on the host system.
* **Virtual Switch / Network:** A dedicated **NAT Network** (`Lab-Network`) configured with internal DHCP.
* **Security Boundary:** 
  * Virtual machines can communicate with each other freely for multi-node attack and defense simulation.
  * The network is isolated from the physical home router/LAN, preventing accidental exposure of vulnerable endpoints.

## Node Specifications
| Node Name | Role | OS / Version | RAM Allocation | Virtual Disks | Network Configuration |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Kali-Linux** | Attacker / Operator | Kali Linux (Latest - Xfce) | 4GB - 8GB | 80GB (Dynamic) | NAT Network (Adapter 1) |
| **V1_Win10** | Victim Endpoint | Windows 10 Pro | 4GB | 80GB (Dynamic) | NAT Network (Adapter 1) |
| **V2_Win11** | Victim Endpoint | Windows 11 Pro | 4GB - 8GB | 80GB (Dynamic) | NAT Network (Adapter 1) |
