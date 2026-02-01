# SOC Playbook – OSINT & Brand Threat Response

## Purpose
This playbook outlines how a **Security Operations Center (SOC)** would detect, investigate, and respond to threats identified through OSINT reconnaissance.

It aligns OSINT findings to **real-world SOC workflows**, bridging intelligence analysis with operational response.

---

## Trigger Conditions
This playbook is activated when:

- New phishing domains are detected
- Brand impersonation reports are received
- Suspicious emails referencing the organization appear
- OSINT monitoring flags new infrastructure or identity exposure

---

## Phase 1: Detection & Alerting

### Data Sources
- OSINT feeds (Hunter.io, Shodan, VirusTotal)
- User-reported phishing emails
- Brand monitoring tools
- DNS and certificate transparency logs

### Alerts Generated
- Newly registered look-alike domains
- Spike in email impersonation attempts
- Reputation changes on known domains
- External exposure of sensitive documents

---

## Phase 2: Triage

**SOC Analyst Actions:**
1. Validate alert legitimacy
2. Correlate OSINT indicators with internal telemetry
3. Assess scope and potential impact
4. Assign severity level

**Severity Guidelines:**
- Low: Informational OSINT exposure
- Medium: Active phishing indicators
- High: Credential harvesting or impersonation confirmed

---

## Phase 3: Investigation

### Investigation Steps
- Analyze phishing emails or URLs
- Validate indicators in VirusTotal
- Review DNS and hosting information
- Identify affected users or systems

### Key Questions
- Is the threat active or historical?
- Are credentials at risk?
- Is brand trust being abused?
- Has user interaction occurred?

---

## Phase 4: Containment & Response

### Response Actions
- Block malicious domains and URLs
- Disable compromised accounts
- Reset credentials if required
- Issue takedown requests for phishing infrastructure

### Coordination
- Work with legal and brand protection teams
- Notify email security providers
- Engage hosting or domain registrars

---

## Phase 5: Recovery

- Confirm removal of malicious content
- Monitor for re-emergence
- Validate user account security
- Restore normal operations

---

## Phase 6: Lessons Learned

**Post-Incident Review:**
- Identify gaps in detection
- Improve OSINT monitoring rules
- Update phishing awareness training
- Refine SOC procedures

---

## Metrics & KPIs
- Mean Time to Detect (MTTD)
- Mean Time to Respond (MTTR)
- Number of phishing attempts blocked
- Number of domains taken down
- User reporting rate

---

## SOC Maturity Alignment
This playbook supports:
- Tier 1 SOC triage
- Tier 2 investigation
- Threat Intelligence integration
- Continuous improvement cycles

---

## Summary
By integrating OSINT into SOC workflows, organizations can:
- Detect threats earlier
- Reduce phishing success rates
- Protect brand trust
- Strengthen overall cyber resilience
