# DVWA Security Lab 🔒

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Tools](https://img.shields.io/badge/Tools-DVWA%20%7C%20BurpSuite%20%7C%20Kali%20Linux-blue)

Practice writeup on Damn Vulnerable Web App. Tested locally for education only.

## Tools Used
- **DVWA** - Damn Vulnerable Web Application
- **BurpSuite Community** - For intercepting requests  
- **Kali Linux / Android** - Testing environment
- **Firefox** - Browser for testing

## Findings

### 1. SQLi Auth Bypass: `' OR '1'='1`
Bypassed login and listed all users

![Auth Bypass](1-auth-bypass.jpg)
<img src="1-auth-bypass.jpg" width="700"/>

### 2. UNION SQLi
Extracted user data with UNION attack

![UNION](2-union-sqli.jpg)
<img src="2-union-sqli.jpg" width="700"/>

### 3. Brute Force Module
No rate limiting at Low security level

![Bruteforce](3-bruteforce.jpg)
<img src="3-bruteforce.jpg" width="700"/>

### 4. XSS
Reflected XSS found at Low security level

![XSS](4-xss.jpg)
<img src="4-xss.jpg" width="700"/>

### 5. Command Injection
OS commands executed via input field

![Command Injection](5-command-injection.jpg)
<img src="5-command-injection.jpg" width="700"/>

### 6. File Inclusion
Local file inclusion vulnerability

![File Inclusion](6-file-inclusion.jpg)
<img src="6-file-inclusion.jpg" width="700"/>

### 7. Security Level
DVWA set to Low security for testing

![Low Security](7-low-security.jpg)
<img src="7-low-security.jpg" width="700"/>

## Mitigation
**SQL Injection**: Use Prepared Statements / Parameterized Queries.  
**XSS**: Implement input validation and output encoding.  
**Brute Force**: Add rate limiting and account lockout.  
**Command Injection**: Use allowlists and avoid system calls with user input.  
**File Inclusion**: Disable `allow_url_include` and validate file paths.

## Disclaimer
This project is for legal educational testing only on the DVWA lab environment. Do not use these techniques on systems without explicit permission.
