# The Inside Job – Hardware-Assisted Malware Deployment Framework for Red Team Operations

## Overview
**The Inside Job** is a hardware-assisted red-team simulation framework designed for academic and research use.  
The system demonstrates how covert hardware devices (such as USB-based HID implants) can be combined with custom malware, a secure C2 infrastructure, and layered stealth techniques to simulate modern APT-style attack chains.

This repository contains:
- System architecture & context diagrams  
- Layer-by-layer workflow documentation  
- Hardware access design  
- Malware execution model  
- C2 communication flow  
- Assumptions, constraints, and design rationale  
- Presentation material for FYP Phase I & II  

---

## System Architecture (High-Level)
The system is built across **four interconnected layers**:

1. **Hardware Access Layer**  
   - Covert USB device injects payload via HID emulation  
   - Requires brief physical access  
   - Triggers the loader on the target machine  

2. **Malware Execution Layer**  
   - Loader activates the Host-Side Agent  
   - Core malware performs collection, persistence, evasion, and command execution  
   - Supports modular extensions  

3. **C2 Infrastructure Layer**  
   - Encrypted communication with Team Server (DNS/HTTPS/custom)  
   - Operator console issues commands & receives telemetry  
   - Supports multi-host session management  

4. **Host Interaction Layer**  
   - Malware interacts with OS APIs  
   - Executes operator instructions  
   - Continuous beaconing and reporting  

---

## Features
- Hardware-triggered malware deployment  
- Modular malware architecture  
- Secure C2 communication  
- Stealth, obfuscation, and anti-analysis mechanisms  
- Realistic red-team simulation flow  
- Architecture diagrams and documentation included  

---

## Purpose & Ethical Use
This project is built **strictly for controlled research, academic demonstrations, and defensive training**.  
It must **not** be used for unauthorized or malicious activities.

---

## Team Members
- **Huzaifa**  
- **Hassaan**  
- **Abdullah**  
- **Saad**

---

## Advisor
- **Dr. Salman Ahmad**

Co-Advisors:
- **Ms. Beenish Urooj**  
- **Dr. Qadeer Ul Hassan**

---


## Disclaimer
This research framework is provided for **educational and defensive cybersecurity purposes only**.  
Unauthorized or unethical use is strictly prohibited.
