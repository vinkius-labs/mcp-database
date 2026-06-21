# Requirement Decomposition Prover MCP Server

AI generates the happy path but omits error handling, edge cases, security, and observability — the '80% Problem'. This tool forces complete requirement decomposition BEFORE code generation: specify inputs/outputs, map failure modes, cover boundary conditions, validate OWASP, plan logging.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/requirement-decomposition-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
AI agents are excellent at generating the visible 80% of a feature. The CRUD endpoint works. The form submits. The API returns data. But the critical 20% is missing: what happens when the network fails? When the input is empty? When concurrent users hit the same resource? When the attacker sends a malformed payload? When production breaks at 3am and there are no logs?

### The Problem It Solves

The '80% Problem' (documented by Augment Code, 2025): AI delivers visible features but systematically omits non-functional requirements. This creates code that works in demos and breaks in production.

- **Error states missing** — The happy path is defined. The failure modes are not. Network errors, database timeouts, malformed input, auth failures, race conditions — none are mapped.
- **Edge cases ignored** — Empty arrays, null values, maximum string lengths, concurrent access, timezone boundaries, unicode characters, zero-value amounts, negative numbers. The boundaries where bugs live.
- **Security unvalidated** — Input validation missing. SQL injection paths open. XSS vectors unprotected. Auth checks incomplete. The AI wrote functional code. An attacker will write the exploit.
- **Observability absent** — No structured logging. No error tracking. No performance metrics. No distributed tracing. If you can't see it, you can't fix it. When production breaks, you're blind.

### How It Works

Requirement Decomposition Prover uses 5 Decision Pivots that force COMPLETE specification before any code is generated:

1. **happyPathDefined** — Core functionality specified with exact inputs, outputs, state transitions, and success criteria.
2. **errorStatesMapped** — Every failure mode identified: network, database, input, auth, timeout, race conditions. Each with recovery strategy.
3. **edgeCasesCovered** — Boundary conditions handled: empty, null, max, concurrent, timezone, unicode, zero, negative, large datasets.
4. **securityValidated** — OWASP Top 10 checklist: injection, broken auth, XSS, misconfiguration. Every input is untrusted.
5. **observabilityPlanned** — Structured logging (not console.log), error tracking, performance metrics, distributed tracing.

The engine catches dismissive patterns: 'errors unlikely', 'assume valid input', 'security not needed', 'internal only'. These are the sentences that precede production incidents.

### Why It Works

- **Pre-generation, not post-generation** — Forces completeness BEFORE code exists, when changes are free. Not after, when they're expensive.
- **13 consistency rules** catch vague requirements, dismissed error states, ignored security, and absent observability.
- **Grounded in IEEE 830 (requirement specification), INVEST criteria (Bill Wake), OWASP Top 10, Twelve-Factor App, and SRE principles.**
- **Eliminates retrofitting costs** — The 80% Problem means the missing 20% often costs MORE to add later than writing the feature from scratch.


## Available Tools
- **validate_requirement_decomposition**: This eliminates the 80% Problem. You must: (1) HAPPY PATH — define exact inputs, outputs, state transitions, and success criteria. "Should work" is not a spec. Specific values, specific types, specific responses, (2) ERROR STATES — for EVERY external dependency: what if it is slow? Down? Returns garbage? For every user input: what if it is malformed? Missing? Hostile? Each error state requires: detection, user response, recovery, alerting, (3) EDGE CASES — empty, null, max-length, unicode, emoji, zero, negative, concurrent access, timezone boundaries, DST transitions, leap years. If a field accepts strings, test the full Unicode range, (4) SECURITY — every input is untrusted. OWASP Top 10 for every endpoint. Password hashing from Day 1. Rate limiting from Day 1. Input validation is a REQUIREMENT, (5) OBSERVABILITY — structured logging (not console.log), metrics (latency, throughput, error rate), alerting (threshold-based), distributed tracing for async flows. If you cannot measure it in production, you cannot fix it in production. If rejected, decompose further before writing any code.

