# File Upload — DVWA

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
Uploads aren't properly validated, so an attacker can upload a web shell and get code execution on the server.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Validate real file type/content (not just extension), store uploads outside the web root, rename files, and disable execution in the upload dir.

## Mapped to
**OWASP:** A05:2021 – Security Misconfiguration  ·  **CWE:** CWE-434 (Unrestricted Upload of File with Dangerous Type)
