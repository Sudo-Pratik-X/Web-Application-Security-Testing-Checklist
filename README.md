# 🛡️ Web Application Security Testing Checklist

An interactive, single-file web application designed to track, filter, and document web and API penetration testing checklists. It provides real-time progress calculations and aggregates critical vulnerability vectors into 16 structured, audit-ready categories.

This tool operates completely client-side. No databases, no external network tracking, and zero tracking dependencies—making it perfect for high-security, air-gapped pentesting environments.

---

## 🚀 Features

- **Dynamic Progress Metrics:** Instantly calculates coverage percentages through an interactive linear status bar and radial target ring.
- **Live Fuzzy Filtering:** Type anything from specific flaws (e.g., `JWT`, `SSRF`) to quickly narrow down required actions across sections.
- **Bulk Administration Toggles:** Expand or collapse verification groups instantly, or toggle tracking flags simultaneously based on search views.
- **Session Privacy Safeguards:** Audit status states stay completely locked inside the local running window session. Reloading or clearing the window safely wipes volatile session footprints.

---

## 🗂️ Checklist Architecture

The testing workbench is structurally broken down into the following core application layers:

1. **Network, TLS & Server Config** — Transport level flaws, cipher validation, host injection, and security header enforcement.
2. **Information Disclosure & Recon** — Leakage of PII, administrative route exposures, source map forensics, and endpoint maps.
3. **CORS, Smuggling & Redirects** — Cross-Origin request validation, HTTP request smuggling vectors, and open forwarding.
4. **Authentication & Login** — Credential enumeration mitigation, cryptographic injection on login portals, and brute force protection.
5. **Password Reset Flow** — Reset token predictability, lifecycle validation, and host spoofing injection.
6. **Session Management** — Replay mitigation, absolute/idle tracking, token rotation protocols, and isolation boundaries.
7. **Cookies** — Security attributes validation (`HttpOnly`, `Secure`, `SameSite`) and token scoping.
8. **OTP & MFA** — Multi-factor authorization rate limiting, bypass pathways, and session boundary validations.
9. **JWT & Tokens** — Verification mechanisms, algorithm downgrade mitigation (`alg=none`), secrets validation, and token lifetime checks.
10. **IDOR & Access Control** — Object/Function level validation mappings (BOLA/BFLA), privilege escalation, and lateral traverse paths.
11. **Injection Vulnerabilities** — SQLi variants, XSS vectors, template injections (SSTI), command lines, XXE, and server-side requests (SSRF).
12. **API Security** — Schema mutation, method tampering, rate-limit boundaries, and unauthenticated endpoints.
13. **CSRF** — Countermeasure coverage and implementation bypass variants.
14. **Business Logic & Payments** — Numeric parameter manipulation, order logic alteration, multi-step workflow bypasses, and state corruption.
15. **File Upload** — Extension manipulation, magic byte circumventions, web shell execution vectors, and archive unpacking vulnerabilities.
16. **OAuth** — Callback URI verification leaks, integration flow vulnerabilities, and structural state forgery validation.

---

## 🛠️ Quick Start

### Local Setup
Since this tool relies entirely on native browser features, there is no installation or build compilation required:

1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/web-security-checklist.git](https://github.com/yourusername/web-security-checklist.git)
