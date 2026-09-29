# Reflected XSS — DVWA

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
Unsanitised input is reflected straight back in the response, so a crafted link executes script in the victim's browser.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Context-aware output encoding, input validation, and a strong Content-Security-Policy.

## Mapped to
**OWASP:** A03:2021 – Injection  ·  **CWE:** CWE-79 (Cross-Site Scripting)
