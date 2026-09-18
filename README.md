# VortexTech Cyber Security Internship – Week 3

## Basic Security Audit of a Sample Website

This project was completed as part of my **VortexTech Cyber Security Internship – Week 3** task.

For this task, I performed a basic security audit of **OWASP Juice Shop** in a local practice environment. The purpose was to test common web security issues and document the results.

## What I Did

- Set up OWASP Juice Shop locally using Docker.
- Tested the search function for Cross-Site Scripting (XSS).
- Tested the login page for SQL Injection.
- Checked authentication error messages.
- Used browser Developer Tools to inspect network requests and API responses.
- Checked for exposed files and sensitive information.
- Documented the findings with screenshots, impact, and possible fixes.

## Findings

Three main security findings were identified:

1. **Cross-Site Scripting (XSS)**
2. **SQL Injection / Authentication Bypass**
3. **Sensitive Information Disclosure through an Exposed FTP Directory**

## Tools Used

- Kali Linux
- Docker
- OWASP Juice Shop
- Web Browser Developer Tools

## How to Run OWASP Juice Shop

Pull the Juice Shop Docker image:

```bash
sudo docker pull bkimminich/juice-shop

Run the application:

sudo docker run -d -p 3000:3000 bkimminich/juice-shop

Then open the website in a browser:

http://localhost:3000

Report

The complete security audit report is included in this repository:

VortexTech_Week3_Security_Audit_Report.pdf

The report includes the testing steps, screenshots, findings, potential impact, and remediation suggestions.

Disclaimer

All testing was performed on OWASP Juice Shop, a deliberately vulnerable practice application running locally. No real production website was tested.
