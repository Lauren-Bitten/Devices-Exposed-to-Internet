# 🛑 Devices Exposed to the Internet: Incident Summary

## 📌 Overview
A Windows device (`lauren-win-targ`) was accidentally left internet-facing for **one day**. Within hours, malicious actors attempted to brute-force their way in.

---

## 🔍 **Findings**
- **304 failed logins** for the `labuser` account.
- Multiple **unique IPs** attempted unauthorized access.
- The **MITRE ATT&CK framework** was used to map attack techniques.

---

## 📡 **Attack Breakdown**
| ActionType  | Remote IP Address      | Device Name       | Attempts |
|------------|----------------------|----------------|-----------|
| LogonFailed | 185.243.96.107      | lauren-win-targ | 75        |
| LogonFailed | 139.180.154.155     | lauren-win-targ | 66        |
| LogonFailed | 49.51.166.101       | lauren-win-targ | 40        |
| LogonFailed | 185.156.73.77       | lauren-win-targ | 24        |
| LogonFailed | 178.20.129.235      | lauren-win-targ | 2         |

✅ **No unauthorized access was detected**.  

---

## 🕵️ **MITRE ATT&CK Techniques Identified**
- **T1110.001** - Brute Force (Password Guessing)
- **T1133** - External Remote Services
- **T1078** - Valid Accounts
- **T1190** - Exploit Public-Facing Application

---

## 🎯 **Lessons Learned**
🔸 Never expose devices to the internet unnecessarily.  
🔸 Implement **strong password policies & lockout mechanisms**.  
🔸 Monitor logs **continuously** to detect suspicious behavior.

🚀 **Full breakdown available in this repo!**
