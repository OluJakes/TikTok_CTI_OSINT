# TikTok OSINT-Based Cyber Threat Intelligence (CTI) Assessment

## 🔎 Executive Overview
This repository presents a **defensive, OSINT-driven Cyber Threat Intelligence (CTI) assessment** conducted against **TikTok (tiktok.com)** and its parent organization **ByteDance**.

The project mirrors **real-world SOC and Threat Intelligence workflows**, demonstrating how adversaries conduct reconnaissance using publicly available data — and how defenders can identify, contextualize, and mitigate those risks **without exploitation or unauthorized access**.

This assessment focuses on **phishing risk, brand impersonation exposure, identity intelligence, and external attack surface awareness**, mapped directly to the **MITRE ATT&CK Reconnaissance tactic**.

---

## 🎯 Intelligence Objectives
This assessment was designed to answer practical CTI questions relevant to SOC and Blue Team operations:

- What **publicly accessible information** could attackers leverage during reconnaissance?
- Does TikTok face **phishing, impersonation, or social-engineering risk**?
- What **identity and infrastructure signals** are externally visible via OSINT?
- How do observed findings align with **known adversary techniques (MITRE ATT&CK)**?
- What **defensive actions** meaningfully reduce real-world risk?

---

## 🧭 Scope & Ethical Boundaries
- **Passive OSINT only** (no scanning, probing, or exploitation)
- Publicly available sources only
- No interaction with TikTok systems or users
- Conducted strictly for **educational and defensive intelligence purposes**

This mirrors how **threat intelligence teams operate legally and ethically** in enterprise environments.

---

## 🛠 Tools & Frameworks Utilized

| Intelligence Domain | Tools / Frameworks |
|-------------------|-------------------|
| Search & Discovery | Google Dorks |
| Identity & Email Intelligence | theHarvester, Hunter.io |
| Infrastructure Intelligence | Shodan |
| Reputation & Indicator Validation | VirusTotal |
| Historical Exposure Analysis | Wayback Machine |
| OSINT Methodology | OSINT Framework |
| Adversary Modeling | MITRE ATT&CK |

---

## 🔍 Key Intelligence Findings (High-Level)
- Publicly indexed login and business portals increase **phishing and impersonation risk**
- Large-scale discoverable email addresses enable **targeted social engineering**
- Extensive subdomain footprint expands **reconnaissance surface**
- CDN and edge-network protections reduce direct infrastructure exposure
- Clean domain reputation indicates **strong baseline security hygiene**
- No evidence of credential leaks identified in this passive assessment

---

## 🧠 Threat Actor Perspective
From an attacker’s viewpoint, this OSINT footprint enables:

- **Spear-phishing campaigns** using real employee email patterns
- **Brand impersonation** through cloned portals and look-alike domains
- **Pre-attack profiling** using historical content and organizational terminology
- **Infrastructure mapping** to understand hosting, CDN, and DNS relationships

These activities align with **pre-intrusion reconnaissance** commonly observed before phishing, credential theft, and fraud campaigns.

---

## 🛡 Defender Takeaways
From a defensive and SOC standpoint, this assessment highlights:

- OSINT exposure is a **leading indicator of phishing risk**
- Email pattern predictability increases attack success probability
- CDN and edge protections significantly reduce exploitability but **do not eliminate social-engineering risk**
- Continuous OSINT monitoring should be treated as a **preventive security control**, not a reactive task

---

## 🧩 MITRE ATT&CK Coverage Summary
All findings were mapped to standardized adversary techniques under the **Reconnaissance tactic (TA0043)**, including:

- **T1593** – Search Open Websites/Domains  
- **T1589** – Gather Victim Identity Information  
- **T1590** – Gather Victim Network Information  

📌 Detailed mappings are available in:  
`mitre/mitre_attack_mapping.md`

---

## 🏢 How This Maps to Real-World SOC Operations
This project directly reflects activities performed by:

- **SOC Analysts** – contextualizing alerts tied to phishing and impersonation
- **Threat Intelligence Analysts** – tracking adversary reconnaissance behavior
- **Blue Teams** – reducing external attack surface before exploitation
- **Security Leadership** – understanding brand and identity risk exposure

The workflow mirrors:
1. Intelligence requirements definition  
2. OSINT collection  
3. Analytical correlation  
4. ATT&CK mapping  
5. Defensive recommendations  

---

## 🧪 SOC / CTI Skills Demonstrated
- Cyber Threat Intelligence (CTI) analysis  
- OSINT collection & validation  
- Phishing & brand impersonation risk assessment  
- Infrastructure reconnaissance interpretation  
- MITRE ATT&CK technique mapping  
- Evidence-driven reporting  
- Ethical security research  

---

## 📂 Repository Structure

| Path | Description |
|----|------------|
| `/report` | Full CTI assessment (PDF) |
| `/evidence` | OSINT screenshots and artifacts |
| `/mitre` | MITRE ATT&CK mapping |
| `/metadata` | Scope, ethics, and methodology |

---

## 👤 Author
**Olumide Solanke**  
Cybersecurity • Threat Intelligence • SOC / Blue Team  

Certifications: CySA+ • CISM • PMP • AWS-SAA
📍 Open to **remote SOC, CTI, and Blue Team roles** (Canada / Ontario)

---

## ⚠ Disclaimer
This repository contains **defensive cyber threat intelligence only**.  
All data was derived from publicly available sources.  
No exploitation, scanning, or unauthorized access was performed.
