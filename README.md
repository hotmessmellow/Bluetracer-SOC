# BlueTrace – QR4Beacon Scenario Pack

A unique SOC/IR lab scenario that correlates **email → DNS → PowerShell** signals for a QR-driven phishing campaign.
Please use for educational purposes/training and meant for **isolated lab** use only.

## Scenario (QR4Beacon)
- A user scans a QR code from a flyer and types the shown URL on their workstation.
- The URL serves a **benign-looking page** but attempts to launch **mshta** to fetch a remote HTA.
- The HTA triggers **PowerShell** with an **EncodedCommand** that beacons via DNS subdomains to a high-entropy domain.
- Persistence is attempted via a **scheduled task**.

## What’s included
- Sigma rules for PowerShell, mshta/certutil, scheduled tasks, and high-entropy DNS.
- Microsoft Sentinel KQL: detection, **beaconing periodicity**, and **email→endpoint** correlation examples.
- Sample logs (XML/CSV) to replay/import into your SIEM.
- IR runbook and a quick 90-second demo script.
- Alert explainability card template (how to document “why this fired”).

## Ethics
Use only with consent in a controlled lab environment. This pack contains **synthetic samples** and detection content.
