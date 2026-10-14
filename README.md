# SSH-Brute-Force-Investigation-Splunk
SOC lab project for analyzing SSH authentication logs, detecting brute-force patterns, and documenting incident response using Splunk.

## Project Overview
This project explores how a SOC analyst can investigate suspected SSH brute-force activity using Linux authentication logs and Splunk. 
The objective is to identify repeated failed login attempts, examine source IPs and targeted accounts, establish an event timeline, and document defensive recommendations.

## Objectives
- Analyze Linux SSH authentication events.
- Identify repeated failed login patterns and suspicious source IPs.
- Use Splunk searches to investigate security events.
- Map observed behavior to MITRE ATT&CK.
- Prepare an incident report with evidence and remediation recommendations.

## Investigation Workflow
1. Prepare a controlled Linux lab.
2. Generate or obtain clearly labelled test authentication logs.
3. Ingest the logs into Splunk.
4. Search for repeated failed logins and group events by source IP and username.
5. Review timestamps and check for any successful login following the failures.
6. Map supported findings to MITRE ATT&CK technique T1110 — Brute Force.
7. Document findings, limitations, and recommended mitigations.

## Tools and Technologies
- Kali Linux / Linux authentication logs
- Splunk Enterprise
- Search Processing Language (SPL)
- MITRE ATT&CK
- GitHub

## Detection Ideas
- Repeated authentication failures within a short period.
- Multiple targeted usernames from one source IP.
- A successful login following repeated failures.
- Unusual authentication patterns requiring further investigation.

## Recommended Defensive Actions
- Review and restrict SSH access.
- Use SSH keys and disable password authentication where appropriate.
- Apply rate limiting or other brute-force protections.
- Monitor authentication logs and investigate suspicious activity.
- Follow organizational incident-response procedures.

## Project Status
Lab project in progress. Detection results, screenshots, sample logs, and incident findings will be added after validation in a controlled environment.

## Disclaimer
This project is intended for defensive security learning and authorized lab testing only. Any sample data must be clearly labelled and must not be presented as evidence of a real-world incident.
