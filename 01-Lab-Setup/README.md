# Lab Setup

## Objective

A Windows-based SOC lab was built to collect and analyze endpoint logs using Splunk Enterprise and Sysmon.

---

## Environment

| Component | Technology |
|-----------|------------|
| SIEM | Splunk Enterprise |
| Log Forwarder | Splunk Universal Forwarder |
| Endpoint | Windows 10 VM |
| Hypervisor | Oracle VirtualBox |
| Log Source | Windows Event Logs, Sysmon |

---

## Architecture

```text
Windows 10 VM
        │
 Windows Event Logs
 Sysmon Logs
        │
 Splunk Universal Forwarder
        │
 Splunk Enterprise
        │
 SOC Investigation
```

---

## Verification

The following were verified before starting the investigation:

- Splunk Enterprise running
- Windows 10 VM operational
- Sysmon installed
- Universal Forwarder connected
- Windows Event Logs received
- Sysmon logs indexed
