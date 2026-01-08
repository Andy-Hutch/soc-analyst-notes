# SIEM Basics – SOC Level 1

## Purpose
A Security Information and Event Management (SIEM) system is a **central tool for monitoring, analyzing, and responding to security events** across an organization. As a SOC L1 analyst, your role is to **monitor SIEM alerts, validate potential threats, and escalate incidents** as needed.

---

## Key SIEM Concepts

### What SIEM Does
- Collects logs from multiple sources (network, endpoints, servers, applications)
- Correlates events to detect patterns and suspicious activity
- Generates alerts for potential security incidents
- Provides dashboards and reporting for SOC analysts

### Common SIEM Log Sources
- Firewall logs (connection attempts, blocked traffic)
- Intrusion Detection/Prevention Systems (IDS/IPS)
- Endpoint Detection & Response (EDR) tools
- Active Directory authentication logs
- Web server logs
- VPN and remote access logs
- Cloud service logs (AWS CloudTrail, Azure AD, etc.)

### Types of Alerts
- Brute-force attacks
- Malware or ransomware detection
- Suspicious login locations or failed logins
- Data exfiltration or large file transfers
- Policy violations (USB usage, admin privilege changes)

---

## SIEM Workflow for L1 Analysts

1. **Monitoring**
   - Review dashboards and alert queues
   - Prioritize alerts based on severity and impacted assets

2. **Validation**
   - Examine logs and correlating events
   - Confirm if the alert is real or false positive
   - Use threat intelligence for context

3. **Investigation**
   - Review impacted endpoints and accounts
   - Check related network traffic or authentication events
   - Collect evidence for escalation

4. **Escalation**
   - Escalate confirmed incidents to SOC L2, CERT, or engineers
   - Provide all gathered logs and context

5. **Documentation**
   - Record all findings and actions in the ticketing system
   - Update alert status (false positive, escalated, resolved)

---

## Troubleshooting Common SIEM Issues

- **High false positive rate**
  - Review and tune correlation rules
  - Check for misconfigured log sources

- **Missing or delayed logs**
  - Verify log forwarding from endpoints
  - Ensure SIEM connectors are active and healthy

- **Alert overload**
  - Prioritize alerts based on business impact
  - Use dashboards to focus on critical events

- **Storage or performance issues**
  - Check SIEM server health
  - Alert SOC engineers to investigate storage or indexing problems

---

## Best Practices
- Always validate alerts before acting  
- Focus on high-risk or critical systems first  
- Collaborate with L2 analysts and engineers when unsure  
- Document findings thoroughly for future reference  
- Continuously learn the SIEM platform to improve efficiency  

---

## Skills Demonstrated
- Log source knowledge across multiple platforms  
- Alert triage and validation using SIEM  
- Incident escalation workflow understanding  
- Troubleshooting SIEM issues and optimizing alert quality  
- Documentation for SOC operations and audits

