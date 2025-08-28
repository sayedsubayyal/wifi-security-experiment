🔐 Wi-Fi Security Experiment: WPA2 vs WPA3
📌 Objective

The purpose of this experiment was to understand the differences between WPA2 and WPA3 Wi-Fi security and to learn how penetration testing tools like Wifite work in a controlled lab environment.

This experiment was done only in my own test lab setup, not on any third-party or unauthorized network.

🛠️ Tools & Environment

Operating System: Kali Linux (built-in wireless adapter)

Tool Used: Wifite (uses Aircrack-ng for cracking)

Test Networks:

A lab Wi-Fi with WPA2-PSK and numeric password

A lab Wi-Fi with WPA3-SAE and similar password

⚙️ Experiment Steps

WPA2 Testing

Captured the WPA2 handshake using Wifite.

Used a numeric-only wordlist for password cracking.

Successfully retrieved the WPA2 password when it was purely numeric.

WPA3 Testing

Attempted the same process against WPA3.

Wifite failed to crack the password, since WPA3 uses SAE (Simultaneous Authentication of Equals) which prevents traditional handshake cracking.

📊 Results & Observations

WPA2 is vulnerable to offline dictionary attacks if weak/numeric passwords are used.

WPA3 is significantly stronger, since the SAE handshake is resistant to offline cracking.

The effectiveness of cracking depends heavily on the wordlist quality.

Tools like Wifite are educational for WPA2, but not effective against WPA3.

📚 Key Learnings

Always use complex passwords (letters + numbers + symbols) for Wi-Fi.

WPA3 adoption is crucial for stronger security.

Ethical hacking experiments should always be done in a controlled lab environment.

Building custom wordlists with tools like crunch helps simulate real-world scenarios.

✅ Disclaimer

This project was conducted strictly for educational and ethical purposes in a controlled lab environment.
I do not encourage or support unauthorized access to any network.
