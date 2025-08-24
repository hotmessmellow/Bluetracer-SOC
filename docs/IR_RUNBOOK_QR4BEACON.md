# QR4Beacon – First-Hour IR Runbook

**Scenario:** QR-driven phishing chain to mshta → PowerShell EncodedCommand → DNS beaconing → scheduled task.

## Triage (0–15 min)
- Validate alerts (PowerShell 4104 + mshta + high-entropy DNS).
- Confirm host/user, process lineage (parent/child), and command lines.

## Containment (15–30 min)
- Isolate endpoint; reset credentials if suspicious activity confirmed.
- Quarantine artifacts (HTA, scripts) for analysis.

## Evidence
- Sysmon/PowerShell logs, DNS logs, scheduled task XML, browser history.

## Eradication & Recovery
- Remove scheduled tasks, block outbound domains, clear autoruns.
- Review e-mail gateways for similar QR domains.

## Post-incident
- Tune detections; add block rules; user awareness on QR phishing.
