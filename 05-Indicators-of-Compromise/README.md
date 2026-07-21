# Indicators of Compromise (IOCs)

## Identified Artifacts

| Indicator | Value |
|-----------|-------|
| User | Administrator |
| Host | Windows 10 VM |
| Process | cmd.exe |
| Parent Process | postgres.exe |
| Event ID | Sysmon Event ID 1 |

---

## Analysis

The investigation identified PowerShell execution and associated process creation events. The activity was analyzed to determine whether it represented legitimate administrative behavior or suspicious endpoint activity.
