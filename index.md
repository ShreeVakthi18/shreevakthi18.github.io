# Security Portfolio

- Hi, I'm **Shree Vakthi**, a B.E. CSE (Cyber Security) student at SRM Madurai College for Engineering and Technology.
- This repo is an index of my hands-on security labs and projects.
- Every lab lives in its own repo with its own screenshots, evidence, and commit history.

---

## Defensive Security & SOC

### [Wazuh SOC Home Lab](https://github.com/ShreeVakthi18/wazuh-soc-home-lab)
- Built a SIEM lab with Wazuh, deployed from the official OVA on VirtualBox.
- Simulated a brute-force login, then local account creation and privilege escalation, on a Windows 10/11 endpoint.
- Investigated the resulting alerts the way a SOC analyst would.
- **Tools:** Wazuh, Windows Security audit logging, VirtualBox.

### [Firewall, IDS & IPS Lab](https://github.com/ShreeVakthi18/Firewall-IDS-IPS-Lab)
- Compared three layers of network defense: Windows Defender Firewall, Snort, and Fail2ban.
- Wrote and tested a rule or policy in each tool.
- Compared detection (alert) against prevention (block) and documented the results with screenshots.
- **Tools:** Windows Defender Firewall, Snort, Fail2ban, Ubuntu VM on VirtualBox.

### [Linux System Monitoring](https://github.com/ShreeVakthi18/linux-system-monitoring)
- Monitored `auth.log` to spot failed login attempts.
- Watched live system activity through `syslog`.
- Managed file and directory permissions on Linux.
- **Tools:** Ubuntu, `tail`, `chmod`, `ls`.

---

## Network Security

### [Network Reconnaissance & Attack Surface Assessment](https://github.com/ShreeVakthi18/Network-Reconnaissance-Attack-Surface-Assessment)
- Ran TCP port scans, service version detection (`-sV`), and OS detection (`-O`) against my own system.
- Found all common TCP ports closed, which showed a small attack surface.
- Noted that OS detection accuracy drops when no ports are open.
- **Tools:** Nmap, Ubuntu on WSL.

### [Network Vulnerability Audit](https://github.com/ShreeVakthi18/network-vulnerability-audit)
- Mapped the attack surface of a Linux target and documented the findings in a risk table.
- Flagged cleartext Telnet (Critical), outdated Apache 2.4.7 (High), and a filtered SMB port (Medium).
- Included terminal screenshots and the raw audit log as evidence.
- **Tools:** Nmap, Linux.

### [Network Traffic Analysis](https://github.com/ShreeVakthi18/network-traffic-analysis)
- Analyzed network traffic as part of my network security practice.
- See the repo for the full write-up and evidence.

---

## Hardening & Cloud Security

### [Linux Infrastructure Hardening](https://github.com/ShreeVakthi18/linux-infrastructure-hardening)
- Wrote a Bash script that hardens a default Linux install.
- Blocks insecure ports (Telnet 23 and SMB 445) with UFW.
- Automates package updates and disables SSH root login.
- Fixes the issues found in my Nmap audit.
- **Tools:** Bash, UFW, SSH, Nmap.

### [AWS Attack Surface Diff Engine (ASDE)](https://github.com/ShreeVakthi18/AWS-Attack-Surface-Diff-Engine)
- Built a Python tool that compares a "known good" cloud baseline against the live state to catch security drift.
- Detects public S3 buckets, open SSH or management ports, and unauthorized IAM access keys.
- Auto-remediates public buckets back to private.
- Outputs JSON events that are ready for SIEMs like Splunk or Sentinel.
- **Tools:** Python, Boto3, Moto.

---

## Forensics & Password Security

### [Project Sentinel: Forensic Triage Suite](https://github.com/ShreeVakthi18/Project-Sentinel-Forensics)
- Wrote a PowerShell tool that captures a point-in-time snapshot for rapid incident response.
- Maps open ports to PIDs, audits persistence mechanisms, and profiles resource-heavy processes.
- Used PID correlation to verify a non-standard listener on port 7070 as a legitimate service.
- **Tools:** PowerShell, Windows 10/11.

### [Offline Password Risk Assessment](https://github.com/ShreeVakthi18/offline-password-risk-assessment)
- Assessed how weak passwords and fast hashing hold up in an offline attack after a credential store leak.
- Used only self-generated md5crypt hashes in a controlled environment.
- Focused on risk analysis and defensive insight, not exploitation.
- **Tools:** John the Ripper, rockyou.txt, Ubuntu on WSL.

---

## Skills Covered

- **SIEM & monitoring:** Wazuh, log analysis, Windows audit policy.
- **Network defense:** Firewalls, IDS/IPS, Snort, Fail2ban, UFW.
- **Recon & auditing:** Nmap scanning, service and OS detection, risk rating.
- **Incident response:** Volatile evidence collection, persistence auditing.
- **Cloud security:** AWS misconfiguration and drift detection.
- **Scripting:** Python, Bash, PowerShell.

---

## Contact

- GitHub: [@ShreeVakthi18](https://github.com/ShreeVakthi18)
