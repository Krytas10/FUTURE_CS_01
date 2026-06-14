# FUTURE_CS_01
Passive Vulnerability Assessment and Security Baseline Report on demo.testfire.net using Nmap, OWASP ZAP, and Browser DevTools. Completed for the Future Interns Cyber Security track.

# Task 1: Vulnerability Assessment Report for a Live Website

📌 Project Overview
This repository contains a professional, non-intrusive Passive Vulnerability Assessment Report conducted on the demonstration retail banking web application, Altoro Mutual (`demo.testfire.net`). The primary objective of this project was to analyze external network-layer visibility, server configuration behaviors, and client-side response configurations to establish a security baseline from a defensive perspective.

🛠️ Tools & Technologies Used
* Nmap: Passive network service enumeration and port visibility mapping.
* OWASP ZAP: Automated passive analysis of traffic patterns and security misconfigurations.
* Browser Developer Tools:** Manual inspection of HTTP response headers and transport properties.
* Canva: Professional document design and reporting layout.

🔍 Key Findings Summary
The passive assessment successfully identified 5 critical configuration oversights:
1. Insecure Data Transmission (HTTP):** Cleartext data transmission without forced SSL/TLS redirection.
2. Server Banner Version Disclosure:** Verbose infrastructure software details broadcasted in HTTP headers (`Apache-Coyote/1.1`).
3. Missing Security Response Headers:** Total absence of client-side protections (`X-Frame-Options`, `CSP`, `HSTS`).
4. Session Cookie Misconfiguration:** Critical tracking cookies lack the `Secure` and `HttpOnly` security flags.
5. Exposure of Public Management Ports:** Alternative service port `8080` left reachable via the open internet.

📂 Deliverables Included
* `Vulnerability_Assessment_Report.pdf`: The complete, client-ready vulnerability assessment report.
* `/screenshots`: Directory containing raw terminal outputs, OWASP ZAP alerts, and browser developer tool evidence captures.

---
*This project was completed as part of the Cyber Security Track (CS) Internship under Future Interns.*
