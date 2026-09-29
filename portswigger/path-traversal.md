# Path Traversal — PortSwigger Web Security Academy

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
User input reaches a filesystem path, so sequences like ../ let an attacker read files outside the intended directory.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Canonicalise and validate paths, allowlist filenames, and never build file paths from raw user input.

## Mapped to
**OWASP:** A01:2021 – Broken Access Control  ·  **CWE:** CWE-22 (Path Traversal)
