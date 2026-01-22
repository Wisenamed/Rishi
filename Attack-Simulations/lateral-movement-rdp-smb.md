# Attack Simulation: Lateral Movement via RDP and SMB

## Objective
Simulate attacker lateral movement using valid credentials to access multiple systems within the environment.

---

## Attack Scenario
After initial access, an attacker attempts to move laterally by authenticating to other systems using RDP and SMB.

---

## Simulated Attacker Actions
- Authentication attempts to multiple hosts
- Use of the same credentials across systems
- Access from non-standard source machines

---

## Observed Telemetry
- Windows authentication events (Logon Type 3 and 10)
- Multiple host access within short time window
- Reuse of credentials across endpoints

---

## SOC Visibility
- Detection of abnormal authentication patterns
- Correlation across hosts
- Escalation due to lateral movement indicators

---

## Defensive Outcome
- Lateral movement detected early
- Credentials rotated
- Affected systems monitored for follow-on activity
