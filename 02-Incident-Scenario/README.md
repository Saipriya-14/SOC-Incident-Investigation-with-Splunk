# Incident Scenario

## Scenario Overview

During routine security monitoring, a Windows endpoint generated multiple Sysmon process creation events. A PowerShell process was observed executing shortly after a user logged into the system. The activity was investigated to determine whether it represented legitimate administrative activity or potentially suspicious behavior.

The investigation focused on analyzing Windows Event Logs and Sysmon telemetry collected in Splunk Enterprise to identify the processes involved, review command-line arguments, reconstruct the sequence of events, and document the findings.

---

## Investigation Objectives

- Identify the process that triggered the investigation.
- Determine which user executed the process.
- Analyze the parent-child process relationship.
- Review command-line arguments.
- Reconstruct the event timeline.
- Collect supporting evidence.
- Map observed activity to the MITRE ATT&CK framework.
- Produce an incident investigation report.

---

## Simulated Activities

The following actions were performed on the Windows 10 virtual machine to generate logs:

- Logged into the Windows system.
- Opened Command Prompt (`cmd.exe`).
- Opened PowerShell (`powershell.exe`).
- Executed basic PowerShell commands such as:
  - `Get-Process`
  - `Get-Service`
  - `Get-ChildItem`
- Opened Notepad (`notepad.exe`) to generate additional process creation events.

These actions generated Windows Event Logs and Sysmon Event ID 1 (Process Creation) events, which were forwarded to Splunk Enterprise for analysis.

---

## Expected Investigation Outcome

The investigation should identify:

- User account involved
- Process execution details
- Parent process
- Command-line activity
- Event timestamps
- Supporting evidence
- Overall assessment of the activity
