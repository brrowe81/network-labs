# Kali VM Setup

## Goals
- Fresh Kali install with guest tools
- Basic hardening and logging enabled
- Snapshot baseline

## Steps
1) Download latest Kali ISO
2) Create VM (2 CPU, 4–8 GB RAM, NAT/Host-only adapters)
3) Install + update:
   \\\ash
   sudo apt update && sudo apt full-upgrade -y
   \\\
4) Install guest tools:
   \\\ash
   sudo apt install -y open-vm-tools-desktop spice-vdagent
   \\\
5) Create user, disable root login over SSH (if enabled), set strong password
6) Snapshot VM as **kali-base**

## Notes
- Network: use **Host-only** for lab-only traffic; add **NAT** only when needed for updates
- Screenshots: put in ./screenshots
