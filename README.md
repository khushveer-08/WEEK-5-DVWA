# Week 6 – Web Security & Vulnerability Testing (VAPT Basics)

## 📌 Project Overview

This project is part of my Week 6 cybersecurity practical on Web Security and Vulnerability Assessment and Penetration Testing (VAPT).

The project focuses on understanding common web application vulnerabilities and performing basic security testing in a controlled lab environment using DVWA, Burp Suite, and OWASP ZAP.

---

## 🎯 Objectives

- Understand the basics of VAPT.
- Study common OWASP web vulnerabilities.
- Set up DVWA for security testing.
- Perform basic SQL Injection testing.
- Perform Reflected and Stored XSS testing.
- Capture HTTP requests using Burp Suite.
- Scan DVWA using OWASP ZAP.
- Identify vulnerabilities and their risk levels.
- Understand vulnerability mitigation techniques.

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux | Security testing environment |
| DVWA | Vulnerable web application for practice |
| Burp Suite Community Edition | HTTP request/response analysis |
| OWASP ZAP | Web vulnerability scanning |
| Docker / XAMPP | DVWA setup |

---

## 🔐 Vulnerabilities Studied

### 1. SQL Injection

SQL Injection occurs when an application does not properly validate user input and an attacker can manipulate database queries.

**Possible impact:**
- Unauthorized database access
- Data exposure
- Data modification

**Prevention:**
- Use parameterized queries
- Validate input
- Use secure database permissions

---

### 2. Cross-Site Scripting (XSS)

XSS occurs when malicious script content is injected into a web application and executed in another user's browser.

Types tested:

- Reflected XSS
- Stored XSS

**Possible impact:**
- Session theft
- Malicious script execution
- User data exposure

**Prevention:**
- Input validation
- Output encoding
- Content Security Policy (CSP)

---

### 3. Broken Authentication

Broken authentication can occur when authentication and session management are implemented insecurely.

**Possible impact:**
- Account compromise
- Unauthorized access
- Session-related attacks

**Prevention:**
- Strong authentication
- Secure session management
- Multi-factor authentication

---

### 4. Security Misconfiguration

Security misconfiguration occurs when applications, servers, or security settings are incorrectly configured.

**Possible impact:**
- Information disclosure
- Unauthorized access
- Increased attack surface

**Prevention:**
- Secure configuration
- Disable unnecessary services
- Keep software updated
- Remove default credentials

---

## 🧪 Practical Testing

### DVWA

DVWA was used as the intentionally vulnerable target application in a local lab environment.

Testing included:

- SQL Injection
- Reflected XSS
- Stored XSS

Screenshots of the testing process are available in the `Screenshots` folder.

---

## 📡 Burp Suite

Burp Suite Community Edition was used to:

- Intercept HTTP requests
- Inspect request parameters
- View server responses
- Understand client-server communication

Relevant screenshots are available in:

`Screenshots/Burp-Suite/`

---

## 🔍 OWASP ZAP

OWASP ZAP was used to perform an automated vulnerability scan against the locally hosted DVWA application.

The scan was used to identify security weaknesses and categorize findings according to their risk level.

The ZAP report is available in:

`ZAP-Report/`

---

## 📊 Findings

| Vulnerability | Risk Level | Possible Impact |
|---|---|---|
| SQL Injection | High | Database/data exposure |
| Stored XSS | High/Medium | Script execution |
| Reflected XSS | Medium | Malicious script execution |
| Security Misconfiguration | Medium | Information exposure |

> Risk levels may vary depending on the specific configuration and scan results.

---

## 🛡️ Mitigation

Recommended security measures include:

- Use parameterized SQL queries.
- Validate and sanitize user input.
- Encode output before displaying it.
- Use secure authentication mechanisms.
- Apply proper session management.
- Configure security headers.
- Disable unnecessary services.
- Keep applications and servers updated.
- Avoid default credentials.
- Follow secure coding practices.

---

## 📚 Learning Outcomes

Through this practical, I learned:

- Basics of VAPT.
- Common web application vulnerabilities.
- How SQL Injection and XSS work.
- How to use Burp Suite for request analysis.
- How to use OWASP ZAP for vulnerability scanning.
- How to identify and classify security findings.
- Importance of vulnerability mitigation.

---

## 📁 Repository Structure

```text
Week-6-Web-Security-VAPT/
│
├── README.md
├── Report/
├── PPT/
├── Screenshots/
