# Access Control & IDOR — PortSwigger Web Security Academy

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
Missing or broken authorization lets a user reach another user's data or admin functions, often via predictable object IDs (IDOR).

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Enforce server-side authorization on every request; use non-guessable references; deny by default.

## Mapped to
**OWASP:** A01:2021 – Broken Access Control  ·  **CWE:** CWE-639 / CWE-284 (Authorization Bypass / Improper Access Control)
