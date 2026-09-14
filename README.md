
# DVWA Security Lab

Practice writeup on Damn Vulnerable Web App. Tested locally for education only.

## Findings

### 1. SQLi Auth Bypass: `' OR '1'='1`
Bypassed login and listed all users
![Auth Bypass](Screenshot_20260914-030425-2.jpg)

### 2. UNION SQLi
Extracted user data with UNION attack
![UNION](Screenshot_20260914-022812-2.jpg)

### 3. Brute Force Module
No rate limiting at Low security level
![Bruteforce](Screenshot_20260914-024828-2.jpg)

## Mitigation
Use Prepared Statements / Parameterized Queries to prevent SQL injection.

## Disclaimer
For legal educational testing only on DVWA lab.<img width="720" height="943" alt="6957" src="https://github.com/user-attachments/assets/b6632597-3a99-424b-970b-58ceabf93f5b" />
<img width="720" height="946" alt="6963" src="https://github.com/user-attachments/assets/5edfdfc7-4d63-4b8f-8b7e-5defc03771b9" />
<img width="720" height="786" alt="6959" src="https://github.com/user-attachments/assets/56c0a14b-b4ac-46a1-b70c-3b84d9dfe769" />
<img width="720" height="779" alt="6962" src="https://github.com/user-attachments/assets/45111ed4-1200-4dcb-b037-13c9f355fe27" />
<img width="720" height="715" alt="6961" src="https://github.com/user-attachments/assets/c949c481-97fc-4a52-8614-0f7443b2ca94" />
<img width="720" height="1483" alt="6966" src="https://github.com/user-attachments/assets/584d8aa1-a0de-4d8c-ad8a-cfd357076479" />
