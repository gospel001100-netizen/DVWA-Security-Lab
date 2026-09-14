# DVWA Security Lab

Practice writeup on Damn Vulnerable Web App. Tested locally for education only.

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
Use Prepared Statements / Parameterized Queries to prevent SQL injection.

## Disclaimer
For legal educational testing only on DVWA lab.<img width="720" height="715" alt="6961" src="https://github.com/user-attachments/assets/16720a47-85a9-4c45-a02a-3fd8763f4c14" />
<img width="720" height="943" alt="6957" src="https://github.com/user-attachments/assets/837d0cf7-0282-4b29-a37c-75f6c24d002d" />
<img width="720" height="946" alt="6963" src="https://github.com/user-attachments/assets/356e615f-78be-4720-9656-fdac35254306" />
<img width="720" height="786" alt="6959" src="https://github.com/user-attachments/assets/64208000-bffc-414b-9122-e362f482cca8" />
<img width="720" height="779" alt="6962" src="https://github.com/user-attachments/assets/7fd93ca6-3347-450e-854c-4f2606cee845" />
<img width="720" height="713" alt="6964" src="https://github.com/user-attachments/assets/39c2aa7d-e1d2-479f-8e0b-51d4cff68f6f" />
<img width="720" height="898" alt="6965" src="https://github.com/user-attachments/assets/d6426df6-dd97-4edf-9941-d8a4d02f3363" />
