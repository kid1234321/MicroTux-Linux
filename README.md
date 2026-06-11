# 🐧 MicroTux OS (v1.0)
An ultra-lightweight, minimal 64-bit Linux operating system engineered entirely from the source code blocks up.

```text
     __
    (o O)     [ MICROTUX OS ]
    / v \     
   /( _ )\    64-bit Core System v1.0
   ^^   ^^    Booting complete.
```

## 🚀 Overview
MicroTux OS is a custom-tailored distribution built using the Linux 6.14 kernel and a statically-linked BusyBox userland payload. Designed with a robust, fail-safe architecture, it functions as an autonomous installation host and bulletproof deployment system on real bare-metal hardware.

## 🛠️ Advanced Core Features
*   **Host Sector Cloning Engine (`install-os`)**: High-speed imaging protocol that streams standardized production payloads directly onto physical hardware storage disks (`dd` master block writes).
*   **Fail-Safe A/B Dual Partition Layout**: Zero-risk deployment array separating active (`TUX_ACTIVE`) and fallback (`TUX_BACKUP`) system environments for risk-free OS updates.
*   **Persistent User Data Isolation (`TUX_DATA`)**: Allocates and mounts storage at the absolute end of the hard drive layout to safely preserve user files across entire system reinstallations.
*   **Pre-Boot OTA Interceptor Loop**: Automatically intercepting and mounting connected USB hardware layers during initialization to scan for and apply fresh system update packages.
*   **Hardware Lifecycle ACPI Monitor**: Integrated `acpid` daemon monitoring physical casing hardware inputs to trigger graceful, safe partition unmount sync structures before cutting power.

## 💾 Hardware Target Parameters
*   **Architecture**: x86_64 Native (Modern 64-bit)
*   **Memory Footprint**: Fits in under 30MB of system RAM
*   **Boot Interface**: Legacy BIOS / Master Boot Record (MBR) compatibility

---
Built completely from scratch for the love of open-source engineering. 
