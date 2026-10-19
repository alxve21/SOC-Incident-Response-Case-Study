# Containment and Response — Tabletop Plan

**SIMULATED / TABLETOP ONLY.** This is a decision framework, not an instruction or record of a change to any real system.

## Before containment

- Notify the incident lead and confirm authority, business impact, and system owner.
- Preserve relevant records and volatile context where feasible; capture system time details.
- Record evidence supporting each action and the likely operational impact.
- Maintain chain-of-custody notes for collected exports or images.

## Conditional actions

| Evidence-supported condition | Candidate action with incident-lead approval |
|---|---|
| Active unauthorized remote access on an identified endpoint | Isolate through the approved response process while preserving telemetry |
| Confirmed compromised account | Restrict/reset the specific account through authorized identity process; preserve logon evidence where feasible |
| Unauthorized task or group membership | Preserve details, then disable/remove the confirmed change through change control |
| Confirmed malicious file/script | Preserve a forensic copy and metadata before quarantine/removal under policy |
| Suspected outbound data transfer | Engage network/data owners to validate destination and content; scope any control |
| Possible log clearing | Preserve remaining endpoint, forwarded, and SIEM copies; escalate integrity concerns |

## Recovery and follow-up

Document action, approver, time, asset, outcome, and rollback steps. Recover only under the incident process. Close with verified scope, uncertainty, monitoring needs, and lessons. No containment is recorded as completed in this tabletop artifact.
