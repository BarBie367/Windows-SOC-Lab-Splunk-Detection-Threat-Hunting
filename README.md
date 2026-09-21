# Windows SOC Lab – Splunk Detection, Threat Hunting & Incident Response
A hands-on SOC lab built on Windows 10 using Splunk, Windows Event Logs, and Sysmon to practice security monitoring, threat hunting, detection engineering, event correlation, alerting, and incident investigation.

# Windows SOC Lab – Splunk Detection, Threat Hunting & Incident Response

## Overview

A hands-on Security Operations Center lab built on Windows 10
using Splunk, Windows Event Logs, and Sysmon.

The project demonstrates security monitoring, log analysis,
detection engineering, threat hunting, event correlation,
alerting, and incident investigation.

## Objectives

- Collect and analyze Windows security telemetry
- Monitor authentication activity
- Detect suspicious behavior
- Create SPL-based security detections
- Investigate and correlate security events
- Map findings to MITRE ATT&CK
- Build a SOC monitoring dashboard
- Document security incidents

## Lab Architecture

[Insert architecture diagram here]

## Technologies

- Splunk Enterprise
- Splunk Forwarder
- Windows 10
- Windows Event Viewer
- Sysmon
- SPL
- PowerShell
- MITRE ATT&CK

## Data Sources

| Data source | Description |
|-------------|-------------|
| Windows Security Logs | Authentication and account activity |
| Windows System Logs | Operating system events |
| Windows Application Logs | Application-related events |
| Sysmon | Process, file, and network telemetry |
| PowerShell Logs | PowerShell activity |

## Project Phases

1. Lab setup and data collection
2. Log analysis and field extraction
3. Authentication investigation
4. Detection engineering
5. Threat hunting
6. Event correlation
7. MITRE ATT&CK mapping
8. Alert configuration
9. Dashboard development
10. Incident reporting

## Detections

| Detection | Event IDs | ATT&CK |
|-----------|-----------|--------|
| Multiple failed logons | 4625 | T1110 |
| Failed logons followed by success | 4625, 4624 | T1110 |
| Suspicious PowerShell | Sysmon, PowerShell | T1059.001 |
| New local user | 4720 | T1136.001 |
| Privileged group modification | 4732 | T1098 |

## Investigations

### INC-001 – Authentication Anomaly

Summary:

Three failed interactive logon attempts against the `admin`
account were followed by a successful authentication.

The activity originated from localhost and requires further
investigation.

| report |

## Dashboard

| Dashboard screen |

## Limitations

This project was conducted in a single-machine Windows 10 lab.
It does not represent a full enterprise environment with
multiple endpoints, Active Directory, or centralized network
infrastructure.

## Disclaimer

All activities were performed in a controlled personal lab
for educational and defensive security research purposes.
