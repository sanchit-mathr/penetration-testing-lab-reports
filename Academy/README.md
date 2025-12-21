# Academy Machine – Penetration Testing Report

## Overview

This directory contains a detailed penetration testing assessment of the **Academy** machine, an intentionally vulnerable Linux-based lab environment inspired by Hack The Box / CTF-style challenges.

The objective of this assessment was to identify security weaknesses, gain initial access, perform post-exploitation enumeration, and evaluate potential privilege escalation paths using standard penetration testing methodology.

---

## Assessment Details

- **Target Name:** Academy
- **Operating System:** Linux
- **Assessment Type:** Internal Penetration Test
- **Difficulty Level:** Easy to Medium
- **Tester:** Sanchit Mathur

---

## Attack Summary

The following attack path was identified during testing:

- Network and service enumeration using **Nmap**
- Anonymous FTP access leading to sensitive information disclosure
- Web directory enumeration using **DirBuster** and **FFUF**
- Insecure file upload vulnerability resulting in **remote code execution**
- Reverse shell access obtained on the target system
- Post-exploitation enumeration using **LinPEAS** and **pspy** to identify privilege escalation vectors

While full root access was not achieved during testing, multiple misconfigurations were identified that indicate insufficient privilege hardening.

---

## Contents

- report.pdf**  
  Full penetration testing report detailing methodology, findings, exploitation steps, and remediation recommendations.

- **screenshots/**  
  Supporting evidence of enumeration, exploitation, and post-exploitation activities.

---

## Tools Used

- Nmap
- FTP
- DirBuster
- FFUF
- Bash Reverse Shell
- LinPEAS
- pspy

---

## Notes

- This assessment was performed **only on a controlled, intentionally vulnerable lab environment**.
- The report is intended strictly for **educational and ethical learning purposes**.

---

## Author

**Sanchit Mathur**  
Cyber Security | CEH | SOC & Pentesting  
Email: mathursanchit7@gmail.com
