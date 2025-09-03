Task 1 – Web Application Security Testing (ZAP)

Tool:
OWASP ZAP v2.16.1

Target Application:
`http://testphp.vulnweb.com` – a deliberately vulnerable web application used for ethical security testing.

Scan Type:
- Spider Scan (Traditional + AJAX)
- Active Scan

Key Vulnerabilities Identified:
| Vulnerability                                | Risk Level | Description                                                                 |
|----------------------------------------------|------------|-----------------------------------------------------------------------------|
| Cross-Site Scripting (Reflected)             | High       | User input is reflected unsanitized, which can allow script execution.      |
| SQL Injection / SQL Injection – MySQL        | High       | SQL payloads in form fields were executed, showing injection vulnerability. |
| Content Security Policy (CSP) Header Missing | Medium     | No policy defined to control content loading and prevent injection attacks. |
| Absence of Anti-CSRF Tokens                  | Medium     | Forms lack CSRF protection, allowing unauthorized actions.                  |
| Server Information Leaks                     | Low        | Server details exposed via HTTP headers.                                    |

Mitigation Suggestions:
- Use parameterized queries to prevent SQL Injection
- Sanitize and validate all user input to block XSS
- Apply proper HTTP security headers (CSP, X-Content-Type-Options, etc.)
- Implement CSRF tokens for all sensitive forms
- Hide sensitive headers like `X-Powered-By` and `Server`

Screenshots:
- `zap-active-scan.png` – ZAP actively scanning the target web application
- `zap-alerts-tab.png` – Vulnerabilities discovered (e.g., XSS, SQLi)
- `zap-alert-details.png` – Detailed view of a high-risk alert (SQLi)

Reflections:
This was my first full hands-on web application scan using OWASP ZAP. I learned how to:
- Launch both spider and active scans
- Read and interpret alert types, risk levels, and mitigation tips
- Navigate ZAP’s interface and explore live request/response data

This experience gave me real-world insight into how automated scanners help analysts identify and respond to common vulnerabilities.

---

  Files:
- `ZAP_Scan_Report.pdf`
- `/screenshots/` folder with 3 visuals
