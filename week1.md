# Week 1 – System Planning and Distribution Selection
[Next Week →](week2.md)
## Overveiw
With week 1 the aim was to plan and deploy a headlss Linux server and verify basic system and network functions using tools. Due to my hardware restaints (Apple M1) I was forced to pivot to UTM instead of VirtualBox, which was used to host the VM while still meeting all coursework requirements.
## System Setup
- **Host machine:** Apple MacBook (M1)
- **Virtualisation platform:** UTM
- **Guest OS:** Ubuntu Server 24.04 LTS (ARM64)
- **Server type:** Headless (no GUI)
- **RAM:** 4 GB
- **CPU:** 2 cores
- **Disk:** 20 GB
## Network Configuration
Two network interfaces were configured:
- **Shared Network (NAT):** Gave internet access for updates and package installation.
- **Emulated VLAN:** Acts as a host-only network for secure local administration and SSH access.

This setup was used to mirror the NAT and host-only adapter architecture used in VirtualBox.
## Command-Line Evidence

### Hostname Verification
```bash
hostname
