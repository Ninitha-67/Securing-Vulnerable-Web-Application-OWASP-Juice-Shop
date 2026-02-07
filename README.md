# 🔐 Securing a Vulnerable Web Application using OWASP Juice Shop
*A Practical Web Application Security Assessment and Hardening Project*

---

## 📌 Quick Summary
This project demonstrates a practical web application security assessment conducted on OWASP Juice Shop in a controlled lab environment. The objective was to identify common web vulnerabilities, analyze their impact, and apply or propose appropriate security mitigations aligned with OWASP Top 10 standards.

---

## 📖 Introduction
Web application security is a critical domain in cybersecurity, as many real-world breaches occur due to insecure coding practices, broken authentication mechanisms, improper access control, and security misconfigurations.

OWASP Juice Shop is an intentionally vulnerable web application developed to showcase common security flaws. This project simulates a real-world penetration testing and hardening workflow in a safe and ethical environment for educational purposes.

---

## 🎯 Objectives
- Understand common web application vulnerabilities  
- Deploy OWASP Juice Shop in a controlled lab environment  
- Perform ethical vulnerability assessment  
- Map findings to OWASP Top 10  
- Apply or propose security mitigations  
- Validate fixes through retesting  
- Document findings in a structured manner  

---

## 🛠️ Tools & Technologies
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
1. Deployment of OWASP Juice Shop in an isolated lab  
2. Application reconnaissance and mapping  
3. Vulnerability identification using manual and tool-based testing  
4. Controlled exploitation for validation  
5. Security hardening and mitigation planning  
6. Retesting to confirm vulnerability mitigation  
7. Documentation and reporting  

---

## 🛑 Vulnerabilities Identified
- SQL Injection  
- Cross-Site Scripting (XSS)  
- Broken Authentication  
- Broken Access Control  
- Security Misconfiguration  
- Sensitive Data Exposure  

All vulnerabilities were mapped to the **OWASP Top 10** framework.

---

## 📊 Findings Summary

| Vulnerability | OWASP Top 10 Category | Impact | Mitigation | Retest Status |
|--------------|----------------------|--------|------------|---------------|
| SQL Injection | Injection | Data compromise | Parameterized queries | Not reproducible |
| XSS | Cross-Site Scripting (XSS) | Script execution | Input sanitization, CSP | Blocked |
| Broken Auth | Identification and Authentication Failures | Account takeover | Strong auth policies | Improved |
| Access Control | Broken Access Control | Privilege escalation | RBAC enforcement | Prevented |
| Misconfiguration | Security Misconfiguration | Info disclosure | Hardening configs | Reduced |
| Data Exposure | Sensitive Data Exposure / Cryptographic Failures | Data leakage | HTTPS, secrets mgmt | Secured |

---

## 🛠️ Security Fixes & Mitigations

### SQL Injection
- **Fix:** Server-side validation and prepared statements  
- **Result:** Injection attempts blocked  

### Cross-Site Scripting (XSS)
- **Fix:** Output encoding and Content Security Policy  
- **Result:** Script execution prevented  

### Broken Authentication
- **Fix:** Strong password policy and secure sessions  
- **Result:** Reduced unauthorized access  

### Broken Access Control
- **Fix:** Role-based access control  
- **Result:** Unauthorized access prevented  

### Security Misconfiguration
- **Fix:** Disabled debug mode, hardened configurations  
- **Result:** Reduced information leakage  

### Sensitive Data Exposure
- **Fix:** HTTPS enforcement and credential protection  
- **Result:** Improved confidentiality  

Some mitigations were applied at configuration level, while others are proposed as secure design recommendations based on OWASP best practices.

---

## 🔁 Validation & Retesting
All identified vulnerabilities were re-tested after mitigation. Previously exploitable issues were no longer reproducible or were significantly reduced.

---

## 🎓 Learning Outcomes
- Gained hands-on experience in web application security testing  
- Improved understanding of OWASP Top 10 vulnerabilities  
- Learned structured vulnerability assessment and reporting  
- Practiced ethical security testing in a controlled environment

---

## 📄 Documentation
📄 **Full Project Report:**  
`Project-Report/OWASP_Juice_Shop_Security_Report.pdf`

---

## ⚠️ Scope & Limitations
- Testing was limited to OWASP Juice Shop in a local lab  
- No real-world or production systems were targeted  
- This project focuses on educational security assessment only  

---

## ⚖️ Ethical Disclaimer
This project was conducted strictly for educational and ethical purposes in a controlled environment. Unauthorized testing on real-world systems is strictly prohibited.

---

## 🏁 Conclusion
This project demonstrates a structured approach to web application security testing, vulnerability analysis, and mitigation. It highlights the importance of proactive security assessments and secure application design aligned with industry best practices.

---

## 📚 References
- OWASP Top 10  
- OWASP Juice Shop Documentation  
- OWASP Testing Guide  
