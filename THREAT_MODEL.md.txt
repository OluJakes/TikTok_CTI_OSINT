# Threat Model – TikTok OSINT-Based Assessment

## Purpose
This document models **realistic attacker behavior** based on findings from a passive OSINT reconnaissance assessment of TikTok and ByteDance.

It demonstrates how adversaries could transform publicly available intelligence into actionable attack paths, aligned with the **Cyber Kill Chain** and **MITRE ATT&CK** frameworks.

---

## Threat Modeling Approach
The analysis follows a **defender-centric threat modeling methodology**:

1. Identify exposed intelligence signals (OSINT)
2. Map attacker goals and capabilities
3. Construct likely attack paths
4. Align activities to MITRE ATT&CK
5. Assess defensive gaps and opportunities

---

## Threat Actor Profiles

### 1. Financially Motivated Cybercriminal
**Motivation:** Fraud, credential theft, account takeover  
**Capabilities:** OSINT, phishing kits, commodity malware  
**Target:** Employees, customers, advertisers  

### 2. Brand Impersonation Actor
**Motivation:** Scams, misinformation, trust abuse  
**Capabilities:** Look-alike domains, cloned login pages  
**Target:** End users and content creators  

### 3. Advanced Persistent Threat (Recon Phase)
**Motivation:** Long-term access, strategic intelligence  
**Capabilities:** Multi-stage reconnaissance, infrastructure mapping  
**Target:** Corporate infrastructure and personnel  

---

## Attack Paths (Kill Chain Mapping)

### Attack Path 1: Spear Phishing via Email Enumeration

**Kill Chain Phase:** Reconnaissance → Weaponization → Delivery  

**Attack Flow:**
1. Attacker enumerates employee emails using Hunter.io and theHarvester
2. Identifies predictable naming patterns
3. Collects internal terminology via Google Dorks and archived content
4. Crafts targeted phishing emails impersonating internal IT or HR
5. Delivers payload or credential harvesting page

**MITRE ATT&CK Techniques:**
- T1589.002 – Gather Victim Identity Information (Email Addresses)
- T1593.002 – Search Open Websites/Domains
- T1566.001 – Phishing: Spearphishing Attachment

**Impact:**
- Credential compromise
- Business Email Compromise (BEC)
- Lateral movement opportunity

---

### Attack Path 2: Brand Impersonation & Fake Login Pages

**Kill Chain Phase:** Reconnaissance → Delivery → Exploitation  

**Attack Flow:**
1. Attacker identifies legitimate TikTok login portals
2. Clones page branding and structure
3. Deploys fake login pages on look-alike domains
4. Distributes links via social media or email

**MITRE ATT&CK Techniques:**
- T1593 – Search Open Websites/Domains
- T1583.001 – Acquire Infrastructure: Domains
- T1566.002 – Phishing: Link

**Impact:**
- User credential harvesting
- Reputational damage
- Customer trust erosion

---

### Attack Path 3: Infrastructure Reconnaissance

**Kill Chain Phase:** Reconnaissance  

**Attack Flow:**
1. Attacker queries Shodan and VirusTotal
2. Maps exposed services and hosting providers
3. Identifies cloud/CDN usage and DNS relationships
4. Establishes baseline for future exploitation attempts

**MITRE ATT&CK Techniques:**
- T1590.005 – Gather Victim Network Information: IP Addresses
- T1596.001 – Search Open Technical Databases

**Impact:**
- Informed targeting
- Improved attack precision
- Reduced attacker noise

---

## Defensive Insights
- Email exposure is the **highest-risk attack surface**
- Brand trust is a critical asset for adversaries
- Reconnaissance alone enables impactful attacks
- OSINT monitoring is a defensive necessity, not optional

---

## Summary
This threat model demonstrates that **no exploitation is required** for adversaries to build credible attack campaigns.  
Proactive monitoring, identity protection, and phishing resistance are critical to risk reduction.
