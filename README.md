# 🔒 Web Vulnerability Assessment using DVWA & Burp Suite

## 📌 Overview

This project was completed as **Task 2** of my Cyber Security Internship. The objective was to identify common web vulnerabilities using **DVWA (Damn Vulnerable Web Application)** and inspect HTTP requests using **Burp Suite**.

---

## 🎯 Objective

- Identify common web vulnerabilities.
- Perform Reflected Cross-Site Scripting (XSS) testing.
- Perform SQL Injection testing.
- Capture and inspect HTTP requests using Burp Suite.
- Document findings and mitigation techniques.

---

## 🛠️ Tools Used

- Kali Linux
- DVWA (Damn Vulnerable Web Application)
- Burp Suite Community Edition
- Apache
- MySQL
- Firefox Browser

---

## 🧪 Tests Performed

### 1. Reflected XSS

**Payload**

```html
<script>alert('XSS')</script>
```

**Result**

The JavaScript executed successfully and displayed an alert box, confirming a Reflected XSS vulnerability.

---

### 2. SQL Injection

**Payload**

```sql
1' OR '1'='1
```

**Result**

The application returned multiple user records, confirming a SQL Injection vulnerability.

---

## 🌐 Burp Suite Analysis

Burp Suite Proxy was used to intercept and inspect HTTP requests between the browser and DVWA.

Captured information included:

- HTTP Methods
- Request Headers
- Parameters
- Cookies
- Server Responses

---

## 📊 Findings

| Vulnerability | Status | Severity |
|--------------|--------|----------|
| Reflected XSS | Detected | High |
| SQL Injection | Detected | Critical |

---

## 🛡️ Mitigation

### XSS

- Input Validation
- Output Encoding
- Content Security Policy (CSP)
- HTML Sanitization
- HttpOnly Cookies

### SQL Injection

- Prepared Statements
- Parameterized Queries
- Input Validation
- Least Privilege
- Generic Error Messages

---

## 📂 Repository Structure

```
internSpark-task-2/
│
├── README.md
├── Web_Vulnerability_Assessment_Report.pdf
├── screenshots/
└── payloads.txt
```

---

## 📄 Report

A detailed assessment report is included in:

**Web_Vulnerability_Assessment_Report.pdf**

---

## 👨‍💻 Author

**Raja Sabarinath**

Cyber Security Intern
