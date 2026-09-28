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

BSCS student (2027) targeting **SOC Analyst and Blue Team roles**. I built a working detection lab with Wazuh, Suricata and pfSense, and every project is backed by screenshots.

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

### Network Map

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '15px'}, 'flowchart': {'nodeSpacing': 40, 'rankSpacing': 55}}}%%
flowchart TB
    NET(("🌐 Internet")):::ext
    subgraph LAN["Internal Lab Network"]
        FW["🔥 pfSense Firewall<br/>WAN and LAN gateway"]:::fw
        WM["🛡️ Wazuh Manager<br/>Indexer + Dashboard"]:::core
        KA["🔎 Kali Linux VM<br/>Suricata IDS"]:::src
        UB["🐧 Ubuntu Server<br/>Wazuh agent"]:::src
        WN["🪟 Windows host<br/>Wazuh agent"]:::src
    end
    NET --- FW
    FW --- WM
    FW --- KA
    FW --- UB
    FW --- WN
    classDef ext fill:#2C3E50,stroke:#1B2631,stroke-width:2px,color:#FFFFFF
    classDef fw fill:#212121,stroke:#000000,stroke-width:2px,color:#FFFFFF
    classDef core fill:#943126,stroke:#571C16,stroke-width:2px,color:#FFFFFF
    classDef src fill:#1A5276,stroke:#0B2E43,stroke-width:2px,color:#FFFFFF
```

<br/>

## 🔍 Detection Evidence

<table>
<tr>
<td width="50%" align="center">
<img src="./assets/wazuh-custom-rule-100001.png" alt="Custom Wazuh rule 100001 firing on new user creation" />
<br/><sub><b>Custom rule:</b> new user created</sub>
</td>
<td width="50%" align="center">
<img src="./assets/wazuh-fim-alerts.png" alt="Wazuh File Integrity Monitoring alerts for a test file" />
<br/><sub><b>File Integrity Monitoring:</b> file changes detected</sub>
</td>
</tr>
</table>

<div align="center">
<img src="./assets/soc-dashboard-alert-timeline.png" alt="SOC dashboard alert timeline in Wazuh" width="60%" />
<br/><sub><b>SOC dashboard:</b> alert volume over time</sub>
</div>

<br/>

## 🧪 Featured Projects

<div align="center">

<a href="https://github.com/malaika-azhar/Cybersecurity-Lab-Projects"><img src="./assets/card-security.png" width="32%" alt="Cybersecurity Lab Projects" /></a>
<a href="https://github.com/malaika-azhar/Cisco-Networking-Lab-Portfolio"><img src="./assets/card-cisco.png" width="32%" alt="Cisco Networking Lab Portfolio" /></a>
<a href="https://github.com/malaika-azhar/Real-World-Tier2-Support-Projects"><img src="./assets/card-support.png" width="32%" alt="Real-World Tier-2 Support Projects" /></a>

</div>

<br/>

## 🗓️ Journey

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '15px'}}}%%
timeline
    2026 Feb to May : Cyber Security Training : Cisco labs
    2026 Jun to Sep : Blue Team Internship : Wazuh, Suricata, DFIR
    2026 Sep : CEH certified : Open source pull request
```

<br/>

## 🛠️ Skills

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

<br/>

## 🤝 Open Source

<div align="center">

[![Uptime Kuma](https://img.shields.io/badge/Uptime_Kuma-Pull_Request-5CDD8B?style=for-the-badge&logo=uptimekuma&logoColor=black)](https://github.com/louislam/uptime-kuma/pulls?q=author%3Amalaika-azhar)

</div>
