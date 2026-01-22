# Incident Report: Lateral Movement and Privilege Abuse

## Incident Summary
Suspicious lateral movement activity was detected involving multiple systems, followed by abnormal privileged account usage, indicating a potential post-compromise escalation attempt.

---

## Incident Details
- Incident Type: Lateral Movement / Privilege Abuse
- Severity: High
- Detection Sources: Splunk SIEM
- Affected Environment: On-Prem Windows Systems

---

## Detection Overview
The incident was identified through correlated alerts detecting abnormal RDP and SMB authentication activity across multiple hosts, combined with privileged account usage outside normal patterns.

---

## Affected Assets
- Multiple Windows endpoints
- Privileged user account(s)

---

## Investigation Timeline
1. Alert triggered for RDP/SMB access to multiple hosts
2. Analyst identified reuse of same credentials across systems
3. Privileged account usage detected shortly after lateral access
4. No approved administrative activity found
5. Incident escalated due to elevated risk

---

## Indicators of Compromise (IOCs)
- Logon Type 3 and 10 events across multiple hosts
- Privileged account authentication from unusual source
- Sequential access patterns inconsistent with baseline behavior

---

## Root Cause Analysis
The activity was consistent with credential compromise followed by lateral movement and attempted privilege escalation.

---

## Containment Actions
- Isolated affected systems
- Reset credentials for impacted accounts
- Temporarily restricted privileged access

---

## Remediation & Recommendations
- Enforce least privilege access
- Monitor lateral movement patterns continuously
- Review administrative access policies

---

## Lessons Learned
- Cross-log correlation improves early detection
- Privileged account monitoring is critical post-compromise
