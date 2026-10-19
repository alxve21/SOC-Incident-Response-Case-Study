# Incident Summary — Tabletop Scenario

> **SIMULATED / TABLETOP ONLY.** This is a hypothetical case for practicing L1 SOC triage and handoff. It does not describe a real incident or observed user environment.

## Situation

An alert queue contains a hypothetical sequence: repeated failed authentication, a possible successful remote logon, an Office-to-PowerShell process alert, possible script staging, scheduled-task and account/privilege-change indicators, remote-access activity on another host, an outbound transfer signal, and a Security log-cleared event. Relationships among the signals are unverified.

## Initial assessment

**Overall status: REQUIRES VERIFICATION.** No account compromise, lateral movement, persistence, exfiltration, or log tampering is confirmed by this outline. Validate each stage against its source, host, time, account, process lineage, and collection coverage.

## Priority questions

1. Are events from the same host/account and a consistent time window?
2. Does any 4624 match reviewed 4625 context?
3. What process, document, command line, and user context are visible?
4. Are task/account changes independently confirmed and authorized?
5. What does outbound telemetry show about process, destination, and data?
6. Is a Security log-clear event present, and what preceded it?

## Escalation posture

Preserve logs and volatile context where feasible, notify the incident lead, and follow authorized containment procedures. Isolate an endpoint or restrict an account only when evidence and impact justify the action and the authorized responder approves it. Do not declare breach based on this scenario alone.
