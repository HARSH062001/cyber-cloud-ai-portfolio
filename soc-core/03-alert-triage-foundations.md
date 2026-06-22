# 03 Alert Triage Foundations

Alert triage is the process of examining a security alert to decide whether it matters, how urgent it is, and what action should happen next.

## What an Alert Is

An alert is a signal produced by a rule, analytic, or tool when activity matches suspicious conditions.

## Severity vs Priority

Severity reflects the potential technical impact of the alert.

Priority reflects how urgently the organisation needs to respond based on business context, affected assets, and confidence level.

## Triage Workflow

1. Read the alert clearly.
2. Identify what triggered it.
3. Review affected user, host, account, or asset.
4. Check supporting logs and context.
5. Decide whether it looks benign, suspicious, or confirmed malicious.
6. Document findings.
7. Escalate if needed.

## Confirming True Positive vs False Positive

Questions to ask:

- Is the activity expected for this user or system?
- Does the alert match known benign behaviour?
- Are there supporting logs that increase confidence?
- Is there evidence of policy violation or compromise?

## Evidence Collection

Useful evidence may include:

- timestamps
- IP addresses
- usernames
- device or hostname
- related log entries
- screenshots of the alert view
- search results from SIEM or EDR tools

## When to Escalate

Escalate when:

- impact appears high
- sensitive assets are involved
- malicious behaviour seems likely
- containment may be needed
- the case exceeds entry-level scope

## Example Triage Template

- Alert name:
- Date and time:
- Severity:
- Affected user or asset:
- Summary of activity:
- Key evidence:
- True positive, false positive, or inconclusive:
- Escalation needed:
- Next action:
