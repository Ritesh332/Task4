# 🔐 Task 4 – Firewall Setup and Configuration

## 🎯 Objective
To configure and test basic firewall rules on a Linux system using UFW (Uncomplicated Firewall). The goal was to block and allow specific ports (e.g., Telnet on port 23, SSH on port 22), test them, and understand how firewall rules affect network traffic.

---

## 🛠️ Tools & System Used
- **Operating System:** Ubuntu 22.04 (Linux)
- **Firewall Tool:** UFW (Uncomplicated Firewall)
- **Terminal**
- **Telnet & SSH (for testing)**
- **Netcat (optional for local testing)**

---

## ✅ What I Did During This Task

1. **Checked UFW Status**
   - Verified whether UFW was active and checked default policies.

2. **Enabled UFW**
   - If disabled, I enabled UFW to start configuring it.

3. **Listed Existing Rules**
   - Viewed current active firewall rules.

4. **Blocked Port 23 (Telnet)**
   - Added a rule to deny inbound traffic on TCP port 23 using: `sudo ufw deny 23`

5. **Tested Telnet Block**
   - Attempted to connect to localhost on port 23.
   - Received a “Connection refused” error — this showed no Telnet service was running.

6. **Simulated Port 23 (Telnet) Using Netcat**
   - Used netcat to simulate a listener.
   - Connected successfully with localhost when UFW allowed port 23.
   - Verified the port was blocked when UFW denied it.

7. **Allowed Port 22 (SSH)**
   - Ensured SSH was accessible.

8. **Verified Rule Application**
   - Telnet connection tested.
   - SSH connection tested.

10. **Removed Telnet Block Rule**
   - Cleaned up the test rule.

11. **Took Screenshots**
    - Captured each major step: enabling UFW, blocking and allowing ports, testing with Telnet and SSH, removing rules.

---

## ⚠️ Disclaimer

This project is intended strictly for educational purposes. The configurations, commands, and testing methods used (e.g., Telnet on port 23) are demonstrated in a controlled, local environment.

Do not expose insecure services like Telnet on real or public-facing systems, as they are highly vulnerable to attacks. Always follow best practices for system and network security in production environments.

---
