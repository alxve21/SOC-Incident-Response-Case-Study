# Triage Notes — Tabletop Scenario

**SIMULATED / TABLETOP ONLY.** This is a workflow for a hypothetical alert sequence, not a record of an actual queue.

## L1 triage sequence

1. **Validate:** confirm product, rule, provider/event ID, host, user, timestamp and time zone; preserve the original record.
2. **Scope:** identify candidate endpoints and accounts from evidence and search a bounded window. Do not assume all stages occurred.
3. **Authentication:** compare 4625 and 4624 context; confirm logon type, source, destination, and authorization.
4. **Execution:** inspect Office/PowerShell lineage and command context; verify file/script evidence separately.
5. **Changes:** validate scheduled task configuration and account/group changes against approved administration.
6. **Network:** distinguish a connection or transfer signal from confirmed exfiltration. Identify process, destination, transfer details, and data context.
7. **Log integrity:** verify the log-clear signal and preserve other available telemetry.
8. **Document uncertainty:** classify each stage separately as CONFIRMED, LIKELY, SUSPICIOUS, POSSIBLE, NOT OBSERVED IN AVAILABLE DATA, or REQUIRES VERIFICATION.

## Evidence handling

Record source, collection time, investigator, export method, time zone, and any redaction. Preserve originals where authorized and keep working copies separate. Do not place secrets or personal information in this public portfolio.

## Escalation

Escalate to the incident lead when unauthorized access is supported, a privileged change is unexplained, evidence may be lost, or multiple systems may be in scope. L1 should not perform disruptive containment outside delegated authority.
