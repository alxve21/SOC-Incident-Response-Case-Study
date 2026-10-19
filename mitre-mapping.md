# MITRE ATT&CK Mapping — Conditional

**SIMULATED / TABLETOP ONLY.** These are investigation candidates, not findings that behavior occurred.

| Hypothetical behavior | Candidate technique | Evidence required before mapping as observed |
|---|---|---|
| Repeated password attempts | [T1110 — Brute Force](https://attack.mitre.org/techniques/T1110/) | Authentication records supporting a pattern across accounts |
| Successful use of an account | [T1078 — Valid Accounts](https://attack.mitre.org/techniques/T1078/) | Verified unauthorized account use with endpoint/source context |
| PowerShell execution | [T1059.001 — PowerShell](https://attack.mitre.org/techniques/T1059/001/) | Process telemetry and context supporting the behavior |
| Scheduled task | [T1053.005 — Scheduled Task](https://attack.mitre.org/techniques/T1053/005/) | Verified task action, principal, trigger, and unauthorized purpose |
| Remote services | [T1021 — Remote Services](https://attack.mitre.org/techniques/T1021/) | Evidence of a specific remote service in an unauthorized sequence |
| Data transfer | [T1041 — Exfiltration Over C2 Channel](https://attack.mitre.org/techniques/T1041/) | Evidence of unauthorized transfer and channel; outbound traffic alone is insufficient |
| Security log cleared | [T1070.001 — Clear Windows Event Logs](https://attack.mitre.org/techniques/T1070/001/) | Verified log-clear event and context |

Record evidence and confidence per mapping. Remove unsupported mappings; this table is not an alert conclusion.
