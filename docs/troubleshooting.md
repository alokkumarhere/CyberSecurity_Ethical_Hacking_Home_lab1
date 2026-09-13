# 🔧 Lab Troubleshooting & Engineering Log

During the deployment of this home lab, several environmental and virtualization challenges were encountered and successfully resolved.

## 1. Kali Linux Accessibility (Orca Screen Reader Issue)
* **Problem:** The built-in accessibility screen reader (Orca) was accidentally triggered during setup, causing text-to-speech audio feedback upon keystrokes.
* **Resolution:** Permanently purged the accessibility package from the system to clean up resources:
  ```bash
  sudo apt purge orca -y
## 2. Windows 10 UI Freezing in VirtualBox
 Problem: The Windows 10 virtual machine experienced random graphics freezes and UI unresponsiveness.
Resolution:
  1.Disabled 3D Acceleration in the VirtualBox display settings for the VM.
  2.Turned off Transparency effects inside Windows 10 Settings (Personalization > Colors) to prevent rendering crashes with the VBoxSVGA driver.

## 3. Windows 11 Hardware & OOBE Network Restrictions
Problem: Windows 11 installation failed due to strict virtual TPM/Secure Boot requirements, followed by forced Microsoft account login prompts requiring an internet connection.
Resolution:
   1.TPM/Secure Boot Bypass: Created LabConfig registry keys (BypassTPMCheck and BypassSecureBootCheck) via Shift + F10 during setup.
   2.Network Bypass: Bypassed the forced online account setup during OOBE using the command line:
     DOS
      ```bash
         oobe\bypassnro
     This unlocked the "I don't have internet" option, allowing a clean, offline local user account creation.
