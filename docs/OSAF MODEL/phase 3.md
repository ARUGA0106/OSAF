# Phase 3: Development – Security Enhanced SDLC (SSDLC)

In the Development Phase, the application’s codebase is implemented, applying security-focused coding standards to guard against vulnerabilities. Incorporating frameworks like OWASP Top 10, SANS/CWE Top 25, and WSTG ensures that secure coding practices, peer reviews, and automated security testing are embedded in the development pipeline.

| S/No | SSDLC Phase | Key Security Objectives                                 | Implementation Item                                 | Code               | Tools & Techniques                                                |
|------|-------------|---------------------------------------------------------|-----------------------------------------------------|--------------------|-------------------------------------------------------------------|
| 1    | Development | Enforce Secure Coding Practices                          | Protect against common risks like SQL injection, XSS, and broken authentication | [OWASP Top 10], [SANS 25] | SAST Tools (e.g., SonarQube, Checkmarx, Fortify), Secure Coding Libraries (e.g., ESAPI for Java, CSRFGuard) |
| 2    | Development | Source Code Review and Peer Review Processes             | Perform manual reviews to catch logical errors or sensitive data exposure | [WSTG], [OWASP Top 10] | Code Review Tools (e.g., GitHub PR, Gerrit, Crucible), Security Checklists for Code Reviews |
| 3    | Development | Security Testing within CI/CD Pipeline                   | Integrate security testing in CI/CD to detect vulnerabilities early | [WSTG], [OWASP Top 10], [SANS 25] | DAST Tools (e.g., OWASP ZAP, Burp Suite), Container Security Scanning (e.g., Aqua Security, Clair) |
| 4    | Development | Input Validation and Output Encoding                     | Mitigate injection and XSS vulnerabilities          | [OWASP Top 10], [SANS 25] | Input Validation Libraries (e.g., Validator.js, Sanitize.js), Web Application Firewall (WAF) |
| 5    | Development | Secure Sensitive Data Handling in Code                   | Store and manage sensitive data securely            | [WSTG], [OWASP Top 10], [SANS 25] | Secrets Management Tools (e.g., HashiCorp Vault, AWS Secrets Manager), Cryptographic Libraries (e.g., bcrypt, AES) |
| 6    | Development | Establish Logging and Monitoring                         | Capture user activities and errors for incident tracking | [OWASP Top 10], [SANS 25] | Logging Libraries (e.g., Log4j, Winston, NLog), SIEM Integration for centralized tracking |
| 7    | Development | Secure Error Handling and Exception Management           | Prevent attackers from gaining insight through errors | [OWASP Top 10], [WSTG] | Error Handling Libraries (e.g., Express.js middleware), Custom Error Messages for end-users |