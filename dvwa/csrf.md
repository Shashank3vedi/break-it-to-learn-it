# Cross-Site Request Forgery (CSRF) — DVWA

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
State-changing actions (like changing a password) lack an anti-CSRF token, so a forged cross-site request can act as the logged-in victim.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Use per-request anti-CSRF tokens, set SameSite cookies, and require re-authentication for sensitive changes.

## Mapped to
**OWASP:** A01:2021 – Broken Access Control  ·  **CWE:** CWE-352 (Cross-Site Request Forgery)
