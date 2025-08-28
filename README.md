# Wi-Fi Security Experiment: WPA2 vs WPA3

> **Educational lab experiment** comparing WPA2 and WPA3 Wi-Fi security using Wifite.

---

##  Objective
Conduct a controlled lab experiment to explore how **WPA2-PSK** and **WPA3-SAE** react to offline dictionary attacks, and to observe the behavior of tools like **Wifite** in each scenario. All testing was performed in a private, permitted environment.

---

##  Tools & Lab Setup
- **OS:** Kali Linux with built-in wireless adapter  
- **Tool:** Wifite (leveraging Aircrack-ng for cracking)  
- **Test Networks:**
  - WPA2-PSK secured network (numeric-only password)
  - WPA3-SAE secured network (similar password setup)

---

##  Experiment Steps
1. **WPA2 Testing**
   - Captured the WPA2 handshake with Wifite.
   - Used a numeric-only wordlist for password cracking.
   - Successfully cracked the WPA2 password when it was purely numeric.

2. **WPA3 Testing**
   - Attempted the same process against WPA3.
   - Wifite failed, as WPA3 uses **SAE**, which resists offline cracking.

---

##  Results & Insights
- **WPA2 vulnerability**: Offline dictionary attacks effective when passwords are weak (e.g., numeric only).
- **WPA3 strength**: SAE-based authentication resists this type of attack.
- **Wordlist significance**: Cracking success depends on complexity and coverage.
- Wifite is **useful for learning WPA2 weaknesses**, but not effective against WPA3.

---

##  Key Learnings
- Use **strong, complex passwords** (mix of letters, numbers, symbols).
- WPA3 adoption significantly improves Wi-Fi security.
- Ethical hacking experiments must be confined to controlled environments.
- Tools like `crunch` can help generate comprehensive wordlists for realistic testing.

---

##  Disclaimer
This experiment was conducted strictly for **educational and ethical purposes** in a controlled lab setup. It does **not** endorse or promote unauthorized access to any networks.

---


