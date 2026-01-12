# BlackPearl – Web Application Penetration Test

## Overview
This repository documents a complete penetration testing assessment of the **BlackPearl** vulnerable lab machine.  
The project focuses on applying **real-world web application penetration testing methodology**, emphasizing enumeration, virtual host discovery, and remote code execution rather than step-by-step exploitation walkthroughs.

The engagement simulates a **black-box internal network penetration test**, similar to scenarios encountered by SOC analysts and junior penetration testers.

---

## Disclaimer
This project was conducted in a **controlled lab environment** intentionally designed to be vulnerable.  
All testing activities were performed strictly for **educational and ethical purposes**.  
No real-world systems were targeted.

---

## Objectives
- Apply structured penetration testing methodology (PTES-inspired)
- Perform network and web application enumeration
- Identify hidden attack surfaces through virtual host discovery
- Exploit a vulnerable CMS leading to remote code execution
- Produce professional-grade penetration testing documentation

---

## Lab Environment

| Component | Details |
|---------|--------|
| Target Name | BlackPearl |
| Target IP | 192.168.1.14 |
| Virtual Host | blackpearl.tcm |
| Operating System | Linux |
| Assessment Type | Black-box |
| Tools Used | Nmap, FFUF, DNSRecon, cURL, Metasploit |

---

## Methodology
The penetration test followed a structured workflow aligned with industry practices:

1. Reconnaissance  
2. Enumeration  
3. Vulnerability Identification  
4. Exploitation  
5. Post-Exploitation  
6. Impact Analysis  
7. Mitigation Recommendations  

This approach mirrors real-world penetration testing and SOC investigation processes rather than CTF-style problem solving.

---

## Key Findings

### Critical Vulnerability – Navigate CMS Remote Code Execution
An outdated instance of **Navigate CMS** was identified behind a virtual host configuration.  
Improper input handling allowed **unauthenticated remote code execution**, resulting in full system compromise.

**Severity:** Critical  
**Attack Complexity:** Low  
**Impact:** Complete compromise of the target system

---

## Exploitation Summary
- Web enumeration revealed a restricted CMS endpoint
- Virtual host discovery exposed additional application functionality
- Host header manipulation enabled access to the vulnerable CMS
- A known Navigate CMS vulnerability was exploited to achieve remote code execution
- Remote shell access was successfully obtained

Exploitation was performed only to validate impact and not for persistence or system damage.

---

## Impact Assessment
Successful exploitation could allow an attacker to:
- Execute arbitrary commands on the server
- Access or exfiltrate sensitive data
- Modify or deface web content
- Pivot to other systems within the internal network

---

## Recommendations

### Immediate Actions
- Upgrade Navigate CMS to the latest patched version
- Restrict access to CMS administrative endpoints
- Remove unnecessary CMS components

### Defensive Hardening
- Implement a Web Application Firewall (WAF)
- Enforce proper virtual host isolation
- Monitor HTTP logs for abnormal Host header activity

### Long-Term Improvements
- Perform regular vulnerability assessments
- Review CMS security configurations
- Maintain consistent patch management practices

---

## Repository Structure
BlackPearl/
├── README.md
├── report
---

## Skills Demonstrated
- Web application enumeration
- Virtual host and Host header testing
- CMS vulnerability exploitation
- Metasploit Framework usage
- Professional penetration testing documentation
- Security impact assessment and remediation planning

---

## Author
Sanchit Mathur  
Cybersecurity Graduate | SOC Analyst | Penetration Testing  

---

## Notes
This repository is intended to demonstrate **hands-on security testing skills** and **structured analytical thinking**, not automated exploitation or tool dependency.

