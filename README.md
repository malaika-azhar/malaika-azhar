<div align="center">

<a href="https://www.linkedin.com/in/malaika-azhar-tech">
  <img src="./banner.png" alt="Malaika Azhar - Cloud Infrastructure and DevOps | Azure · Linux · Networking" width="100%" />
</a>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/malaika-azhar-tech)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:malaikawork21@gmail.com)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/malaikaazhar)

</div>

<br/>

## 👩‍💻 About

I am targeting **Cloud Infrastructure Engineer and DevOps roles**, building on Microsoft Azure, Linux and a strong networking foundation. Cloud security is my longer-term goal.

I spent my Cyberster internship doing SOC and detection engineering work (Wazuh SIEM, Suricata IDS, pfSense, threat intelligence, forensics), and I earned the CEH certification. That security background shapes how I build Azure infrastructure: least-privilege access, locked-down network rules, and log-based verification with KQL. Every project is backed by a README, the commands I ran, a cleanup script and screenshot evidence, including the failed attempts.

I am studying Computer Science at Virtual University of Pakistan (expected 2027).

<br/>

## 🧪 Featured Projects

<table>
<tr>
<td width="33%" align="center" valign="top">
<a href="https://github.com/malaika-azhar/Cloud-Infrastructure-Engineering"><img src="./assets/card-cloud.png" alt="Cloud Infrastructure Engineering" /></a>
<br/><sub>Cloud infrastructure projects: virtual machines, networking, storage, identity and access, monitoring, load balancing</sub>
</td>
<td width="33%" align="center" valign="top">
<a href="https://github.com/malaika-azhar/Linux-SysAdmin-Labs"><img src="./assets/card-linux.png" alt="Linux SysAdmin Labs" /></a>
<br/><sub>Backup/restore, Nginx TLS, SSH hardening, BIND9 DNS, user offboarding, monitoring on Azure Ubuntu</sub>
</td>
<td width="33%" align="center" valign="top">
<a href="https://github.com/malaika-azhar/Cybersecurity-Lab-Projects"><img src="./assets/card-security.png" alt="Cybersecurity Lab Projects" /></a>
<br/><sub>SOC, SIEM triage, DFIR, malware analysis, threat mapping</sub>
</td>
</tr>
<tr>
<td width="33%" align="center" valign="top">
<a href="https://github.com/malaika-azhar/Cisco-Networking-Lab-Portfolio"><img src="./assets/card-cisco.png" alt="Cisco Networking Lab Portfolio" /></a>
<br/><sub>26 labs: VLANs, OSPF/EIGRP, ACLs, IPsec VPN, port security, Samba4 AD</sub>
</td>
<td width="33%" align="center" valign="top">
<a href="https://github.com/malaika-azhar/Real-World-Tier2-Support-Projects"><img src="./assets/card-support.png" alt="Real-World Tier-2 Support Projects" /></a>
<br/><sub>osTicket helpdesk on Azure, SPF/DKIM/DMARC audit, Wireshark fault analysis</sub>
</td>
<td width="33%" align="center" valign="top">
<a href="https://github.com/malaika-azhar/customer-tech-support-portfolio"><img src="./assets/card-customer-support.png" alt="Customer Technical Support Portfolio" /></a>
<br/><sub>Ticket simulations, troubleshooting flowcharts, escalation scripts</sub>
</td>
</tr>
</table>

<br/>

## ☁️ Azure Cloud Infrastructure Engineering

