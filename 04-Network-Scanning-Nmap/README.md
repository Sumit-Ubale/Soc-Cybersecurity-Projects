# Network Scanning & Enumeration using Nmap

## 📌 Objective
The objective of this project is to perform **network scanning and service enumeration**
to identify exposed services, software versions, and potential attack surfaces
on a target system.  
This activity represents the **reconnaissance and enumeration phase** of a real-world
Red Team / VAPT assessment.

---

## 🧪 Lab Setup
- **Attacker Machine:** Kali Linux
- **Target Machine:** Metasploitable-2 (Intentionally vulnerable VM)
- **Network Type:** Host-only network
- **Target IP:** 192.168.0.125

This lab was conducted in a **controlled and legal environment** for learning purposes only.

---

## 🛠️ Tool Used
- **Nmap (Network Mapper)**  
  Used for host discovery, port scanning, service detection, and OS fingerprinting.

---

## 🔍 Scanning Techniques Performed

### 1️⃣ Host Discovery
Used to verify whether the target machine is alive on the network.

### 2️⃣ Basic Port Scanning
Identified open TCP ports and exposed services.

### 3️⃣ Service & Version Enumeration
Detected exact service names and software versions running on open ports.

### 4️⃣ Aggressive Scan
Performed OS detection, script scanning, and advanced service enumeration
to gather maximum information about the target.

---

## 📊 Key Findings (Summary)
- Multiple **legacy and insecure services** were exposed.
- Several services were running **outdated software versions**.
- High-risk services such as **FTP, Telnet, SMB, rsh, and MySQL** were publicly accessible.
- The system presented a **large attack surface**, increasing the risk of exploitation.

---

## 🔐 Security Risks Identified
- Plaintext authentication services (FTP, Telnet)
- Legacy remote access services (rsh, rlogin)
- Old web and database software versions
- Weak default configurations commonly abused by attackers

---

## 🛡️ Recommended Mitigations
- Disable unused and legacy services
- Replace Telnet and FTP with secure alternatives (SSH, SFTP)
- Apply regular patching and updates
- Restrict access using firewall rules
- Enforce strong authentication mechanisms

---

## 🎯 Learning Outcome
Through this project, I gained hands-on experience in:
- Network reconnaissance
- Understanding attack surfaces
- Service and version enumeration
- Mapping exposed services to potential security risks

This project strengthened my **Red Team mindset** while also improving
my **defensive security awareness**.

---

## ⚠️ Disclaimer
This project was performed strictly for **educational purposes**
on an intentionally vulnerable system within a private lab environment.
Unauthorized scanning of real systems is illegal.
