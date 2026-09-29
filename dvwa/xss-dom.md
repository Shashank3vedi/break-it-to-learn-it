# DOM-based XSS — DVWA

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
Client-side JavaScript writes untrusted data into a dangerous DOM sink, so the injection happens entirely in the browser.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Use safe DOM APIs (textContent, not innerHTML), avoid eval/document.write with untrusted data, and apply CSP.

## Mapped to
**OWASP:** A03:2021 – Injection  ·  **CWE:** CWE-79 (Cross-Site Scripting)
