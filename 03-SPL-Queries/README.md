# SPL Queries

## Overview

This section contains the Splunk Search Processing Language (SPL) queries used during the SOC incident investigation. These searches were performed to analyze Sysmon and Windows Event Logs, identify suspicious process execution, examine parent-child process relationships, and reconstruct the incident timeline.

---

## Investigation Areas

The following queries were used during the investigation:

- Process Creation Analysis
- Parent-Child Process Investigation
- User Activity Analysis
- Timeline Reconstruction

---

## Query Files

| File | Purpose |
|------|---------|
| Process_Creation.spl | Identify Sysmon Event ID 1 process creation events |
| Parent_Child_Process.spl | Review parent-child process relationships |
| Process_By_User.spl | Identify processes executed by specific users |
| Timeline.spl | Display events in chronological order |

---

## Skills Demonstrated

- Splunk Search Processing Language (SPL)
- Windows Event Log Analysis
- Sysmon Log Analysis
- Process Investigation
- Timeline Analysis
- Security Event Correlation

  ## Process_Creation.spl
  - index=* sourcetype="WinEventLog:Microsoft-Windows-Sysmon/Operational" EventCode=1
| table _time User Image ParentImage CommandLine

## Command.exe.spl
- index=* sourcetype="WinEventLog:Microsoft-Windows-Sysmon/Operational" EventCode=1 Image="*cmd.exe"
| table _time User Image ParentImage CommandLine
| sort -_time

## Parent_Child_Process.spl
- index=* sourcetype="WinEventLog:Microsoft-Windows-Sysmon/Operational" EventCode=1
| table _time ParentImage Image CommandLine

 
