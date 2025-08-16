# Windows VM Setup

## Goals
- Windows workstation/server for blue-team logs and basic target hardening
- Enable useful logging (Security, PowerShell, Sysmon optional)
- Snapshot baseline

## Steps
1) Install Windows (local admin, strong password)
2) Enable PowerShell logging:
   - Group Policy: Script Block + Module logging
3) (Optional) Install Sysmon with a community config
4) Windows Update, disable unnecessary services for lab
5) Snapshot VM as **win-base**

## Notes
- Network: Host-only adapter for lab, NAT as needed for updates
- Screenshots: ./screenshots
