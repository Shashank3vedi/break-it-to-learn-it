# File Inclusion (LFI / RFI) — DVWA

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
The app includes a file based on user input, allowing local (LFI) or remote (RFI) files to be loaded and sometimes executed.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Allowlist includable files, never build include paths from user input, and disable remote URL includes.

## Mapped to
**OWASP:** A03:2021 – Injection  ·  **CWE:** CWE-98 / CWE-22 (File Inclusion / Path Traversal)
