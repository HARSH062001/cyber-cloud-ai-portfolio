# 02 Cloud Logging Foundations

Cloud logging gives defenders visibility into what happened, when it happened, and which identity or resource was involved.

## CloudTrail

AWS CloudTrail records management activity and API actions. It is a core source for understanding account activity, policy changes, access behavior, and investigation timelines.

## GuardDuty

Amazon GuardDuty analyzes signals such as CloudTrail events, DNS activity, and other telemetry to surface suspicious behavior and possible threats. It helps move from raw logs toward security findings.

## Audit Logs

Audit logs create a record of administrative and security-relevant actions. They are important for incident response, internal review, and external compliance evidence.

## Detection Logic

Logs become useful when they support detection logic such as:

- unusual sign-in behavior
- policy or role changes
- repeated denied actions
- access from unexpected locations or services
- suspicious enumeration activity

## Why Logs Matter for SOC Work

SOC teams rely on logs to investigate alerts, validate timelines, and separate normal activity from malicious behavior. Without logs, analysts lose context and cannot explain what happened with confidence.

## Project Connections

Cloud logging foundations support future work in:

- `04-cloudtrail-log-analyzer`
- `07-guardduty-alert-parser`
- SOC and detection-oriented portfolio evidence
