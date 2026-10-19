# Scope Analysis — Tabletop Scenario

**SIMULATED / TABLETOP ONLY.** Scope is unknown until evidence is collected. This document lists questions, not affected assets.

| Dimension | Evidence to validate | Current status |
|---|---|---|
| Endpoints | Host identifiers in original Windows, Sysmon, and SIEM records | REQUIRES VERIFICATION |
| Accounts | Target, subject, task principal, and group-member identities | REQUIRES VERIFICATION |
| Authentication | 4625/4624, logon type, source, destination, and authorization | REQUIRES VERIFICATION |
| Execution | Process image, parent, command line, hashes, and file context | REQUIRES VERIFICATION |
| Persistence / changes | Task XML, creation/update events, group/account changes | REQUIRES VERIFICATION |
| Lateral activity | Remote-service evidence on both endpoints | REQUIRES VERIFICATION |
| Data movement | Network telemetry, process attribution, destination, data context | REQUIRES VERIFICATION |
| Log integrity | Log-clear event/provider and remaining sources | REQUIRES VERIFICATION |

## Analysis guardrails

- Expand scope only when observable identifiers support the relationship.
- A successful RDP/SMB logon is not automatically a confirmed compromise.
- Outbound traffic is not automatically exfiltration; establish what moved and whether it was unauthorized.
- Distinguish missing telemetry from negative evidence.
- Record search window, time zone, sources, and collection gaps for reproducibility.
