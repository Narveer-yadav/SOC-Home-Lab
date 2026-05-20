Incident Title: Security Audit Log Cleared Detected

Date & Time:
02/05/2026  10:23:25 PM

Alert Type:
Anti-Forensics Activity / Audit Log Deletion

Description:
A Security audit log clearing event was detected on the Windows system. Event ID 1102 was triggered, indicating that the Windows Security log was manually cleared. This behavior is considered highly suspicious because attackers often delete logs to remove evidence of malicious activity and avoid detection.

Affected Host:
Narveer

Event ID:
1102

User Account:
narveer

Severity:
High

Analysis:
Splunk Security logs showed Event ID 1102, confirming that the Security event log was cleared. This activity is uncommon during normal operations and is often associated with anti-forensics techniques used by attackers after unauthorized access, privilege escalation, or malicious actions. The event should be investigated immediately to determine whether it was performed by an authorized administrator or suspicious actor.

Recommended Action:
Verify the user who cleared the logs and confirm whether the action was legitimate. Review previous authentication events, suspicious process activity, and related alerts before the log deletion. Restrict unnecessary administrative access and enable monitoring for repeated log-clearing attempts.
