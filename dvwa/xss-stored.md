# Stored XSS — DVWA

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
Malicious script is saved by the app (e.g. in a comment/guestbook) and then served to every user who views it.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Encode on output, validate/sanitise on input, and enforce CSP; treat all stored data as untrusted.

## Mapped to
**OWASP:** A03:2021 – Injection  ·  **CWE:** CWE-79 (Cross-Site Scripting)
