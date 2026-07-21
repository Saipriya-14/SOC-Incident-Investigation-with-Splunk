# SOC Incident Investigation with Splunk Enterprise

## Project Overview

This project demonstrates a complete Security Operations Center (SOC) incident investigation using Splunk Enterprise, Splunk Universal Forwarder, Windows Event Logs, and Sysmon. A simulated cyber attack was performed in a controlled virtual lab environment to generate realistic security events. These logs were collected, indexed, and analyzed in Splunk to identify suspicious activities, reconstruct the attack timeline, document Indicators of Compromise (IOCs), and map attacker techniques to the MITRE ATT&CK framework.

The project follows a structured SOC investigation workflow similar to that used by entry-level SOC analysts, covering log collection, event analysis, evidence gathering, incident reporting, and security documentation.

---

## Project Objectives

- Build a SOC lab using Splunk Enterprise and VirtualBox.
- Configure Splunk Universal Forwarder to collect Windows logs.
- Install and configure Sysmon for enhanced endpoint visibility.
- Simulate suspicious activities in a controlled environment.
- Investigate security events using Splunk Search Processing Language (SPL).
- Correlate events to reconstruct the attack timeline.
- Identify Indicators of Compromise (IOCs).
- Map attacker techniques to the MITRE ATT&CK framework.
- Produce a professional incident investigation report.

---

## Lab Environment

| Component | Details |
|-----------|---------|
| SIEM Platform | Splunk Enterprise |
| Log Forwarder | Splunk Universal Forwarder |
| Endpoint | Windows 10 Virtual Machine |
| Hypervisor | Oracle VirtualBox |
| Log Sources | Windows Event Logs, Sysmon |
| Operating System | Windows 10 |
| Investigation Tool | Splunk Search & Reporting |

---

## Lab Architecture

```text
Windows 10 VM
│
├── Windows Event Logs
├── Sysmon Logs
│
▼
Splunk Universal Forwarder
│
▼
Splunk Enterprise
│
▼
SOC Investigation
│
├── SPL Queries
├── Event Correlation
├── IOC Analysis
├── Attack Timeline
├── MITRE ATT&CK Mapping
└── Incident Report
```

---

## Investigation Workflow

1. Configure the lab environment.
2. Install and configure Sysmon.
3. Configure Splunk Universal Forwarder.
4. Forward Windows Event Logs and Sysmon logs.
5. Simulate attacker activities.
6. Analyze events using SPL queries.
7. Correlate security events.
8. Identify Indicators of Compromise (IOCs).
9. Reconstruct the attack timeline.
10. Map techniques to the MITRE ATT&CK framework.
11. Document findings and recommendations.

---

## Skills Demonstrated

- Security Monitoring
- SOC Incident Investigation
- SIEM Operations
- Splunk Enterprise
- Splunk Search Processing Language (SPL)
- Windows Event Log Analysis
- Sysmon Log Analysis
- Event Correlation
- Threat Detection
- IOC Analysis
- Attack Timeline Reconstruction
- MITRE ATT&CK Mapping
- Incident Reporting
- Technical Documentation

---

## Tools Used

- Splunk Enterprise
- Splunk Universal Forwarder
- Sysmon
- Oracle VirtualBox
- Windows Event Viewer
- Windows 10

---

## Repository Structure

```text
SOC-Incident-Investigation-with-Splunk/
│
├── README.md
├── 01-Lab-Setup/
├── 02-Attack-Scenario/
├── 03-SPL-Queries/
├── 04-Evidence/
├── 05-Attack-Timeline/
├── 06-Indicators-of-Compromise/
├── 07-MITRE-ATTACK/
├── 08-Incident-Report/
└── Screenshots/
```

---

## Investigation Highlights

- Built a Windows-based SOC lab using Splunk Enterprise and VirtualBox.
- Configured Splunk Universal Forwarder to collect Windows Event Logs and Sysmon logs.
- Investigated simulated process creation events using Sysmon Event ID 1.
- Used SPL queries to identify suspicious processes and analyze event details.
- Reconstructed attack activity from collected log data.
- Documented Indicators of Compromise (IOCs) and supporting evidence.
- Mapped observed techniques to the MITRE ATT&CK framework.
- Produced a structured incident investigation report with findings and recommendations.

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Building and configuring a SIEM environment.
- Collecting and analyzing Windows security logs.
- Investigating endpoint activity using Sysmon.
- Writing and executing SPL queries.
- Correlating security events.
- Performing SOC-style incident investigations.
- Documenting evidence and investigation findings.
- Creating professional cybersecurity documentation for GitHub.

---

## Future Improvements

- Simulate additional attack scenarios (brute force, PowerShell, persistence).
- Create Splunk dashboards for security monitoring.
- Configure automated Splunk alerts.
- Integrate Sigma detection rules.
- Add Atomic Red Team attack simulations.
- Expand MITRE ATT&CK coverage.
