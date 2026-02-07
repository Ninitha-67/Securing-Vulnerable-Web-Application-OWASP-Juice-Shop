# 🔐 Securing a Vulnerable Web Application using OWASP Juice Shop
*A Practical Web Application Security Assessment and Hardening Project*

---

## 📌 Introduction
Web application security is a critical component of modern cybersecurity. A significant number of real-world security breaches occur due to insecure application logic, weak authentication mechanisms, improper access control, and misconfigurations.

OWASP Juice Shop is an intentionally vulnerable web application designed to demonstrate common security flaws listed in the OWASP Top 10. This project simulates a real-world penetration testing scenario in a controlled environment to identify, analyze, and mitigate web application vulnerabilities in an ethical manner.

---

## 🎯 Objectives
- Understand common web application vulnerabilities  
- Deploy a vulnerable web application in a secure lab environment  
- Perform ethical security testing using industry-standard tools  
- Map identified vulnerabilities to OWASP Top 10 categories  
- Apply appropriate security fixes and configurations  
- Validate mitigation effectiveness through retesting  
- Document findings and security recommendations  

---

## 🛠️ Tools & Technologies Used
- OWASP Juice Shop  
- Docker  
- Kali Linux  
- Ubuntu Linux  
- VirtualBox  
- Burp Suite  
- Nmap  
- Web Browser (Firefox / Chrome)  

---

## 🧪 Environment Setup
- **Host OS:** Windows  
- **Guest OS:**
  - Ubuntu (Target Server)
  - Kali Linux (Attacker Machine)
- **Deployment Method:** Docker Container  
- **Network Configuration:** Host-Only / Internal Network  

---

## ⚙️ Methodology
This project follows a structured and ethical security testing methodology:

1. Deployment of OWASP Juice Shop in an isolated environment  
2. Initial reconnaissance and application mapping  
3. Identification of vulnerabilities using manual and tool-based testing  
4. Controlled exploitation of vulnerabilities for validation  
5. Implementation of security fixes and hardening measures  
6. Retesting to ensure vulnerabilities are mitigated  
7. Documentation of findings and recommendations  

---

## 🛑 Vulnerabilities Identified
The following vulnerabilities were identified during the assessment:

- SQL Injection  
- Cross-Site Scripting (XSS)  
- Broken Authentication  
- Broken Access Control  
- Security Misconfiguration  
- Sensitive Data Exposure  

All findings were mapped to relevant **OWASP Top 10** categories.

---

## 🛠️ Security Fixes & Mitigations

### 1. SQL Injection
**Issue:**  
Improper input handling allowed malicious SQL queries.

**Fix Applied:**  
- Implemented server-side input validation  
- Used parameterized queries and prepared statements  

**Outcome:**  
SQL injection attempts were successfully blocked.

---

### 2. Cross-Site Scripting (XSS)
**Issue:**  
User-supplied input was rendered without sanitization.

**Fix Applied:**  
- Input validation and output encoding  
- Applied Content Security Policy (CSP)  

**Outcome:**  
Injected scripts were neutralized.

---

### 3. Broken Authentication
**Issue:**  
Weak password policies and improper session handling.

**Fix Applied:**  
- Enforced strong password policies  
- Implemented secure session management  

**Outcome:**  
Unauthorized access attempts were reduced.

---

### 4. Broken Access Control
**Issue:**  
Restricted resources were accessible without proper authorization.

**Fix Applied:**  
- Implemented role-based access control (RBAC)  
- Enforced server-side authorization checks  

**Outcome:**  
Unauthorized resource access was prevented.

---

### 5. Security Misconfiguration
**Issue:**  
Default configurations and verbose error messages exposed system details.

**Fix Applied:**  
- Disabled debug modes  
- Hardened server and container configurations  

**Outcome:**  
Information leakage was minimized.

---

### 6. Sensitive Data Exposure
**Issue:**  
Sensitive information was transmitted without proper protection.

**Fix Applied:**  
- Enforced HTTPS  
- Secured credentials and secrets  

**Outcome:**  
Data confidentiality and integrity were improved.

---

## 🔁 Validation & Retesting
All applied security fixes were validated by retesting the previously exploited vulnerabilities.  
Post-mitigation testing confirmed that vulnerabilities were no longer reproducible.

---

## 📄 Documentation
- Detailed vulnerability analysis and mitigation steps are documented in the **Project Report PDF**  
- Findings include impact assessment and security recommendations  

---

## ⚠️ Ethical Disclaimer
This project was conducted strictly for **educational and ethical purposes** within a controlled laboratory environment. No real-world systems were targeted or harmed.

---

## 📚 References
- OWASP Top 10  
- OWASP Juice Shop Official Documentation  
- OWASP Testing Guide  

---

## 🏁 Conclusion
This project demonstrates practical knowledge of web application security testing, vulnerability assessment, and mitigation aligned with industry best practices. It emphasizes the importance of secure application design and proactive security assessments.
