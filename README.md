# Windows-Linux VM-Platform for Global Remote Workforce
Cross-Platform Virtualization Environment for Remote Employee Access (Windows &amp; Linux)
 

**IT Support Trainee / System Administrator**  
*1 May – 31 July 2025, Finland*  


IT Support Trainee / System Administrator
1 May – 31 July 2025, Finland

At the beginning of my traineeship at Tutors Finland / España, I proposed and defined my own project: 
to design and implement a virtualized infrastructure that could serve as a testing and development environment for Tutors’ internal IT operations. 

The project goals were to:
- build a secure and scalable virtualization platform separated from production systems
- enable remote access and centralized management for future testing and training
- document the entire setup to support later development and troubleshooting

I installed Debian 12 on a dedicated bare-metal server and then deployed Proxmox VE on top of it as the main hypervisor. 
The environment included Windows Server 2025 and Ubuntu Server 24.04 LTS configured as domain controllers 
Windows using Active Directory and Ubuntu using Samba in AD-compatible mode. 
I also added Windows 11 Pro and Ubuntu Desktop 24.04 virtual workstations for testing authentication, remote connections and network configurations.

I set up bridged and VLAN-segmented networking, static IP addresses and routing verified through command-line tools. 
DNS and DHCP services were configured and tested for cross-platform name resolution. 
For remote access, I implemented Reemo for Windows systems and ThinLinc for Linux, both running persistently to allow login at any time. 
I also created a macOS architecture model using dedicated Mac Mini hosts from external data centers to ensure Apple-compliant remote management.

All configurations and tests were performed manually. 
I used PowerShell for Windows automation and Bash for Linux scripting, verifying every step through CLI diagnostics. 
I documented the entire process – installation, networking, authentication, remote access and testing – in a structured format to ensure the setup could be replicated and maintained in the future.
This project became a fully functional, administrator-controlled virtualization environment that Tutors can use for secure internal testing and future remote-access development.

Technology Stack

Virtualization and Infrastructure
- Debian 12 base system, Proxmox VE, KVM, ZFS storage, bridged and VLAN networking, static IP configuration, snapshot and rollback management

Operating Systems
- Windows Server 2025, Ubuntu Server 24.04 LTS, Windows 11 Pro, Ubuntu Desktop 24.04

Directory and Authentication
- Active Directory, Samba AD-compatible domain, DNS, DHCP, Group Policy testing, user and role management

Remote Access
- Reemo Remote Desktop, ThinLinc multi-user environment, browser-based access, persistent login configuration, Jump Desktop (macOS plan)

Automation and Scripting
- PowerShell for Windows configuration, Bash for Linux deployment and maintenance, command-line diagnostics (ping, traceroute, ip route, systemctl)

Monitoring and Diagnostics
- Proxmox shell, Windows Event Viewer, Syslog, journalctl, connectivity and performance testing

Security and Access Control
- Role-based permissions in Proxmox, SSH key authentication, secure boot, account separation

Documentation and Maintenance
- Technical documentation, configuration logs, network maps, version tracking, recovery and rollback procedures


## VM PROJECT SCREENSHOTS
https://jyu-my.sharepoint.com/:b:/g/personal/jokrpaak_jyu_fi/Eb5GXIEqJvZGlatl0420MhABazk4DB9gyfDBJV7m0cDjsQ?e=iBomhv
