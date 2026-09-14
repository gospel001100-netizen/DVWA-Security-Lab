# DVWA-Security-Lab
# DVWA Security LabPractice writeup on Damn Vulnerable Web App. Tested locally for education only.**Findings:**1. SQLi Auth Bypass: `' OR '1'='1` - Bypassed login2. UNION SQLi: Extracted user data  3. Brute Force: No rate limiting at Low level**Fix:** Use Prepared Statements to block injection.Disclaimer: Legal testing only.
