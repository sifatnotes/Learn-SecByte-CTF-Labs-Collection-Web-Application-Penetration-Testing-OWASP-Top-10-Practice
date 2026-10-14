# Learn-SecByte-CTF-Labs-Collection-Web-Application-Penetration-Testing-OWASP-Top-10-Practice
A curated collection of hands-on web application penetration testing CTF labs covering SQL Injection, XSS, SSRF, Deserialization, SSTI, File Upload to RCE, XXE, Command Injection, LFI/RFI, CSRF, REST/GraphQL API Exploitation, and Business Logic Flaws from Learn SecByte.
# Learn SecByte CTF & Cybersecurity Labs Collection

Welcome to the **Learn SecByte CTF & Cybersecurity Labs Collection**. This repository is a structured, searchable index of hands-on web application security, OWASP Top 10 vulnerability exploitation, modern API security (REST/GraphQL), business logic flaw testing, and remote code execution (RCE) labs designed for cybersecurity students, CTF players, web penetration testers, bug bounty hunters, and application security engineers.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Securing and auditing modern web applications requires a deep technical understanding of server-side vulnerabilities, client-side execution contexts, serialization routines, and API logic. Hosted on [Learn SecByte](https://learn.secbyte.org/), this collection of CTF challenge labs provides comprehensive, practical training across web application security testing.

From discovering classical database injection vectors (SQLi) and client-side script execution (XSS), to abusing server-side template engines (SSTI), weaponizing object deserialization gadget chains, fetching cloud metadata via SSRF, exploiting XML external entities (XXE), uploading webshells, abusing path traversal (LFI/RFI), and targeting REST/GraphQL API logic flaws, these exercises build complete web application penetration testing capabilities.

---

## Lab Collection & Index

Below is the complete, searchable index of all web security, OWASP Top 10, API, and RCE challenges in this collection:

| # | Lab / Challenge Name | Category | Focus / Key Topics | Lab Link |
|---|----------------------|----------|---------------------|----------|
| 1 | **API Siege: REST & GraphQL Modern Exploitation** | API & Business Logic Security | GraphQL introspection, batching attacks, IDOR in REST endpoints, rate limit bypasses | [Access Lab](https://learn.secbyte.org/ctf/api-siege-rest-graphql-modern-exploitation) |
| 2 | **Business Logic Under Pressure** | API & Business Logic Security | Race conditions in payments, parameter pollution, workflow bypasses, negative quantities | [Access Lab](https://learn.secbyte.org/ctf/business-logic-under-pressure) |
| 3 | **Command Injection: OS Command Execution Lab** | Server-Side Vulnerabilities | Shell metacharacter injection, blind OS command injection, out-of-band (OOB) data exfiltration | [Access Lab](https://learn.secbyte.org/ctf/command-injection-os-command-execution-lab) |
| 4 | **Server-Side Template Injection: From Reflection to RCE** | Server-Side Vulnerabilities | Jinja2, Twig, Freemarker SSTI, engine detection, sandbox escapes, remote code execution | [Access Lab](https://learn.secbyte.org/ctf/server-side-template-injection-from-reflection-to-rce) |
| 5 | **Insecure Deserialization: Object Injection & Hidden Gadget Chains** | Server-Side Vulnerabilities | Java/PHP/Python deserialization, YSoSerial gadget chains, magic methods (`__wakeup`, `readObject`), RCE | [Access Lab](https://learn.secbyte.org/ctf/insecure-deserialization-object-injection-hidden-gadget-chai) |
| 6 | **XML Shadows: XXE Injection and XML Security Weaknesses** | Server-Side Vulnerabilities | External entity resolution, out-of-band XXE (OOB-XXE), local file disclosure, SSRF via XML | [Access Lab](https://learn.secbyte.org/ctf/xml-shadows-xxe-injection-and-xml-security-weaknesses) |
| 7 | **SSRF: Cloud Metadata & Hidden Consoles** | Server-Side Vulnerabilities | Server-Side Request Forgery, AWS/GCP/Azure IMDS metadata retrieval, internal network pivot, loopback bypass | [Access Lab](https://learn.secbyte.org/ctf/ssrf-cloud-metadata-hidden-console) |
| 8 | **Traversal, LFI & RFI: Medium Lab** | Input Validation & File Security | Directory traversal (`../`), Local File Inclusion, Remote File Inclusion, PHP wrappers (`php://filter`, `data://`) | [Access Lab](https://learn.secbyte.org/ctf/traversal-lfi-rfi-medium-lab) |
| 9 | **File Upload to RCE: From Innocent Images to Shells** | Input Validation & File Security | MIME type bypass, double extensions, null-byte injection, polyglot web shell execution | [Access Lab](https://learn.secbyte.org/ctf/file-upload-to-rce-from-innocent-images-to-shells) |
| 10 | **CSRF & Session Exploitation: Token Tangle** | Client-Side Security | Cross-Site Request Forgery, SameSite cookie attribute bypass, token leakage, session fixation | [Access Lab](https://learn.secbyte.org/ctf/csrf-session-exploitation-token-tangle) |
| 11 | **XSS Recon to Exploit: Discovery, Payloads & Bypass Techniques** | Client-Side Security | Reflected, Stored, DOM-based XSS, WAF payload obfuscation, CSP bypasses, session hijacking | [Access Lab](https://learn.secbyte.org/ctf/xss-recon-to-exploit-discovery-payloads-bypass-techniques) |
| 12 | **SQL Injection: Fundamentals & Advanced Exploitation** | Database Injection | Union-based, Error-based, Blind Boolean/Time-based SQLi, out-of-band exfiltration, `sqlmap` usage | [Access Lab](https://learn.secbyte.org/ctf/sql-injection-fundamentals-advanced-exploitation) |

---

## Categories

### 1. Database & Server-Side Execution Flaws
Exploit low-level input validation weaknesses on the server, including database injections, OS command execution, and template engine bugs.
- [SQL Injection: Fundamentals & Advanced Exploitation](https://learn.secbyte.org/ctf/sql-injection-fundamentals-advanced-exploitation)
- [Command Injection: OS Command Execution Lab](https://learn.secbyte.org/ctf/command-injection-os-command-execution-lab)
- [Server-Side Template Injection: From Reflection to RCE](https://learn.secbyte.org/ctf/server-side-template-injection-from-reflection-to-rce)

### 2. Advanced Server-Side Injections & Request Forgery
Abuse XML parsers, language object deserialization routines, and server-initiated request vectors to reach cloud metadata and execute code.
- [SSRF: Cloud Metadata & Hidden Consoles](https://learn.secbyte.org/ctf/ssrf-cloud-metadata-hidden-console)
- [XML Shadows: XXE Injection and XML Security Weaknesses](https://learn.secbyte.org/ctf/xml-shadows-xxe-injection-and-xml-security-weaknesses)
- [Insecure Deserialization: Object Injection & Hidden Gadget Chains](https://learn.secbyte.org/ctf/insecure-deserialization-object-injection-hidden-gadget-chai)

### 3. File Security, Traversal & Client-Side Attacks
Bypass file upload restrictions, exploit local/remote file inclusions, execute client-side scripts, and forge cross-site requests.
- [Traversal, LFI & RFI: Medium Lab](https://learn.secbyte.org/ctf/traversal-lfi-rfi-medium-lab)
- [File Upload to RCE: From Innocent Images to Shells](https://learn.secbyte.org/ctf/file-upload-to-rce-from-innocent-images-to-shells)
- [XSS Recon to Exploit: Discovery, Payloads & Bypass Techniques](https://learn.secbyte.org/ctf/xss-recon-to-exploit-discovery-payloads-bypass-techniques)
- [CSRF & Session Exploitation: Token Tangle](https://learn.secbyte.org/ctf/csrf-session-exploitation-token-tangle)

### 4. API Security & Business Logic Flaws
Audit modern REST and GraphQL APIs for authorization flaws and break complex application workflows.
- [API Siege: REST & GraphQL Modern Exploitation](https://learn.secbyte.org/ctf/api-siege-rest-graphql-modern-exploitation)
- [Business Logic Under Pressure](https://learn.secbyte.org/ctf/business-logic-under-pressure)

---

## Learning Path

Follow this structured progression path to master web application security testing and OWASP Top 10 exploitation:

1. **Phase 1: Fundamental Server & Client Attacks** — Master core input validation flaws, client-side script execution, and database injection:
   - [SQL Injection: Fundamentals & Advanced Exploitation](https://learn.secbyte.org/ctf/sql-injection-fundamentals-advanced-exploitation)
   - [XSS Recon to Exploit: Discovery, Payloads & Bypass Techniques](https://learn.secbyte.org/ctf/xss-recon-to-exploit-discovery-payloads-bypass-techniques)
   - [CSRF & Session Exploitation: Token Tangle](https://learn.secbyte.org/ctf/csrf-session-exploitation-token-tangle)

2. **Phase 2: File System & Local Injections** — Leverage file inclusion, directory traversal, and malicious file uploads:
   - [Traversal, LFI & RFI: Medium Lab](https://learn.secbyte.org/ctf/traversal-lfi-rfi-medium-lab)
   - [File Upload to RCE: From Innocent Images to Shells](https://learn.secbyte.org/ctf/file-upload-to-rce-from-innocent-images-to-shells)
   - [Command Injection: OS Command Execution Lab](https://learn.secbyte.org/ctf/command-injection-os-command-execution-lab)

3. **Phase 3: Advanced Server-Side Exploitation** — Trigger template injections, object deserialization, SSRF, and XXE:
   - [Server-Side Template Injection: From Reflection to RCE](https://learn.secbyte.org/ctf/server-side-template-injection-from-reflection-to-rce)
   - [XML Shadows: XXE Injection and XML Security Weaknesses](https://learn.secbyte.org/ctf/xml-shadows-xxe-injection-and-xml-security-weaknesses)
   - [SSRF: Cloud Metadata & Hidden Consoles](https://learn.secbyte.org/ctf/ssrf-cloud-metadata-hidden-console)
   - [Insecure Deserialization: Object Injection & Hidden Gadget Chains](https://learn.secbyte.org/ctf/insecure-deserialization-object-injection-hidden-gadget-chai)

4. **Phase 4: API & Business Logic Vulnerabilities** — Audit REST/GraphQL endpoints and exploit business workflow logic:
   - [API Siege: REST & GraphQL Modern Exploitation](https://learn.secbyte.org/ctf/api-siege-rest-graphql-modern-exploitation)
   - [Business Logic Under Pressure](https://learn.secbyte.org/ctf/business-logic-under-pressure)

---

## How to Use the Labs

1. Select a challenge link from the index or category sections above.
2. Read the scenario requirements and target URL details on [Learn SecByte](https://learn.secbyte.org/).
3. Deploy web security testing frameworks (Burp Suite Pro/Community, OWASP ZAP, `sqlmap`, `ffuf`, Postman, `YSoSerial`) inside an isolated environment.
4. Intercept HTTP requests, construct custom injection payloads, bypass web application firewalls (WAFs), execute remote code, and retrieve challenge flags.

---

## Disclaimer

This repository and its linked resources are strictly designed for educational, threat research, and authorized technical security training purposes. Never test, deploy, or execute web application exploits or automated scanners against unauthorized websites, applications, or production environments.
