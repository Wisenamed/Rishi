# SOC Runbook: Cloud Resource Abuse Response

## Trigger
Alerts indicating anomalous Azure resource provisioning or subscription abuse.

---

## Initial Triage
1. Identify affected subscription and resources
2. Review user or service principal activity
3. Confirm business justification

---

## Investigation Steps
1. Review Azure Activity Logs
2. Validate RBAC permissions
3. Check for identity compromise indicators
4. Assess cost and security impact

---

## Containment Actions
- Disable affected account or service principal
- Remove unauthorized resources
- Restrict permissions temporarily

---

## Escalation Criteria
- High-cost or large-scale resource abuse
- Privileged roles involved
- Repeated abuse attempts

---

## Post-Incident Actions
- Improve cloud monitoring rules
- Apply stricter RBAC
- Update cloud security policies
