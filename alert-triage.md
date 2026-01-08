# Alert Triage – SOC Level 1

## Purpose
Alert triage is the first step in handling potential security incidents. The goal is to quickly assess alerts from SIEM, EDR, or other monitoring tools, determine if they are true threats, and escalate them if necessary.

As a SOC L1 analyst, your job is to **filter noise from real threats** and ensure incidents are addressed in a timely and effective manner.

---

## Typical Alert Sources
- Firewall logs (e.g., brute-force attempts, port scanning)
- Endpoint Detection & Response (EDR) alerts
- Intrusion Detection/Prevention System (IDS/IPS) events
- Authentication logs (failed logins, account lockouts)
- Web and application security alerts
- Threat intelligence feeds

---

## Alert Triage Workflow

1. **Initial Review**
   - Check alert details: timestamp, source/destination IP, affected user or system
   - Identify the alert type (malware, phishing, brute force, suspicious login, etc.)
   - Evaluate severity and urgency

2. **Validation**
   - Cross-reference source/destination IP with threat intelligence
   - Compare against historical alerts for repeated patterns
   - Check user/system behavior for anomalies

3. **Investigation**
   - Examine logs or endpoint data to confirm suspicious activity
   - Determine if the alert is a false positive or a true incident
   - Document observations clearly

4. **Escalation**
   - If confirmed or complex: escalate to SOC L2 or CERT
   - Include all collected evidence and steps taken

5. **Resolution & Documentation**
   - Record the action taken
   - Update alert ticket status
   - Recommend preventative actions if applicable

---

## Example Scenarios

### Scenario 1: Firewall Brute-Force
**Alert:** Multiple failed login attempts on `FW-NY-01` firewall  
**Steps Taken:**
- Verified failed attem
