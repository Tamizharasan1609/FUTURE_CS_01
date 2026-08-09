# Web Application Vulnerability Assessment — Task 1

## Website Tested
http://demo.testfire.net (a public practice site built for security testing)

## Scope
This assessment was conducted using **passive and automated scanning techniques only**.

**Allowed:**
- Public-facing pages only
- Passive scanning
- Header and cookie configuration checks

**Not performed:**
- Login bypass
- Manual exploitation
- Brute-force attacks
- Denial-of-Service (DoS) testing

## Tools Used
| Tool | Purpose |
|---|---|
| Nmap | Network and port scanning |
| OWASP ZAP | Automated web application security assessment |
| Chrome DevTools | HTTP response header and cookie inspection |

## Summary of Findings
- 4 open ports identified (53, 80, 443, 8080)
- 15 security alert categories flagged by OWASP ZAP
- Missing security headers (CSP, X-Frame-Options, HSTS, X-Content-Type-Options)
- Session cookie missing `Secure` and `SameSite` attributes
- Server version disclosure via `Server` header
- Overall Risk Rating: **Medium**

## Deliverables in This Folder
- `Web_Vulnerability_Assessment_demo_testfire_net.pptx` — Full vulnerability assessment report
- `Nmap_scan.png` — Nmap scan evidence
- `ZAP_alerts.png` — OWASP ZAP scan evidence
- `DevTools_headers.png` — Response header evidence
- `DevTools_cookies.png` — Cookie configuration evidence

## Author
Tamizharasan S
Future Interns — Cyber Security Internship
