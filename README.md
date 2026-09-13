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
---

## 🚀 Key Objectives & Capabilities
* **Network Enumeration & Scanning:** Discovering live hosts and open ports across internal targets using Kali Linux.
* **Endpoint Analysis:** Assessing Windows-based operating system behaviors and security controls.
* **Safe Environment Isolation:** Maintaining a secure, air-gapped virtual network to practice offensive techniques without risk.

---

## 🛠️ Documentation & Engineering Logs
* [Architecture & Design Details](docs/architecture.md)
* [Step-by-Step Lab Setup Guide](docs/lab-setup-guide.md)
* [Troubleshooting & Engineering Hurdles](docs/troubleshooting.md)

---
## 📸 Lab Preview
<img width="1898" height="1102" alt="Screenshot 2026-09-13 033949" src="https://github.com/user-attachments/assets/4a9de0d6-051c-4626-bed4-4ecf989aecc8" />

<img width="1337" height="935" alt="Screenshot 2026-09-13 011540" src="https://github.com/user-attachments/assets/58317634-51ee-44eb-b41e-07e79f15cb71" />


<img width="1767" height="1158" alt="Screenshot 2026-09-12 221801" src="https://github.com/user-attachments/assets/4c430af6-c5b2-4557-a487-52dbc0bed69b" />


