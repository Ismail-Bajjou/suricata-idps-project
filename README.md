# suricata-idps-project
## Overview

This project deploys **Suricata** as an **IDPS** to detect and block attacks generated from an attacker machine (Kali) against a vulnerable target (Metasploitable).  
The goal is to understand how Suricata works, including:
- IDS and IPS modes  
- Suricata architecture  
- Configuration files  
- ET (Emerging Threats) rules  
- Custom rule creation  
- Alert and drop analysis  

This environment provides a clear introduction to intrusion detection and prevention.

## Architecture

This lab uses a simple 3‑machine network:
- **Ubuntu (Suricata IDPS):** monitors traffic, detects attacks, and blocks malicious packets.  
- **Kali (Attacker):** generates scans, exploits, DoS, and brute‑force traffic.  
- **Metasploitable (Victim):** vulnerable machine used to trigger Suricata alerts.
![](images/architecture.png)


Suricata can operate in two modes:
- **IDS mode (passive):** Suricata only listens and generates alerts.  
- **IPS mode (inline):** Suricata analyzes packets and drops malicious ones in real time.

This architecture allows testing detection first, then prevention.

