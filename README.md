# ShadowEncrypt-Windows-PoC

## ⚠ WARNING

`locker.exe` is a ransomware behavior proof-of-concept executable.

Running this executable will attempt to encrypt/lock files in the current working directory.

DO NOT execute this binary on:
- Personal systems
- Production machines
- Important data directories
- Shared environments

Run ONLY inside:
- Isolated virtual machines
- Malware analysis sandboxes
- Disposable lab environments
- Controlled cybersecurity research setups

The author is not responsible for data loss or misuse.

---

# Overview

ShadowEncrypt-Windows-PoC is a Windows ransomware behavior simulation developed as a cybersecurity research project.

The project demonstrates:
- Hybrid cryptographic ransomware workflow
- File encryption operations
- Symmetric/asymmetric key handling
- Ransomware execution flow
- Malware analysis concepts
- Defensive security research techniques

This repository is intended strictly for:
- Academic research
- Malware analysis training
- Threat simulation
- Incident response practice
- Defensive cybersecurity education

---

# Technical Architecture

The project implements a hybrid encryption model:

1. A random Fernet symmetric key is generated
2. Files are encrypted using Fernet encryption
3. The Fernet key is encrypted using RSA-OAEP with SHA256
4. The encrypted key artifact is stored on disk

Cryptographic stack:
- Fernet (AES-based authenticated encryption)
- RSA public/private key cryptography
- OAEP padding with SHA256

---

# Included File

```bash
locker.exe
```

This executable is the packaged ransomware behavior simulation binary built using PyInstaller.

---

# Behavioral Characteristics

The executable:
- Enumerates files in the working directory
- Encrypts eligible files in-place
- Skips operational files to avoid self-breakage
- Uses RSA-wrapped symmetric encryption keys
- Demonstrates ransomware-style encryption flow

Scope:
- Current directory only
- Non-recursive traversal

---

# Safe Testing Procedure

Recommended environment:
- Windows virtual machine
- Snapshot enabled
- No personal files
- Isolated network
- Disposable test data

Suggested workflow:
1. Create VM snapshot
2. Add dummy test files
3. Execute locker.exe
4. Observe encryption behavior
5. Restore VM snapshot

---

# Educational Objectives

This project was created to study:
- Ransomware execution techniques
- File encryption behavior
- Malware operational flow
- Cryptographic abuse in malware
- Detection and mitigation opportunities
- Incident response scenarios

---

# Research Disclaimer

This repository was developed solely as a cybersecurity research and educational project.

It is NOT intended for:
- Unauthorized access
- Extortion
- Real-world attacks
- Malicious deployment
- Criminal activity

Any misuse of this project is strictly prohibited.

---

# Technologies Used

- Python 3.11
- PyInstaller
- cryptography library
- RSA-OAEP
- Fernet encryption

---

# Author
Pratyush Mohanty
Cybersecurity Research Project  
Windows Malware Behavior PoC  