Structured reflection tool that forces COMPLETE requirement decomposition before code generation — eliminates the "80% Problem" where AI delivers the happy path but omits error handling, edge cases, security, and observability. Based on IEEE 830 requirements specification, Gause & Weinberg "Exploring Requirements" (1989), and the "Swiss Cheese Model" of failure prevention. Catches Happy-Path-Only (building the success case and ignoring every failure mode — "Build a user registration endpoint." Happy path: POST /register with name, email, password → create user → return 201. Shipped. Then: Week 1: 400 users register with "password123" — no strength validation. Account takeovers begin. Week 2: someone registers with the same email twice — duplicate users, login resolves to first-created user, second user cannot access their data. Week 3: bot registers 50,000 accounts in 12 hours — no rate limiting. Database grows 4GB. Week 4: user registers with email "admin@company.com" — no email verification. They reset the admin password and access the admin panel. Every one of these was predictable. Every one was in the requirements — just unwritten. The "80% Problem": the happy path IS 80% of the code. The other 20% is 80% of the bugs), Error Amnesia (no systematic mapping of what goes wrong — "What if the database is down?" "That won't happen." AWS RDS has 99.95% uptime SLA — which means 4.38 hours of downtime PER YEAR. If registration handles 200 requests/hour, that is 876 failed registrations per year. Each failed registration with no error handling: user sees a 500 error with a stack trace (information disclosure — CWE-209), retries 3 times (tripling the load on a struggling DB), then abandons. Recovery: nothing — no retry queue, no graceful degradation, no user notification. Systematic error mapping: for EVERY external dependency (database, email service, payment gateway, third-party API), answer: what happens when it is slow (>2s)? Unavailable? Returns garbage? Each answer requires: detection method, user-facing response, retry strategy, alerting), Edge-Case Ignorance (not testing boundary conditions that WILL occur in production — The registration form accepts "name" as a string. What is tested: name="John Smith." What is NOT tested: Empty string: name="" — does validation catch it? What error message? Maximum length: name="A" × 10,000 characters — does the DB column handle it? Denial of service? Unicode: name="José María García-López" — does the system handle accented characters? RTL: name="محمد" — does the UI render correctly? Does search work? Emoji: name="Alex 🚀 Smith" — does the DB column support utf8mb4? Script injection: name="<script>alert(1)</script>" — XSS? SQL injection: name="'; DROP TABLE users; --" — is input parameterized? Null byte: name="John\x00Smith" — does the application truncate at null? Every field. Every input. Every boundary. If you only test "John Smith," you only support "John Smith"), Security-as-Afterthought (treating security as a phase, not a requirement — "We will add security later." The registration endpoint stores passwords in plain text: users.password = request.password. "We will add hashing in the security sprint." Before the security sprint: database backup is stolen from an unsecured S3 bucket. 50,000 passwords in plain text. Users reuse passwords — their bank accounts, email, and social media are now compromised. Cost: $150 per record (IBM Cost of a Data Breach 2024) = $7.5M liability. Plus mandatory breach notification (GDPR Article 33: 72 hours). Security requirements must be defined WITH functional requirements — not after. OWASP Top 10 is not optional. Input validation is not a feature — it is a requirement), and Observability Void (shipping code with no visibility into production behavior — "The registration endpoint is slow." How slow? For whom? Since when? Without observability: "We don't know." console.log("user registered") tells you: nothing useful. No timestamp, no user ID, no latency, no success/failure, no request ID for correlation. Structured logging: logger.info("user_registered", {user_id: "uuid", latency_ms: 142, email_sent: true, source: "web", ip_country: "US"}) — queryable, alertable, traceable. Metrics: registration_count (rate), registration_latency_p95 (performance), registration_failure_rate (reliability). Alert: if failure_rate > 5% for 5 minutes → PagerDuty. Without observability, every production issue starts with: "Let me add some logs and redeploy"). Call once per feature before writing any code


## Installation & Usage

To install and use the **Requirement Decomposition Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/requirement-decomposition-prover](https://vinkius.com/mcp/requirement-decomposition-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
