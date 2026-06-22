# 02 Log Analysis Foundations

Logs are one of the most important sources of evidence in cybersecurity because they show what happened, when it happened, and which user, system, or process was involved.

## Why Logs Matter

Without logs, defenders lose visibility. With logs, analysts can investigate suspicious activity, confirm timelines, and support detection, triage, and reporting.

## Common Log Sources

### Windows Event Logs

Useful for authentication events, account changes, process activity, service changes, and other host-level evidence.

### Linux Auth Logs

Useful for login attempts, sudo activity, remote access behaviour, and authentication failures.

### Firewall Logs

Useful for network connections, blocked traffic, unusual destinations, and policy enforcement visibility.

### Web Server Logs

Useful for HTTP requests, user agents, status codes, suspicious access patterns, and application exposure.

### CloudTrail Logs

Useful for cloud account activity, API actions, identity changes, and administrative behaviour in AWS.

## Common Fields to Understand

- timestamp
- source IP
- destination IP
- username
- event ID
- action
- status

## Suspicious Patterns

- repeated failed logins
- successful login after many failures
- sign-in from unusual locations or times
- privilege changes
- disabled security controls
- unusual process execution
- large bursts of denied actions
- unexpected access to admin interfaces

## Practical Mini-Labs I Can Build

- compare normal versus suspicious login events
- review Windows security event examples
- inspect Linux authentication failure patterns
- parse simple web server logs for unusual requests
- review sample CloudTrail events for risky activity
- write short analyst summaries from example logs
