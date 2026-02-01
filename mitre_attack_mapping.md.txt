# MITRE ATT&CK Mapping – OSINT Reconnaissance Assessment

## Overview
This document maps findings from the OSINT-based Cyber Threat Intelligence (CTI) assessment
of TikTok and ByteDance to relevant **MITRE ATT&CK Reconnaissance techniques**.

The mapping demonstrates how publicly available information can be leveraged by adversaries
during early-stage attack planning, while also enabling defenders to align detection,
prevention, and monitoring strategies with a standardized framework.

---

## Reconnaissance Tactic (TA0043)

The **Reconnaissance** tactic describes adversary techniques used to gather information
about a target organization in preparation for future operations such as phishing,
impersonation, or infrastructure abuse.

---

## MITRE ATT&CK Technique Mapping

| Tool Used | OSINT Finding | ATT&CK Technique | Sub-Technique | Description | Defensive Considerations |
|--------|--------------|----------------|--------------|-------------|--------------------------|
| Google Dorks | Publicly indexed login and API-related URLs | T1593 | T1593.002 – Search Open Websites/Domains | Adversaries search public websites to identify authentication portals and exposed resources | Reduce indexed sensitive endpoints; monitor for cloned login pages |
| Google Dorks | Public PDF and document discovery | T1593 | T1593.003 – Search Open Websites/Domains | Public documents may reveal organizational structure or terminology | Review document publication processes; remove unnecessary metadata |
| theHarvester | Large volume of subdomains identified | T1590 | T1590.005 – Gather Victim Network Information | Subdomain enumeration enables infrastructure mapping | Maintain strict subdomain governance and asset inventory |
| theHarvester | Discovery of hosting and IP associations | T1590 | T1590.001 – Gather Victim Network Information | Passive identification of hosting providers and network ranges | Use CDN/edge protections and limit direct origin exposure |
| Hunter.io | Identification of employee email patterns | T1589 | T1589.002 – Gather Victim Identity Information | Email patterns enable targeted phishing and impersonation | Enforce DMARC, SPF, DKIM and employee phishing training |
| Hunter.io | Enumeration of high-confidence employee emails | T1589 | T1589.001 – Gather Victim Identity Information | Real identities used to craft convincing spear-phishing lures | Minimize public exposure of staff email addresses |
| Shodan | Identification of internet-facing services | T1590 | T1590.005 – Gather Victim Network Information | Adversaries validate exposed services and ports | Continuously monitor exposed assets; harden edge services |
| VirusTotal | DNS and domain relationship visibility | T1590 | T1590.001 – Gather Victim Network Information | Mapping domain relationships and infrastructure dependencies | Monitor reputation changes and domain associations |
| Wayback Machine | Historical web content analysis | T1593 | T1593.003 – Search Open Websites/Domains | Legacy content may expose deprecated services or workflows | Regularly review archived content; request removal if necessary |
| OSINT Framework | Structured tool selection for recon | T1593 | Multiple | Framework-guided reconnaissance increases efficiency and coverage | Apply framework-based monitoring defensively |

---

## Threat Progression Context

When combined, the mapped techniques demonstrate a realistic attacker progression:

1. **Initial Discovery** – Search engines and archives reveal public portals and documents  
2. **Identity Mapping** – Email patterns and staff identities are enumerated  
3. **Infrastructure Mapping** – Subdomains, services, and hosting providers are identified  
4. **Preparation for Exploitation** – Intelligence supports phishing, impersonation, or abuse campaigns  

This progression reflects common pre-attack behavior observed in phishing, BEC, and brand
impersonation campaigns.

---

## Defensive Value of MITRE Mapping

Mapping OSINT findings to MITRE ATT&CK provides:

- A shared language between security, risk, and leadership teams
- Alignment between intelligence findings and detection strategies
- Improved prioritization of defensive controls
- Clear justification for security investments

---

## Conclusion

This MITRE ATT&CK mapping highlights how **passive OSINT activities align directly with
recognized adversary reconnaissance techniques**. Understanding this relationship enables
organizations to shift from reactive defense toward proactive threat intelligence–driven
security monitoring.

