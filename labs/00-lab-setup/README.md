# Objective
Build the foundational virtual lab environment used by all subsequent labs in this portfolio. By the end of this setup you will have Oracle VirtualBox installed, three virtual machines provisioned (Windows Server 2022, Windows 10/11 Pro, and Ubuntu Server 22.04), and an internal network connecting them. This environment supports Active Directory, networking, Windows troubleshooting, osTicket, and PowerShell labs without requiring any external hardware beyond a single host computer.
# Tools Used
| Tool | Purpose
| --- | --- |
| Oracle VirtualBox 7.x| Type-2 hypervisor for running all lab VMs |
| Windows Server 2022 ISO | Domain controller and DNS server (Labs 01, 03, 05) |
| Windows 10/11 Pro ISO | Domain-joined client workstation (Labs 01-03, 05) |
| Ubuntu Server 22.04 LTS ISO | LAMP stack host for osTicket (Lab 04) |
| VirtualBox Extension Pack | USB 2.0/3.0 support and PXE boot (optional) |
# Hardware Requirements
| Resource | Minimum | Recommended |
| --- | --- | --- |
| CPU | 4 cores (Intel VT-x / AMD-V enabled) | 6+ cores |
| RAM | 12 GB | 16+ GB |
| Disk Space | 120 GB free | 200+ GB free (SSD preferred) |
| Network | Any internet connection for ISO downloads | Wired connection for stability |

> **Note:** Intel VT-x or AMD-V must be enabled in your BIOS/UEFI settings. VirtualBox will not start 64-bit VMs without hardware virtualization support.
# Diagram Description
```mermaid
flowchart TB
    A[Host Machine<br/>(Your PC)
