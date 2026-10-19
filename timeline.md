# Timeline — Tabletop Sequence

> **SIMULATED / TABLETOP ONLY.** These stages are hypothetical. No timestamps, usernames, hosts, IP addresses, counts, or event records are assigned to the hypothetical stages. Separate local Splunk observations are documented in the repository README and do not populate this timeline.

| Order | Hypothetical signal | Starting status | Validation needed |
|---|---|---|---|
| 1 | Failed authentication | REQUIRES VERIFICATION | Confirm Security 4625, source, targets, host, and window |
| 2 | Possible successful remote logon | REQUIRES VERIFICATION | Validate 4624, logon type, account, source, destination, and authorization |
| 3 | Office-launched PowerShell | REQUIRES VERIFICATION | Review Sysmon 1/4688, lineage, command line, user, and document context |
| 4 | Possible script staging | REQUIRES VERIFICATION | Validate file path, hash, creator, and execution relationship |
| 5 | Task or account/privilege change | REQUIRES VERIFICATION | Confirm task details and applicable account/group events; identify actor and approval |
| 6 | Lateral-movement indicator | REQUIRES VERIFICATION | Confirm source/destination records and remote-service context |
| 7 | Outbound transfer signal | REQUIRES VERIFICATION | Identify telemetry source, process, destination, transfer and data context |
| 8 | Security log cleared indicator | REQUIRES VERIFICATION | Verify provider/event and preserve surrounding evidence |

## Correlation notes

Populate timestamps only in a separate evidence-backed exercise. Normalize time zones and record source clock. Correlate by host, account, source/destination, process identifiers, and event details; order alone is insufficient. If absent, label **NOT OBSERVED IN AVAILABLE DATA** or **REQUIRES VERIFICATION**, not “did not happen.”
