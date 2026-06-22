# 01 IAM Foundations

Identity and Access Management (IAM) is one of the most important foundations in cloud security because it controls who can access what, how they access it, and what actions they are allowed to perform.

## Authentication vs Authorization

Authentication answers: who are you?

Authorization answers: what are you allowed to do?

A user might authenticate successfully with a password, MFA, or single sign-on, but still should not be authorized to perform sensitive actions unless their permissions explicitly allow it.

## Core IAM Components

### Users

Users represent individual identities. In AWS, long-term IAM users should be handled carefully because static credentials create security risk if they are over-permissioned or exposed.

### Groups

Groups help assign permissions to multiple users consistently. Instead of attaching many custom permissions to each user, groups make access management easier to review and maintain.

### Roles

Roles are identities that can be assumed temporarily by users, services, or workloads. Roles are safer than sharing long-term credentials because they support temporary access and clearer trust relationships.

### Policies

Policies define what actions are allowed or denied. In AWS, policies are JSON documents that describe actions, resources, and effects such as Allow or Deny.

## Least Privilege

Least privilege means giving only the permissions required to perform a task and nothing more. This reduces blast radius if an account is compromised, misused, or configured incorrectly.

Practical least-privilege review questions:

- Does this identity need every action in the policy?
- Does this identity need access to every resource listed?
- Can broad wildcard permissions be narrowed?
- Can temporary role access replace long-term standing access?

## MFA

Multi-factor authentication adds a second layer beyond just a password. MFA is critical for administrator or privileged access because stolen passwords are common and often lead directly to account compromise.

## Privilege Escalation Risk

Privilege escalation happens when an identity can gain more power than intended. In cloud IAM, this can happen through overly broad permissions, risky role assumptions, policy editing rights, or the ability to create new keys, roles, or attached policies.

Common warning signs:

- wildcard permissions such as `*:*`
- permission to attach or edit policies
- permission to assume high-privilege roles
- permission to create access keys or new identities without strong controls

## AWS IAM Beginner Lab Plan

This is a safe learning plan only. It does not require real production access.

1. Read sample IAM policy JSON files and identify actions, resources, and effects.
2. Compare a broad policy with a narrower least-privilege version.
3. Mark risky statements such as wildcard actions or wildcard resources.
4. Create a simple checklist for reviewing users, groups, roles, and policies.
5. Document findings in a short report format for GitHub evidence.

## Security+ Connection

IAM supports several Security+ themes:

- identification and authentication
- access control models
- account management
- least privilege
- multifactor authentication
- privilege abuse and insider risk

## GRC Connection

IAM is also a governance and control topic because organizations must define who should have access, review whether access is appropriate, and retain evidence that access controls are working.

GRC links include:

- access review processes
- segregation of duties
- privileged access oversight
- evidence for audits and control testing

## SOC and Logging Connection

IAM activity matters to defenders because identity abuse often appears in logs before a major incident is visible elsewhere.

Important logging connections:

- sign-in events
- failed access attempts
- policy changes
- new user or role creation
- suspicious privilege escalation behavior

## Interview Questions

- What is the difference between authentication and authorization?
- Why is least privilege important in cloud environments?
- What is the difference between an IAM user and an IAM role?
- Why can wildcard permissions create risk?
- How does MFA reduce account compromise risk?
- What IAM events would you want to monitor in logs?

## Project Connection: 03 IAM Permissions Auditor

The `03-iam-permissions-auditor` project will turn these foundations into practical portfolio evidence by reviewing IAM structures, flagging overly broad access, and documenting access-risk findings in a beginner-friendly way.
