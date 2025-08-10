# Task 4 – Configuring and Testing Firewall Rules

## 🎯 Objective:
Configure a custom firewall rule on Windows 11 and test it to confirm the configuration works.

---

## 🛠 Tools Used:
- Windows 11 built-in **Windows Defender Firewall with Advanced Security**
- Command Prompt (for testing ports)
- Telnet (for port testing)

---

## 🧪 Steps Performed:

1. **Opened Firewall Settings**
   - Searched and launched *Windows Defender Firewall with Advanced Security*.

2. **Created a New Inbound Rule**
   - Selected **Port**.
   - Chose **TCP** and specified the port number (example: 80).
   - Selected **Block the connection**.
   - Applied to **Domain**, **Private**, and **Public** profiles.
   - Named the rule `Block Port 80 Test`.

3. **Tested the Rule**
   - Used Telnet to connect:  
     ```
     telnet 127.0.0.1 80
     ```
   - Confirmed that the connection failed when the rule was active.

4. **Exported Firewall Configuration**
   - Exported the policy to a file named `firewall_config.wfw`.

---

## 📂 Files in this Task:
- `firewall_config.wfw` → Exported firewall rules.
- `README.md` → Steps and documentation for Task 4.

---

## 📌 Notes:
- This was done on my own system for safe, ethical testing.
- Only one port was blocked for demonstration purposes.
