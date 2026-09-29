# Server-Side Request Forgery (SSRF) — PortSwigger Web Security Academy

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
The server can be tricked into making requests to unintended internal or external destinations chosen by the attacker.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Allowlist outbound destinations, block internal ranges/metadata endpoints, and don't send raw user-supplied URLs.

## Mapped to
**OWASP:** A10:2021 – Server-Side Request Forgery  ·  **CWE:** CWE-918 (SSRF)