Six Azure projects in one repository: [Cloud-Infrastructure-Engineering](https://github.com/malaika-azhar/Cloud-Infrastructure-Engineering)

| Project | What I built and tested |
|---|---|
| Virtual Machines | Ubuntu 24.04 VM with SSH key login, 4 GB data disk mounted by UUID (still mounted after reboot), VM resize, stopped vs deallocated comparison |
| Virtual Networking | VNet with 2 subnets and 2 NSGs, SSH limited to one IP, rules tested with IP flow verify, VNet peering |
| Storage | Blob tiers, soft delete and versioning recovery, SAS tokens (200 then 403), storage firewall, Azure Files over SMB |
| Entra ID and RBAC | Users and groups, RBAC tested as a real user, custom role, managed identity reading a Key Vault secret, resource lock, Azure Policy deny rule |
| Monitor and Log Analytics | Azure Monitor Agent, KQL to find failed SSH logins, metric and log alerts that fired, saved workbook |
| Load Balancer | Standard Load Balancer with 2 private nginx servers behind 1 public IP, failover and recovery tested |

<br/>

## 🌐 Networking (my strongest area)

26 labs in Cisco Packet Tracer, each with topology, configuration, verification and a Limitations section: [Cisco-Networking-Lab-Portfolio](https://github.com/malaika-azhar/Cisco-Networking-Lab-Portfolio)

| Track | Labs | What I covered |
|---|---|---|
| Core networking | 11 | VLSM and CIDR (172.16.0.0/20 split across 3 buildings and 3 WAN links), multi-VLAN DHCP, inter-VLAN routing, VLAN troubleshooting, OSPF (single and multi-area), EIGRP, RIP, static routing, OSPF/EIGRP redistribution, NAT/PAT, HSRP failover and failback, centralized syslog |
| Network security | 6 | Standard and extended ACLs, AAA, SSH hardening, port security with STP loop prevention, IPsec site-to-site VPN |
| IT support | 9 | AD, DNS, email, gateway IP conflict, LAN/Wi-Fi, printing, RDP/VPN, system diagnostics, Windows Update |

This is the base under my Azure work: the same ideas (subnetting, routing, NSG rules, peering, load balancing) I first built and broke in Packet Tracer.

<br/>

## 🔐 Security in My Azure Projects

My Blue Team background shows in how I build. These are tested results from the projects above, not just configuration:

- **Network:** NSGs per subnet with SSH allowed only from one IP, checked with IP flow verify (Deny then Allow)
- **Identity:** RBAC tested as a real user, custom role, managed identity reading a Key Vault secret instead of a stored password
- **Governance:** resource lock and an Azure Policy deny rule
- **Data protection:** SAS tokens (200 then 403), storage firewall, soft delete and versioning recovery
- **Detection:** Azure Monitor Agent and KQL to find failed SSH logins, with metric and log alerts that fired

<br/>

## 🐧 Linux and Systems

Six labs on an Azure Ubuntu VM: [Linux-SysAdmin-Labs](https://github.com/malaika-azhar/Linux-SysAdmin-Labs)

- Backup and restore with a script, checksums and cron, tested by deleting live data on purpose and restoring it
- Nginx reverse proxy with TLS
- SSH hardening with firewall and patching
- BIND9 DNS server
- User management and offboarding
- Disk and uptime monitoring

<br/>

## 🏅 Certifications

I earned the **Certified Ethical Hacker (C|EH)** credential from EC-Council in September 2026. It sits alongside Cisco's Introduction to Cybersecurity and IBM's Cybersecurity Fundamentals.

<div align="center">

<a href="https://aspen.eccouncil.org/Verify">
  <img src="./certs/ceh-badge.png" alt="Certified Ethical Hacker (C|EH) - EC-Council" width="140" />
</a>

**Certified Ethical Hacker (C|EH)** · EC-Council · September 2026 · Certificate No. `ECC7025643981` · [Verify credential →](https://aspen.eccouncil.org/Verify)

![Cisco](https://img.shields.io/badge/Cisco-Introduction_to_Cybersecurity-1BA0D7?style=flat-square&logo=cisco&logoColor=white)
![IBM](https://img.shields.io/badge/IBM-Cybersecurity_Fundamentals-052FAD?style=flat-square)

</div>

<br/>

## 🛠️ Skills

<div align="center">

<img src="https://skillicons.dev/icons?i=azure,linux,bash,powershell,python,git,github,nginx&theme=dark" alt="Tech stack icons" />

</div>

| Area | Tools and topics |
|---|---|
| Cloud (Azure) | Virtual Machines, Virtual Network, NSGs, Storage, Entra ID, RBAC, Key Vault, Azure Monitor, Log Analytics, Load Balancer, Azure Policy |
| Linux and systems | Ubuntu Server, Nginx and TLS, BIND9 DNS, SSH hardening, firewall, cron, Bash, Samba4 Active Directory |
| Networking | TCP/IP, DNS, DHCP, VLANs, inter-VLAN routing, OSPF, EIGRP, ACLs, Wireshark, Cisco Packet Tracer |
| Security and detection | Wazuh SIEM, Suricata IDS, pfSense, MITRE ATT&CK, KQL log analysis, SIEM alert triage, DFIR, SPF/DKIM/DMARC, Nmap, Kali Linux |
| Tools | Git, GitHub, Python, osTicket, Vue 3, Node.js |

<br/>

## 🛡️ SOC and Detection Engineering

**Cybersecurity Intern, Blue Team** · Cyberster · Jun 2026 to Sep 2026

- Deployed a Wazuh SIEM with File Integrity Monitoring and custom detection rules on Ubuntu and Windows endpoints.
- Wrote and tested Suricata IDS rules and integrated the alerts into Wazuh.
- Added threat intelligence feeds (VirusTotal, URLhaus, MITRE ATT&CK) to the SIEM.
- Did malware analysis and digital forensics: disk imaging, Prefetch, registry and timeline correlation.
- Documented every week in a report (12 weekly reports) and loaded a URLhaus feed of 20,000+ malicious URLs into Wazuh.
- After patching openssh on a monitored endpoint, re-scanned and confirmed findings on that package dropped from 30 to 6.

**Lab architecture:** a Wazuh Manager collects events from an Ubuntu server, a Windows host, a Suricata IDS on Kali Linux and a pfSense firewall, with threat intelligence added on top and alerts shown on a SOC dashboard.

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '13px'}, 'flowchart': {'nodeSpacing': 18, 'rankSpacing': 30, 'padding': 8}}}%%
flowchart LR
    subgraph SRC["Log Sources"]
        UA["🐧 Ubuntu agent"]:::src
        WA["🪟 Windows agent"]:::src
        SU["🔎 Suricata IDS<br/>(Kali)"]:::src
        PF["🔥 pfSense firewall<br/>(syslog)"]:::src
    end
    subgraph TI["Threat Intelligence"]
        UH["URLhaus feed"]:::ti
        VT["VirusTotal"]:::ti
        AT["MITRE ATT&CK"]:::ti
    end
    UA --> WM
    WA --> WM
    SU --> WM
    PF --> WM
    UH --> WM
    VT --> WM
    AT --> WM
    WM["🛡️ Wazuh Manager<br/>custom rules + FIM"]:::core --> DB["📊 SOC Dashboard<br/>alerts + reports"]:::out
    classDef src fill:#1A5276,stroke:#0B2E43,stroke-width:2px,color:#FFFFFF
    classDef ti fill:#5B2C6F,stroke:#3B1A48,stroke-width:2px,color:#FFFFFF
    classDef core fill:#943126,stroke:#571C16,stroke-width:2px,color:#FFFFFF
    classDef out fill:#1E8449,stroke:#0B4F2A,stroke-width:2px,color:#FFFFFF
```

<table>
<tr>
<td width="50%" align="center">
<img src="./assets/wazuh-custom-rule-100001.png" alt="Custom Wazuh rule 100001 firing on new user creation" />
<br/><sub><b>Custom rule 100001:</b> alert fires when a new Linux user account is created</sub>
</td>
<td width="50%" align="center">
<img src="./assets/wazuh-fim-alerts.png" alt="Wazuh File Integrity Monitoring alerts for a test file" />
<br/><sub><b>File Integrity Monitoring:</b> file added, modified and deleted events detected</sub>
</td>
</tr>
</table>

<br/>

## 🗓️ Journey

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '15px'}}}%%
timeline
    2026 Feb to May : Cyber Security Training : Cisco networking labs
    2026 Jun to Sep : Blue Team Internship : Wazuh, Suricata, DFIR
    2026 Sep : CEH certified : First open source pull request
    2026 Sep to Oct : Azure cloud projects : Linux SysAdmin labs
```

<br/>

## 🤝 Open Source

<div align="center">

[![Uptime Kuma](https://img.shields.io/badge/Uptime_Kuma-Pull_Request-5CDD8B?style=for-the-badge&logo=uptimekuma&logoColor=black)](https://github.com/louislam/uptime-kuma/pulls?q=author%3Amalaika-azhar)

</div>

Pull request to Uptime Kuma fixing drag-and-drop of monitors out of a group hierarchy (Vue 3, Node.js, Vite).

<br/>

## 🎯 Career Goal

I am looking for a **Cloud Infrastructure Engineer** or **DevOps** role (intern or junior), where I can keep building Azure and Linux infrastructure on real systems. My longer-term goal is **cloud security**, combining that work with my Blue Team background.

<br/>

## 📬 Contact

[LinkedIn](https://www.linkedin.com/in/malaika-azhar-tech) · [malaikawork21@gmail.com](mailto:malaikawork21@gmail.com)
