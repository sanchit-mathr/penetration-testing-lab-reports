#Dev (Boltwire) – Penetration Testing Report

## Machine Overview
- **Machine Name:** Dev (Boltwire)
- **Environment:** Local Lab (Intentionally Vulnerable)
- **Assessment Type:** Penetration Testing
- **Initial Access:** Unauthenticated External Attacker
- **Final Goal:** Root Access
- **Author:** Sanchit Mathur

---

## Objective
The objective of this assessment was to identify exposed services, enumerate vulnerabilities, gain initial access, escalate privileges, and achieve full system compromise while following a structured penetration testing methodology.

---

## Attack Chain Overview
The machine was compromised by chaining together multiple low-severity misconfigurations and vulnerabilities:
Nmap Enumeration
→ FFUF Directory Discovery
→ NFS Enumeration
→ save.zip Disclosure
→ Credential & SSH Key Extraction
→ Boltwire CMS Enumeration
→ Local File Inclusion (LFI)
→ SSH Access
→ Sudo Misconfiguration
→ GTFOBins (zip) Exploitation
→ Root Access
This demonstrates how improper system hardening can lead to complete compromise without the use of advanced exploits.

---

## Key Vulnerabilities Identified

| Vulnerability | Impact |
|---------------|--------|
| Exposed NFS Share | Sensitive file disclosure |
| Weak ZIP File Protection | Credential and key leakage |
| Local File Inclusion (LFI) in Boltwire CMS | User enumeration |
| Credential Reuse | Unauthorized SSH access |
| Misconfigured sudo permissions (zip) | Full root compromise |

---

## Skills Demonstrated
- Network and service enumeration (Nmap)
- Web directory and content discovery (FFUF)
- NFS enumeration and exploitation
- Password cracking (ZIP file)
- SSH private key analysis
- Web application testing (LFI)
- Linux privilege escalation techniques
- GTFOBins exploitation
- Professional penetration testing documentation

---

## Tools Used
- Nmap
- FFUF
- showmount / mount (NFS)
- John the Ripper
- SSH
- GTFOBins
- Linux command-line utilities

---

## Evidence & Screenshots
All supporting screenshots and proof-of-exploitation evidence are available in the `screenshots/` directory and are referenced within the full penetration testing report.

---

## Full Report
A detailed, step-by-step penetration testing report is available here:

📄 **Dev_Penetration_Testing_Report.pdf**

The report includes:
- Executive summary
- Scope and methodology
- Commands used
- Findings and evidence
- Privilege escalation steps
- Recommendations

---

## Recommendations (High-Level)
- Restrict NFS exports and enforce authentication
- Avoid storing sensitive credentials in shared locations
- Sanitize user input to prevent file inclusion vulnerabilities
- Audit sudo permissions regularly
- Monitor binaries for GTFOBins abuse
- Apply defense-in-depth hardening practices

---

## Disclaimer
This project was conducted in a controlled lab environment on an intentionally vulnerable machine for educational and learning purposes only.  
No unauthorized testing was performed against real-world systems.

---

## Notes
This machine is part of a larger collection of documented penetration testing case studies aimed at demonstrating hands-on offensive security skills and structured reporting.
