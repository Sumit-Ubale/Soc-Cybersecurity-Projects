# Network Scanning Findings Report

## 🎯 Target Information
- **Target:** Metasploitable-2
- **IP Address:** 192.168.0.125
- **Operating System:** Linux (Ubuntu-based)
- **Purpose:** Enumeration and attack surface identification

---

## 🔎 Open Ports and Service Analysis

### Port 21 – FTP (vsftpd 2.3.4)
- **Risk:** Anonymous login enabled and plaintext authentication
- **Impact:** Attackers can gain unauthorized access or upload malicious files
- **Severity:** High

---

### Port 22 – SSH (OpenSSH 4.7p1)
- **Risk:** Outdated SSH version
- **Impact:** Susceptible to brute-force attacks and legacy vulnerabilities
- **Severity:** Medium

---

### Port 23 – Telnet
- **Risk:** Credentials transmitted in plaintext
- **Impact:** Password interception through network sniffing
- **Severity:** High

---

### Port 25 – SMTP (Postfix)
- **Risk:** Possible user enumeration
- **Impact:** Helps attackers identify valid email accounts
- **Severity:** Medium

---

### Port 80 – HTTP (Apache 2.2.8)
- **Risk:** Outdated web server version
- **Impact:** Vulnerable to known web application attacks
- **Severity:** Medium

---

### Ports 139 & 445 – SMB (Samba 3.x)
- **Risk:** Known remote code execution vulnerabilities
- **Impact:** Full system compromise possible
- **Severity:** Critical

---

### Ports 512 / 513 / 514 – rsh / rlogin / shell
- **Risk:** Legacy remote access services
- **Impact:** Authentication bypass and remote command execution
- **Severity:** Critical

---

### Port 3306 – MySQL (5.0.51a)
- **Risk:** Old database version
- **Impact:** Unauthorized database access and data leakage
- **Severity:** High

---

### Port 8180 – Apache Tomcat
- **Risk:** Exposed application server
- **Impact:** Abuse of management interfaces and web exploits
- **Severity:** High

---

## 🧠 Overall Risk Assessment
The target system exposes **multiple high-risk services simultaneously**.
The combination of:
- Outdated software
- Plaintext protocols
- Legacy remote services

creates a **critical security posture**, making the system highly vulnerable
to both automated and manual attacks.

---

## 🛡️ General Recommendations
- Disable unnecessary services
- Remove legacy protocols
- Enforce encrypted communication
- Patch and update all services
- Apply least privilege principles

---

## ✅ Conclusion
This enumeration phase successfully identified the target’s attack surface
and highlighted critical weaknesses.  
These findings provide a strong foundation for the **vulnerability scanning phase**
in a complete VAPT lifecycle.
