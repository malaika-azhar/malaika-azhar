<div align="center">

<a href="https://www.linkedin.com/in/malaika-azhar-tech">
  <img src="./banner.png" alt="Malaika Azhar - Aspiring SOC Analyst | Blue Team" width="100%" />
</a>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/malaika-azhar-tech)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:malaikawork21@gmail.com)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/malaikaazhar)

</div>

<br/>

## 👩‍💻 About

BSCS student (Virtual University of Pakistan, 2027) targeting **SOC Analyst and Blue Team roles**.

During my Blue Team internship I built a working detection setup: Wazuh SIEM, Suricata IDS, a pfSense firewall and live threat intelligence feeds. Every project in my repositories is backed by screenshot evidence, including the failed attempts.

<br/>

## 🏅 Certifications

I earned the **Certified Ethical Hacker (C|EH)** credential from EC-Council in September 2026. It sits alongside Cisco's Introduction to Cybersecurity and IBM's Cybersecurity Fundamentals. The credential can be checked on EC-Council's verification page with the certificate number below.

<div align="center">

<a href="https://aspen.eccouncil.org/Verify">
  <img src="./certs/ceh-badge.png" alt="Certified Ethical Hacker (C|EH) - EC-Council" width="140" />
</a>

**Certified Ethical Hacker (C|EH)** · EC-Council · September 2026 · Certificate No. `ECC7025643981` · [Verify credential →](https://aspen.eccouncil.org/Verify)

![Cisco](https://img.shields.io/badge/Cisco-Introduction_to_Cybersecurity-1BA0D7?style=flat-square&logo=cisco&logoColor=white)
![IBM](https://img.shields.io/badge/IBM-Cybersecurity_Fundamentals-052FAD?style=flat-square)

</div>

<br/>

## 📈 Internship Results

Results from my 12-week Blue Team internship: I documented every week in a report, loaded a URLhaus feed of 20,000+ malicious URLs into Wazuh, and mapped detections across 6 MITRE ATT&CK tactics. After patching openssh on a monitored endpoint, I re-scanned to confirm the findings on that package dropped from 30 to 6.

<div align="center">

![Reports](https://img.shields.io/badge/Weekly_Reports-12_Documented-943126?style=for-the-badge)
![Feed](https://img.shields.io/badge/Threat_Feed-20%2C000%2B_URLs-1A5276?style=for-the-badge)
![MITRE](https://img.shields.io/badge/MITRE_ATT%26CK-6_Tactics_Mapped-5B2C6F?style=for-the-badge)
![CVE](https://img.shields.io/badge/Findings_After_Patch-30_→_6-2ea44f?style=for-the-badge)

</div>

<br/>

## 🧱 Lab Architecture

My lab is built around a Wazuh Manager that collects events from an Ubuntu server, a Windows host, a Suricata IDS on Kali Linux and a pfSense firewall. Threat intelligence from URLhaus and VirusTotal is added on top, and the alerts end up on a SOC dashboard.

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

### Network Map

All lab machines sit in one internal network behind the pfSense firewall.

<div align="center">
<img src="./assets/network-map.png" width="55%" alt="Lab network map: Internet, pfSense firewall and internal lab network" />
</div>

<br/>

## 🔍 Detection Evidence

Screenshots from my Wazuh lab: custom rules, File Integrity Monitoring and a SOC dashboard.

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

<div align="center">
<img src="./assets/soc-dashboard-alert-timeline.png" alt="SOC dashboard alert timeline in Wazuh" width="60%" />
<br/><sub><b>SOC dashboard:</b> alert volume over time, built in Wazuh</sub>
</div>

<br/>

## 🧪 Featured Projects

<table>
<tr>
<td width="33%" align="center" valign="top">
<a href="https://github.com/malaika-azhar/Cybersecurity-Lab-Projects"><img src="./assets/card-security.png" alt="Cybersecurity Lab Projects" /></a>
<br/><sub>SOC, SIEM triage, DFIR, malware analysis, threat mapping</sub>
</td>
<td width="33%" align="center" valign="top">
<a href="https://github.com/malaika-azhar/Cisco-Networking-Lab-Portfolio"><img src="./assets/card-cisco.png" alt="Cisco Networking Lab Portfolio" /></a>
<br/><sub>VLANs, OSPF/EIGRP, ACLs, IPsec VPN, port security</sub>
</td>
<td width="33%" align="center" valign="top">
<a href="https://github.com/malaika-azhar/Real-World-Tier2-Support-Projects"><img src="./assets/card-support.png" alt="Real-World Tier-2 Support Projects" /></a>
<br/><sub>osTicket helpdesk on Azure, SPF/DKIM/DMARC audit, Wireshark fault analysis</sub>
</td>
</tr>
</table>

<br/>

## 🗓️ Journey

I started with Cisco networking labs, moved into Blue Team work during my internship, and closed this period with the CEH certification and my first open source pull request.

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '15px'}}}%%
timeline
    2026 Feb to May : Cyber Security Training : Cisco labs
    2026 Jun to Sep : Blue Team Internship : Wazuh, Suricata, DFIR
    2026 Sep : CEH certified : Open source pull request
```

**Cybersecurity Intern, Blue Team** · Cyberster · Jun 2026 to Sep 2026
- Deployed a Wazuh SIEM with File Integrity Monitoring and custom detection rules on Ubuntu and Windows endpoints.
- Wrote and tested Suricata IDS rules, and integrated the alerts into Wazuh.
- Added threat intelligence feeds (VirusTotal, URLhaus, MITRE ATT&CK) to the SIEM.
- Did malware analysis and digital forensics: disk imaging, Prefetch, registry and timeline correlation.

<br/>

## 🛠️ Skills

My main focus is SIEM monitoring, detection rules and digital forensics, supported by networking and firewall knowledge.

<div align="center">

<img src="https://skillicons.dev/icons?i=linux,windows,bash,powershell,python,git,github,azure&theme=dark" alt="Tech stack icons" />

<br/><br/>

![Wazuh](https://img.shields.io/badge/Wazuh-005EB8?style=for-the-badge&logo=wazuh&logoColor=white)
![Suricata](https://img.shields.io/badge/Suricata-EF3B2D?style=for-the-badge)
![pfSense](https://img.shields.io/badge/pfSense-212121?style=for-the-badge&logo=pfsense&logoColor=white)
![Splunk](https://img.shields.io/badge/Splunk-000000?style=for-the-badge&logo=splunk&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Kali](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![Cisco](https://img.shields.io/badge/Cisco_IOS-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![MITRE](https://img.shields.io/badge/MITRE_ATT%26CK-C8102E?style=for-the-badge)

</div>

| Area | Tools and topics |
|---|---|
| SIEM and detection | Wazuh, Suricata, Splunk, MITRE ATT&CK, D3FEND |
| Forensics and malware | Autopsy, Sleuth Kit, Prefetch, registry, ANY.RUN, VirusTotal |
| Network security | pfSense, Cisco IOS, Wireshark, ACLs, VPN |

<br/>

## 🤝 Open Source

<div align="center">

[![Uptime Kuma](https://img.shields.io/badge/Uptime_Kuma-Pull_Request-5CDD8B?style=for-the-badge&logo=uptimekuma&logoColor=black)](https://github.com/louislam/uptime-kuma/pulls?q=author%3Amalaika-azhar)

</div>

Pull request to Uptime Kuma fixing drag-and-drop of monitors out of a group hierarchy.

<br/>

## 🎯 Career Goal

I am looking for a **SOC Analyst (Blue Team)** or **Network/NOC Engineer** role where I can keep building detection and investigation skills on real systems.

<br/>

## 📬 Contact

[LinkedIn](https://www.linkedin.com/in/malaika-azhar-tech) · [malaikawork21@gmail.com](mailto:malaikawork21@gmail.com)
