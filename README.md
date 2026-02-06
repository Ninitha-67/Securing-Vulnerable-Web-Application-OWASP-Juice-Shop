# # Securing a Vulnerable Web Application (OWASP Juice Shop)

This project demonstrates the complete lifecycle of securing a deliberately vulnerable web application:
**Deployment → Vulnerability Identification → Root Cause Analysis → Mitigation Recommendations → Validation (Re-testing)**

⚠️ Educational use only. Tested in an isolated lab environment.

## Project Overview
This project demonstrates security testing of the OWASP Juice Shop vulnerable web application in a controlled lab environment using Kali Linux and Docker.

## Tools & Technologies
- Kali Linux
- Ubuntu Server
- Docker
- OWASP Juice Shop
- VirtualBox

## Environment Setup
- Attacker Machine: Kali Linux
- Target Machine: Ubuntu Server
- Application: OWASP Juice Shop (Dockerized)
- Network: Host-Only / NAT

## How to Run (Local Lab)

### Target (Ubuntu)
sudo apt update
sudo apt install docker.io -y
sudo docker run -d --name juice -p 3000:3000 bkimminich/juice-shop

### Access (Kali Browser)
Attacker (Kali):
- Open [http://< Ubantu IP >:3000]
## Vulnerabilities Tested
- Authentication Bypass
- SQL Injection
- Cross-Site Scripting (XSS)
- Broken Access Control

## Key Findings (OWASP-aligned)
- DOM-Based XSS (Injection)
- Broken Access Control (Admin route access attempts)
- Token Exposure Risk (LocalStorage)
- Business Logic Risk (Quantity manipulation attempts)

## Security Hardening (Recommendations)
- Input sanitization + output encoding + CSP for XSS prevention
- Server-side authorization checks + RBAC for admin routes
- Server-side validation for quantity and pricing logic
- Store tokens using HttpOnly cookies + token expiry/rotation

## Validation (Re-testing)
- Re-tested payloads to verify controls (blocked/sanitized behavior observed where applicable)

## Learning Outcomes
- Understanding vulnerable web applications
- Hands-on penetration testing practice
- Secure deployment using Docker
- Ethical hacking methodology

## Disclaimer
This project is created strictly for educational purposes in a controlled environment. No real-world systems were harmed or targeted.
