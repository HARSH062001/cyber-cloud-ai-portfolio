# 03 SIEM Foundations

A Security Information and Event Management (SIEM) platform collects, normalizes, and analyzes logs so analysts can detect and investigate security events more efficiently.

## SIEM Purpose

The main purpose of a SIEM is to turn large volumes of log data into useful security visibility. It helps centralize events, correlate signals, and support monitoring and investigations.

## Alerts

Alerts are generated when rules, analytics, or detections match suspicious conditions. Good alerts are specific enough to be actionable without overwhelming analysts.

## Triage

Triage is the process of reviewing an alert to decide:

- is it real?
- how severe is it?
- what evidence supports it?
- what should happen next?

## False Positives

False positives are alerts that look suspicious but are actually benign. Reducing false positives matters because alert fatigue can waste time and cause real threats to be missed.

## Microsoft Sentinel Connection

Microsoft Sentinel is a cloud-native SIEM and SOAR platform. Learning SIEM foundations now supports the `05-microsoft-sentinel-soc-lab` project later by building the mindset needed for alert review, investigation, and detection understanding.

## Practical Focus

When building SIEM skill, I should practice:

- reading alerts clearly
- checking supporting evidence
- mapping activity to likely risk
- writing short analyst summaries
