# Alert Explainability Card (Template)

**Alert Name:** (e.g., Mshta Remote HTA Execution)  
**Why it fired:** `Image=mshta.exe` AND `CommandLine contains http` (LOLBIN execution technique)  
**Data Source:** Sysmon Event ID 1 (Process Create)  
**ATT&CK:** T1218.005  
**Confidence:** Medium/High  
**Next steps:** Verify parent process, destination host, related DNS queries, and any subsequent PowerShell 4104 events.
