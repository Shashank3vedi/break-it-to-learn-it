# Brute Force — DVWA

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
The login form has no rate-limiting, lockout, or CAPTCHA, so credentials can be guessed by automated repeated attempts.

## Find it
_TODO — add how you spotted it in the lab (the parameter / page / behaviour)._

## Break it (lab)
_TODO — add your step-by-step exploitation and the payloads you used, with screenshots._

## Fix it
Add rate-limiting and account lockout, enforce strong passwords + MFA, and add CAPTCHA after failed attempts.

## Mapped to
**OWASP:** A07:2021 – Identification & Authentication Failures  ·  **CWE:** CWE-307 (Improper Restriction of Excessive Authentication Attempts)
