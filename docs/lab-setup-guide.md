# 🛠️ Step-by-Step Lab Provisioning Guide

Follow this guide to replicate or rebuild the cybersecurity home lab environment.

## Phase 1: Hypervisor & Network Configuration
1. Install **Oracle VirtualBox** on your host machine.
2. Navigate to **File > Preferences > Network**.
3. Create a new **NAT Network** (e.g., named `Lab-Network`) and ensure **Supports DHCP** is checked.

## Phase 2: Attacker Provisioning (Kali Linux)
1. Download the latest Kali Linux installer ISO.
2. Create a new VirtualBox VM with 4GB+ RAM and 2+ CPU cores.
3. Attach the ISO, complete the standard Xfce desktop installation, and configure network Adapter 1 to use `Lab-Network`.
4. Verify connectivity using terminal diagnostic commands (`ip a` and `ping`).

## Phase 3: Victim Provisioning (Windows 10 / 11)
1. Create new VMs for Windows 10 and Windows 11 using respective ISOs.
2. Allocate at least 4GB RAM per node and attach both to the shared `Lab-Network`.
3. Apply required bypasses during installation (such as OOBE network bypass `oobe\bypassnro` for Windows 11 and local user provisioning).
