# AWS Application Security Testing Lab

## Overview
This project demonstrates the deployment and security testing of a vulnerable web application using AWS EC2 and Docker. The objective of this lab is to practice identifying common web application vulnerabilities aligned with the OWASP Top 10.

## Technologies Used
- AWS EC2
- Docker
- OWASP Juice Shop
- Burp Suite
- OWASP ZAP
- Ubuntu Linux

## Lab Architecture

User (Security Tester)
        │
        │ HTTP Requests
        │
AWS EC2 Instance (Ubuntu)
        │
Docker Container
        │
OWASP Juice Shop (Vulnerable Web App)

## Deployment Steps

1. Launch AWS EC2 Ubuntu instance
2. Configure security group (SSH + HTTP)
3. Install Docker
4. Deploy OWASP Juice Shop container
5. Access application via public IP

## Security Testing

The following vulnerabilities were tested:

- SQL Injection
- Cross-Site Scripting (XSS)
- Broken Authentication
- Sensitive Data Exposure

Detailed findings are documented in the vulnerabilities folder.

## Screenshots

Application running:

![Juice Shop](screenshots/juice-shop-running.png)

## Learning Outcome

This lab provided hands-on experience with:

- Deploying vulnerable applications
- Conducting web application security testing
- Understanding OWASP Top 10 vulnerabilities
- Documenting security findings

## Future Improvements

- Integrate automated scanning with OWASP ZAP
- Implement SIEM logging for attack detection
- Add remediation examples
