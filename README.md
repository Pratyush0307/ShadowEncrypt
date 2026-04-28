# ShadowEncrypt-Windows-PoC

## ⚠ WARNING
**Executing `locker.exe` will encrypt/lock files on the host system.**

Run this executable **ONLY** inside:
- Isolated virtual machines
- Malware analysis sandboxes
- Controlled lab environments
- Disposable test systems

**Do NOT run this on your personal machine or production systems.**

---

## Overview
ShadowEncrypt-Windows-PoC is a Windows ransomware proof-of-concept developed as a **cybersecurity research project** to study ransomware behavior, encryption workflows, and defensive detection techniques.

This project demonstrates:
- File encryption behavior
- Ransomware execution flow
- Key handling mechanisms
- Malware analysis concepts
- Defensive security research use cases

## Included File
```bash
locker.exe
```

This executable simulates ransomware-style encryption and is provided strictly for educational malware research.

---

## Research Purpose
Developed for:
- Malware behavior analysis
- Incident response practice
- Threat simulation
- Defensive security testing
- Cybersecurity academic research

---

## Usage Warning
```bash
./locker.exe
```

⚠ Running the executable may lock/encrypt files in the execution environment.

Use only on dummy files or inside a VM snapshot you can restore.

---

## Safe Testing Recommendation
Recommended environment:
- Windows Virtual Machine
- Snapshot enabled
- Isolated test folder
- No personal files present

Example workflow:
1. Create VM snapshot
2. Place dummy test files
3. Execute locker.exe
4. Analyze behavior
5. Restore snapshot

---

## Disclaimer
This repository was developed **solely as a cybersecurity researcher project** for academic and defensive purposes.

It is NOT intended for:
- Unauthorized access
- Real-world deployment
- Malicious activity
- Extortion or destructive use

The author assumes no liability for misuse or damage caused by running this software.

---

## Educational Note
This repository is published to support understanding of ransomware mechanics so defenders can better detect and mitigate such threats.

---

## Author
Pratyush Mohanty <br>
Cybersecurity Research Project  <br>
Malware Analysis / Defensive Security PoC <br>
