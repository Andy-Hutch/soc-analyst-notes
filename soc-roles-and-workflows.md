# SOC Roles and Workflows – SOC Level 1

## Purpose
Understanding the Security Operations Center (SOC) structure and workflows is essential for a SOC L1 analyst. This knowledge helps you **know who to escalate alerts to, how incidents flow through the team, and how each role contributes to defending the organization**.

---

## SOC Team Structure

| Role | Responsibilities |
|------|-----------------|
| **SOC L1 Analyst** | First line of defense; triages alerts, investigates basic incidents, escalates complex cases |
| **SOC L2 Analyst** | Handles complex alerts escalated from L1; performs deep-dive analysis and incident investigation |
| **SOC Engineer** | Configures and maintains security tools (SIEM, EDR, IDS/IPS); ensures alerts and systems function properly |
| **SOC Manager** | Oversees SOC operations, manages team performance, reports to senior management |
| **CERT / Incident Response Lead** | Coordinates response to critical incidents, performs advanced forensic analysis, manages communication with stakeholders |
| **Threat Researcher** | Analyzes malware, threat actors, and emerging campaigns; supports SOC with intelligence and context |
| **GRC Auditor** | Ensures compliance with regulations, evaluates security policies, audits controls |
| **Penetration Tester (Red Team)** | Identifies vulnerabilities and tests defenses; not part of SOC but helps improve detection capabilities |

---

## SOC Workflows

### 1. Alert Handling
1. **Detection:** SIEM or EDR generates an alert  
2. **Triage (L1):** L1 analyst validates alert, identifies impacted assets, and determines severity  
3. **Escalation:** L1 escalates confirmed incidents to L2, CERT, or SOC Engineer as needed  
4. **Resolution:** Incident is contained, eradicated, and systems restored  
5. **Documentation:** Actions, evidence, and lessons learned are recorded  

### 2. Incident Response
1. **Initial Response:** SOC L1 identifies incident and collects initial evidence  
2. **Analysis:** SOC L2, CERT, or Threat Researcher investigates  
3. **Containment & Mitigation:** Isolate affected systems, block malicious IPs, stop malware spread  
4. **Recovery:** Restore systems from backups, verify integrity  
5. **Post-Incident Review:** Update playbooks, detection rules, and lessons learned  

### 3. Escalation Guidelines
- L1 handles routine alerts and low-complexity incidents  
- Escalate if:  
  - Incident affects critical systems or data  
  - Malware or ransomware detected  
  - Alert requires advanced analysis or forensics  
- Always provide detailed context and evidence to L2/CERT  

---

## Example Scenario

**Incident:** Multiple employees report suspicious emails containing attachments  

**Workflow:**
1. **L1 Analyst:** Triage alerts, check headers, verify attachments  
2. **L2 Analyst:** Investigates suspicious attachments in sandbox  
3. **Threat Researcher:** Analyzes malware variant and threat actor  
4. **SOC Engineer:** Ensures mail gateway blocks sender domain  
5. **SOC Manager:** Monitors overall response, communicates status to management  

**Outcome:** Phishing campaign contained, affected users secured, detection rules updated  

---

## Best Practices
- Understand each team member’s role to **escalate correctly**  
- Document everything clearly for **traceability and audits**  
- Learn from each incident to improve detection and response  
- Stay aware of cross-functional workflows with IT, Threat Intel, and GRC teams  
- Communicate effectively: a SOC is a **team effort**

---

## Skills Demonstrated
- Knowledge of SOC team structure and responsibilities  
- Understanding of alert and incident workflows  
- Escalation decision-making  
- Collaboration across SOC roles and external teams  
- Documentation for audits and incident tracking

