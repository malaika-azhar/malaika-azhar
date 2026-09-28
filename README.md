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
I completed a Blue Team internship where I built a working detection setup: Wazuh SIEM, Suricata IDS, a pfSense firewall and live threat intelligence feeds.
Every project in my repositories is backed by screenshot evidence, including the failed attempts.

<br/>

## 🏅 Certifications

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

<div align="center">

![Reports](https://img.shields.io/badge/Weekly_Reports-12_Documented-943126?style=for-the-badge)
![Feed](https://img.shields.io/badge/Threat_Feed-20%2C000%2B_URLs-1A5276?style=for-the-badge)
![MITRE](https://img.shields.io/badge/MITRE_ATT%26CK-6_Tactics_Mapped-5B2C6F?style=for-the-badge)
![CVE](https://img.shields.io/badge/Findings_After_Patch-30_→_6-2ea44f?style=for-the-badge)

</div>

<br/>

## 🧱 Lab Architecture

How my SOC lab fits together:

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '15px'}, 'flowchart': {'nodeSpacing': 35, 'rankSpacing': 50}}}%%
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

<br/>

## 🔍 Detection Evidence

Screenshots from my Wazuh lab (Ubuntu agent, custom rules and File Integrity Monitoring).

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

| | Project | What it covers |
|---|---|---|
| 🛡️ | [Cybersecurity Lab Projects](https://github.com/malaika-azhar/Cybersecurity-Lab-Projects) | SOC, SIEM triage, DFIR, malware analysis, threat mapping |
| 🌐 | [Cisco Networking Lab Portfolio](https://github.com/malaika-azhar/Cisco-Networking-Lab-Portfolio) | VLANs, OSPF/EIGRP, ACLs, IPsec VPN, port security |
| 🎫 | [Real-World Tier-2 Support Projects](https://github.com/malaika-azhar/Real-World-Tier2-Support-Projects) | osTicket helpdesk on Azure, SPF/DKIM/DMARC audit, Wireshark fault analysis |

<br/>

## 💼 Experience

**Cybersecurity Intern, Blue Team** · Cyberster · Jun 2026 to Sep 2026
- Deployed a Wazuh SIEM with File Integrity Monitoring and custom detection rules on Ubuntu and Windows endpoints.
- Wrote and tested Suricata IDS rules, and integrated the alerts into Wazuh.
- Added threat intelligence feeds (VirusTotal, URLhaus, MITRE ATT&CK) to the SIEM.
- Did malware analysis and digital forensics: disk imaging, Prefetch, registry and timeline correlation.

<br/>

## 🛠️ Skills

<div align="center">

<img src="https://skillicons.dev/icons?i=linux,windows,bash,powershell,python,git,github,azure&theme=dark" alt="Tech stack icons" />

</div>

| Area | Tools and topics |
|---|---|
| SIEM and detection | Wazuh, Suricata, Splunk, MITRE ATT&CK, D3FEND |
| Forensics and malware | Autopsy, Sleuth Kit, Prefetch, registry, ANY.RUN, VirusTotal |
| Network security | pfSense, Cisco IOS, Wireshark, ACLs, VPN |

<br/>

## 🤝 Open Source

- [Uptime Kuma](https://github.com/louislam/uptime-kuma/pulls?q=author%3Amalaika-azhar): pull request fixing drag-and-drop of monitors out of a group hierarchy.

<br/>

## 📬 Contact

[LinkedIn](https://www.linkedin.com/in/malaika-azhar-tech) · [malaikawork21@gmail.com](mailto:malaikawork21@gmail.com)
