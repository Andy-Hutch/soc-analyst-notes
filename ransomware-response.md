# Ransomware Response – SOC Level 1

## Purpose
Ransomware is one of the most severe cybersecurity incidents a SOC analyst can face. The goal of ransomware response is to **contain the attack, minimize damage, investigate the source, and support recovery**.  

As a SOC L1 analyst, your role is often **initial detection, triage, and escalation** to SOC L2, CERT, and incident response teams.

---

## Typical Indicators of Ransomware
- Endpoint EDR alerts for encryption activity
- Unexpected file renaming or extension changes
- Suspicious network traffic to unknown destinations
- User reports of inaccessible files
- High CPU/disk usage on multiple systems

---

## Ransomware Response Workflow

1. **Detection**
   - Receive alerts from SIEM or EDR
   - Correlate logs to confirm ransomware activity
   - Identify affected users, endpoints, and network segments

2. **Containment**
   - Isolate infected systems from the network
   - Disable compromised accounts temporarily
   - Block malicious IPs and domains
   - Stop lateral movement if possible

3. **Investigation**
   - Collect malware hashes and indicators
   - Identify the ransomware variant (if possible)
   - Review EDR/endpoint logs for infection timeline

4. **Escalation**
   - Escalate to SOC L2 or CERT for deeper forensic analysis
   - Provide all collected evidence, endpoints, and logs

5. **Eradication & Recovery**
   - Remove ransomware and malicious files
   - Restore systems from clean backups
   - Verify system integrity

6. **Post-Incident Review**
   - Document timeline, response actions, and lessons learned
   - Update detection rules to prevent recurrence
   - Share intelligence with the team

---

## Roles Involved
| Role | Responsibilities |
|------|-----------------|
| SOC L1 Analyst | Initial alert triage, containment, evidence collection |
| SOC L2 Analyst | Deep technical analysis, malware investigation, endpoint remediation |
| SOC Engineer | Ensure security tools are functioning, check logs, support containment measures |
| CERT / Incident Response Lead | Coordinate incident response, manage communications, oversee eradication and recovery |
| Threat Researcher | Analyze ransomware variant, gather intelligence, recommend defensive measures |

---

## Example Scenario
**Incident:** Office in France hit with ransomware, multiple endpoints encrypted  

**Steps Taken as SOC L1:**  
1. Reviewed SIEM alert and confirmed multiple endpoints affected  
2. Isolated affected endpoints from the network  
3. Collected malware hashes and screenshots of ransom note  
4. Escalated to SOC L2 and CERT for investigation and recovery  

**Outcome:** Contained the ransomware, endpoints restored from backups, and new detection rules created to prevent recurrence  

---

## Best Practices
- Prioritize containment first to stop spread  
- Document everything for legal and audit purposes  
- Maintain clear communication with team and management  
- Work quickly, but follow SOPs to avoid mistakes  
- Learn from every incident: Update playbooks and detection rules  

---

## Skills Demonstrated
- Ransomware detection and containment  
- Coordination with SOC team and CERT  
- Incident triage and escalation  
- Evidence collection for forensic analysis  
- Post-incident review and preventative action
