# 05 AI Security Foundations

AI security focuses on how AI systems can be misused, manipulated, or exposed through unsafe data handling, weak permissions, and poor guardrails.

## Prompt Injection

Prompt injection happens when an attacker crafts input that tries to override instructions, extract sensitive information, or change the system's intended behavior.

## Data Leakage

AI systems can leak sensitive data if prompts, retrieved context, logs, or outputs are not handled carefully. Privacy and confidentiality should be considered at every stage.

## Agent Permissions

AI agents become higher risk when they can take actions across tools and systems. The more permissions an agent has, the more important approval gates, scope limits, and auditability become.

## Guardrails

Guardrails are the policies and technical limits that reduce unsafe behavior. Examples include:

- human approval before high-impact actions
- restricted tool permissions
- clear system boundaries
- logging and review of actions
- output checks for sensitive or unsafe content

## AI Security Project Connection

These foundations connect directly to the `08-ai-prompt-injection-lab` project. That project can become a practical place to document prompt injection scenarios, guardrail design, and lessons about safe AI-assisted workflows.
