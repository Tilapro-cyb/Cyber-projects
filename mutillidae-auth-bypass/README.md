# Mutillidae Authentication Bypass

## Objective
Test the Mutillidae vulnerable web application to identify and exploit authentication flaws.

## Tools Used
- Mutillidae (OWASP Web App)
- Burp Suite
- Firefox Developer Tools
- Basic payloads (e.g., `' OR '1'='1`)

## Method
1. **Accessed login page** of Mutillidae hosted locally.
2. Interacted with login form to understand parameter behavior.
3. Tested common SQL Injection payloads in the username/password fields.
4. Successfully bypassed authentication using `' OR '1'='1` as input.

## Key Findings
- The login page is vulnerable to SQL Injection.
- Input is not sanitized or validated on the server side.

## What I Learned
- Basics of SQL injection in login forms.
- Importance of input validation and parameterized queries.

## Next Steps
- Try login bypass using Burp Suite’s Intruder tool.
- Explore privilege escalation possibilities inside the app.
