# Wi-Fi Security Experiment: WPA2 vs WPA3

## Overview
This repository documents a controlled educational lab experiment comparing the security behavior of WPA2-PSK and WPA3-SAE wireless networks.  
The focus is on observing how offline dictionary attacks work against WPA2 and why the same approach fails against WPA3.

All testing was performed in a private, permitted lab environment.

---

## Objective
- Analyze the effectiveness of offline dictionary attacks against WPA2-PSK.
- Observe WPA3-SAE behavior when similar attack techniques are attempted.
- Evaluate the practical limitations of tools like Wifite in modern Wi-Fi security.

---

## Lab Environment
- Operating System: Kali Linux
- Wireless Adapter: Built-in adapter (monitor mode supported)
- Tooling:
  - Wifite
  - Aircrack-ng (via Wifite)
- Test Networks:
  - WPA2-PSK (numeric-only password)
  - WPA3-SAE (comparable password policy)

---

## Experiment Methodology

### WPA2 Testing
- Captured a valid WPA2 four-way handshake using Wifite.
- Performed an offline dictionary attack using a numeric-only wordlist.
- Successfully recovered the password due to weak password complexity.

### WPA3 Testing
- Attempted the same approach against a WPA3-SAE network.
- Wifite failed to proceed with offline cracking.
- No reusable handshake was available for dictionary attacks.

---

## Results and Observations
- WPA2 is vulnerable to offline dictionary attacks when weak passwords are used.
- WPA3’s SAE authentication prevents traditional offline cracking.
- Password complexity plays a critical role in WPA2 security.
- Wifite is effective for learning WPA2 weaknesses but ineffective against WPA3 by design.

---

## Key Takeaways
- Numeric-only or simple passwords significantly weaken WPA2 security.
- WPA3 adoption provides meaningful protection against offline attacks.
- Strong passphrases (length, symbols, mixed case) remain essential.
- Ethical testing must always be limited to authorized environments.
- Wordlist quality directly affects cracking success in WPA2 scenarios.

---

## Disclaimer
This project was conducted strictly for educational purposes within a controlled lab environment.  
No unauthorized networks were targeted or accessed.

---

## References
- IEEE 802.11 WPA3 Specification
- Aircrack-ng Documentation
- Wifite Project
