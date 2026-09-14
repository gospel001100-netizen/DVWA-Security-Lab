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
For legal educational testing only on DVWA lab.
