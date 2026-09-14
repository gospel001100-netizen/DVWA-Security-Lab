# DVWA Security Lab

Practice writeup on Damn Vulnerable Web App. Tested locally for education only.

## Findings

### 1. SQLi Auth Bypass: `' OR '1'='1`
Bypassed login and listed all users
![Auth Bypass](Screenshot_20260914-030425-2.jpg)
<img src="Screenshot_20260914-030425-2.jpg" width="700"/>

### 2. UNION SQLi
Extracted user data with UNION attack
![UNION](Screenshot_20260914-022812-2.jpg)
<img src="Screenshot_20260914-022812-2.jpg" width="700"/>

### 3. Brute Force Module
No rate limiting at Low security level
![Bruteforce](Screenshot_20260914-024828-2.jpg)
<img src="Screenshot_20260914-024828-2.jpg" width="700"/>

### 4. Finding 4
Description of what you found here
![Screenshot 4](Screenshot_4.jpg)
<img src="Screenshot_4.jpg" width="700"/>

### 5. Finding 5
Description of what you found here
![Screenshot 5](Screenshot_5.jpg)
<img src="Screenshot_5.jpg" width="700"/>

### 6. Finding 6
Description of what you found here
![Screenshot 6](Screenshot_6.jpg)
<img src="Screenshot_6.jpg" width="700"/>

### 7. Finding 7
Description of what you found here
![Screenshot 7](Screenshot_7.jpg)
<img src="Screenshot_7.jpg" width="700"/>

## Mitigation
Use Prepared Statements / Parameterized Queries to prevent SQL injection.

## Disclaimer
For legal educational testing only on DVWA lab.
