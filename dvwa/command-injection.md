# Command Injection — DVWA

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
User input is passed into an OS shell command without sanitisation, letting an attacker run arbitrary system commands.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Avoid shell calls; use language-native/parameterised APIs, allowlist expected values, and never pass raw input to a shell.

## Mapped to
**OWASP:** A03:2021 – Injection  ·  **CWE:** CWE-78 (OS Command Injection)
