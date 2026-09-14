<img width="720" height="898" alt="6965" src="https://github.com/user-attachments/assets/f10ca8a1-dd32-4809-89ed-126465f2c041" />
<img width="720" height="946" alt="6963" src="https://github.com/user-attachments/assets/9465bb54-1cc9-4434-b71e-ee1fd6b5e09f" />
<img width="720" height="713" alt="6964" src="https://github.com/user-attachments/assets/ade3abe0-1297-4614-84d6-3f852691a67e" />
<img width="720" height="943" alt="6957" src="https://github.com/user-attachments/assets/272f715d-8636-4389-92e9-d2194038e98b" />
<img width="720" height="786" alt="6959" src="https://github.com/user-attachments/assets/de072a90-1ee2-4408-b102-7f697dd17896" />
<img width="720" height="779" alt="6962" src="https://github.com/user-attachments/assets/57d27aed-2014-48cf-901e-af5427c0806d" />
<img width="720" height="715" alt="6961" src="https://github.com/user-attachments/assets/c3415914-f2c1-4779-b888-86cdfb36c018" />
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
