# 🛡️ Enterprise-Grade Cybersecurity & Ethical Hacking Home Lab

A fully isolated, multi-node virtualized cybersecurity laboratory built using Oracle VirtualBox, Kali Linux, and Windows target endpoints. Designed for safe penetration testing, vulnerability assessment, network enumeration, and defensive security research.

---

## 🏗️ Lab Architecture & Topology

The lab is hosted locally on a hypervisor with strict network isolation to prevent any accidental exposure to the local home network or public internet.

* **Hypervisor:** Oracle VirtualBox
* **Attacker Node:** Kali Linux (Latest - Xfce Desktop) with comprehensive offensive toolsets.
* **Victim Node 1:** Windows 10 Pro (Isolated endpoint target)
* **Victim Node 2:** Windows 11 Pro (Isolated endpoint target with hardware bypass configuration)
* **Networking:** Dedicated private **NAT Network** with DHCP enabled for secure inter-VM communication.
