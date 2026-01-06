# Digital-Forensics-Incident-Response
# 🔍 Digital Forensics & Incident Response (DFIR) Portfolio

## 📋 Project Description
This repository documents two distinct forensic investigations conducted in a simulated lab environment. The goal was to apply the Incident Response Lifecycle and digital evidence handling best practices.

## 📂 Case Study 1: Ransomware Investigation (LockBit 3.0)
**Scenario:** A critical server infrastructure was compromised by crypto-ransomware.
* **Methodology:** NIST SP 800-61 (Incident Response Lifecycle).
* **Actions Taken:**
    * **Containment:** Network isolation and preservation of volatile memory (RAM).
    * **Analysis:** Identified entry vector via RDP logs and compromised credentials.
    * **Recovery:** Restoration from offline immutable backups.

## 📂 Case Study 2: Mobile Forensics (Android)
**Scenario:** Forensic analysis of a seized Android device linked to corporate espionage.
* **Methodology:** Logical and Physical extraction analysis.
* **Tools Used:** ADB (Android Debug Bridge), SQLite Browser, Autopsy.
* **Key Findings:**
    * Recovered deleted SMS from `mmssms.db`.
    * Reconstructed timeline of events using `contacts2.db` and call logs.
    * Verified geolocation data confirming suspect's presence at the crime scene.

## ⚖️ Chain of Custody & Standards
All evidence was handled according to **RFC 3227** (Order of Volatility):
1. CPU Cache / RAM
2. Swap / Page File
3. Hard Drive Data
4. Archival Media

## 📸 Investigation Screenshots
![Forensic Analysis](link_to_screenshot.png)
*Figure 1: SQL Analysis of the messaging database.*
