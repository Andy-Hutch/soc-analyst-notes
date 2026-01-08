# Phishing Analysis – SOC Level 1

## Purpose
Phishing analysis focuses on identifying malicious emails, links, or attachments that attempt to steal credentials, deliver malware, or compromise company systems. As a SOC L1 analyst, your role is to **detect, validate, and escalate phishing incidents** before they impact the organization.

---

## Indicators of Phishing
- Suspicious sender email or domain (spoofing)
- Mismatched URLs and displayed text
- Unexpected attachments (e.g., macro-enabled documents)
- Urgent or threatening language
- Poor grammar or unusual formatting
- Reports from employees who clicked suspicious links

---

## Phishing Analysis Workflow

1. **Initial Review**
   - Identify sender, recipient, and email headers
   - Check subject and content for suspicious indicators
   - Note any attachments or embedded links

2. **Validation**
   - Check sender against known safe/blacklisted domains
   - Verify URLs using threat intelligence or sandbox
   - Check for attachment hashes in malware databases

3. **Investigation**
   - Detonate attachments in sandbox (if available)
   - Inspect network or endpoint behavior after click/open
   - Identify impacted users or systems

4. **Escalation**
   - If confirmed malicious: escalate to SOC L2, CERT, or Threat Researcher
   - Include all evidence, screenshots, and analysis steps

5. **Mitigation & Documentation**
   - Block sender or domain in email gateway
   - Quarantine affected emails
   - Notify impacted users to reset credentials
   - Record all actions in ticketing system

---

## Example Scenarios

### Scenario 1: Employee Clicked Malicious Link
**Alert:** User `anna.hr` clicked on a suspicious link claiming to be payroll update  
**Steps Taken:**
- Checked email headers for spoofing  
- Verified URL in threat intelligence (malicious domain)  
- Confirmed user clicked link, endpoint showed no compromise yet  
**Action:** Escalated to SOC L2 for endpoint monitoring and isolation  

### Scenario 2: Malicious Attachment
**Alert:** HR received an email with `PayrollUpdate.docm` attachment  
**Steps Taken:**
- Verified sender domain  
- Sandbox detonation confirmed macro downloads malware  
- Determined potentially impacted endpoints  
**Action:** Escalated to CERT and SOC L2, blocked sender domain, quarantined emails

### Scenario 3: Targeted Phishing Campaign
**Alert:** Multiple employees report similar suspicious emails  
**Steps Taken:**
- Correlated logs across mail server  
- Collected attachments and URLs  
- Confirmed phishing campaign pattern  
**Action:** Escalated to SOC L2 and Threat Researcher, blocked campaign indicators

---

## Best Practices
- Always validate before acting: False positives are common  
- Document each step: Key for escalations and audits  
- Prioritize high-risk targets (finance, HR, executives)  
- Use threat intelligence: Know known phishing campaigns  
- Communicate with impacted users: Quick action reduces risk  

---

## Skills Demonstrated
- Email and attachment analysis  
- Log correlation for phishing detection  
- Escalation protocols to L2, CERT, and Threat Researcher  
- Endpoint awareness and sandbox usage  
- Documentation suitable for audits and incident reports  
