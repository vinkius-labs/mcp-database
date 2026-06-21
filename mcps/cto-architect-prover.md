# CTO Architect Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cto-architect-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

An AI proposed Kubernetes for 50 users, says 'use HTTPS' as a security strategy, and plans database migrations during maintenance windows. That is not architecture — that is Resume-Driven Development. This tool forces five CTO-level architectural axes: stack fitness, failure tolerance, security hardening, migration safety, and observability.

## Description
## The Problem

Ask an LLM to design a production architecture. It will propose Kubernetes, Kafka, and microservices for a 3-person seed team. It will say "use HTTPS" as the entire security strategy. It will plan database migrations during "scheduled maintenance windows." And it will skip observability entirely.

Every LLM commits five architectural reasoning failures:
1. **Resume-Driven Development** — proposes overcomplex tech stacks that no small team can operate.
2. **SPOF Blindness** — designs happy-path architectures without redundancy or failover.
3. **Security Theater** — says "use HTTPS" and "passwords are hashed" without depth.
4. **Migration Amnesia** — plans schema changes that lock tables or require downtime.
5. **Observability Void** — skips health probes, metrics, alerting, and DR targets.

## How It Works

The CTO Architect Prover forces the LLM to fill 5 reflection fields and commit to 5 Decision Pivots before concluding any architecture is production-ready.

### The 5 Architectural Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Stack Fitness** | Justified | Match tech to team size, budget, and stage. |
| **Failure Tolerance** | Tolerated | Name every redundancy mechanism and failover path. |
| **Security Posture** | Hardened | Specific controls with thresholds — not "use HTTPS." |
| **Migration Safety** | Safe | Zero-downtime: expand/contract, parallel writes, rollback. |
| **Observability** | Proven | Health probes, metrics, alerting, specific RTO/RPO. |

### The Verdict Matrix

```
Axis 1 fails → OVER_ENGINEERED
Axis 2 fails → SPOF_DETECTED
Axis 3 fails → SECURITY_VULNERABLE
Axis 4 fails → MIGRATION_BLOCKED
Axis 5 fails → OBSERVABILITY_VOID
All pass     → ARCHITECTURE_PROVEN
```

## Why It Works

Tool calls are obligations. The LLM cannot skip security controls or ignore migration strategies. It must justify the stack against constraints, name specific redundancy mechanisms, define security thresholds, describe zero-downtime migration procedures, and set RTO/RPO targets with numbers. Every rejection names the exact architectural axis that failed.


## Available Tools (1)
- **validate_cto_architect**: Think like a senior CTO who has been paged at 3 AM — not how the system works when everything is fine, but how it behaves when things BREAK. You must: (1) justify STACK FITNESS — match technology complexity to team size, budget, stage, and timeline. A 3-person seed team does not need Kubernetes. A monolith handles 10K concurrent users. Justify AGAINST constraints — "we chose React and Node" is not justification, (2) prove FAILURE TOLERANCE — name every redundancy mechanism, failover path, and circuit breaker. For each component (database, cache, queue, API gateway, external services): what happens when it crashes? How long until recovery? What is the blast radius? "Should work fine" is not tolerance — design for the CRASH, (3) harden SECURITY POSTURE — name specific controls with thresholds, not categories. Rate limiting: X req/min per IP. Auth: token type, algorithm, rotation schedule. Queries: parameterized via ORM, no string concatenation. CORS: whitelist, not wildcard. Encryption: algorithm, key rotation, scope. "We use HTTPS" is not hardening, (4) define MIGRATION SAFETY — expand/contract pattern, parallel writes during transition, API versioning (/v2 alongside /v1), deterministic rollback tested in staging. "Maintenance window" is blocked — zero-downtime ONLY, (5) prove OBSERVABILITY — health probes (/health/live, /health/ready), metric dashboards with alert thresholds (p99 latency, error rate, saturation), log aggregation with search, and specific RTO/RPO targets with tested recovery procedures. "Check the logs" and "we will monitor" are not observability. If rejected, your architecture has a production-critical gap.

Structured reflection tool for senior CTO-level production architecture validation. Forces the agent to justify stack fitness against constraints, prove failure tolerance with specific redundancy mechanisms, harden security with named controls and thresholds, define zero-downtime migration strategies, and prove observability with health probes and RTO/RPO targets. Catches Resume-Driven Development (Kubernetes for 50 users, microservices for a 3-person team — technology chosen for the resume, not the problem), Single Points of Failure ("should work fine" without naming redundancy for database, cache, load balancer, and external dependencies), Security Theater ("we use HTTPS and encryption" without rate limiting thresholds, token rotation, parameterized queries, CORS whitelist, and encryption algorithm specifics), Migration Amnesia ("we will migrate carefully" without expand/contract pattern, parallel writes, API versioning, or deterministic rollback — table locks in production are blocked), and Observability Voids ("we monitor the system" without health probes, metric dashboards, alert thresholds, log aggregation, or RTO/RPO targets — SSH to check logs is not monitoring). Call once per architecture decision or system design review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CTO Architect Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We will build our SaaS with Kubernetes, Kafka for event streaming, and 8 microservices. We have a team of 3 developers and launch in 6 weeks. Security: we use HTTPS."

**🤖 AI Agent:**
> OVER_ENGINEERED + SECURITY_VULNERABLE — Two fatal gaps. First: Kubernetes, Kafka, and 8 microservices for a 3-person team launching in 6 weeks is Resume-Driven Development. A Node.js monolith with PostgreSQL ships in 6 weeks. Kubernetes adds 3 months of operational overhead. Second: 'use HTTPS' is not a security strategy — name rate limiting thresholds, auth token type, parameterized queries, and encryption algorithm.

---

**👤 You:**
> "Node.js monolith, 4-person team, $800/mo infra. PostgreSQL streaming replica (async, <1s lag). Redis Sentinel for cache. ALB with 10s health checks. Circuit breaker on Stripe (5s timeout, 3 retries). Rate limiting: 100/min per IP. JWT RS256, 15min access, 7-day refresh. Parameterized via Prisma. CORS whitelist. AES-256 on PII. Expand/contract migrations: dual-write, backfill, switch, drop. API v2 alongside v1. Rollback tested in staging. Health: /health/live, /health/ready. Prometheus + Grafana, p99 < 200ms alert. RTO < 4h, RPO < 1h, daily S3 backups, tested quarterly."

**🤖 AI Agent:**
> ARCHITECTURE_PROVEN — CTO-level architecture validated. Stack: Node.js monolith right-sized for 4-person team at $800/mo. Failure tolerance: PostgreSQL replica, Redis Sentinel, ALB, circuit breaker on Stripe. Security: rate limiting 100/min, JWT RS256 with rotation, parameterized Prisma, CORS whitelist, AES-256. Migration: expand/contract with tested rollback. Observability: health probes, Prometheus with p99 alerting, RTO < 4h, RPO < 1h. Production-ready.

---

**👤 You:**
> "We need to migrate our user table to add a new column for subscription tier. We will take the system offline for 2 hours on Saturday night, run ALTER TABLE, and deploy the new code. We will check the logs manually after to make sure everything works."

**🤖 AI Agent:**
> MIGRATION_BLOCKED + OBSERVABILITY_VOID — Two fatal gaps. First: 'take the system offline for 2 hours' is a maintenance window — blocked. Use expand/contract: add the column with a default value (no lock), dual-write from the application, backfill existing rows in batches, switch reads, drop the old logic. Each step handles live traffic. Second: 'check the logs manually' is not monitoring — define automated health probes and alerting thresholds.


## ❓ FAQ

**Q: What is 'Resume-Driven Development'?**
It is when engineers choose technologies because they look impressive on a resume, not because they solve the problem. Kubernetes for a 3-person seed team with 50 users is Resume-Driven Development. A monolith with PostgreSQL would ship in 8 weeks. Kubernetes adds 3 months of operational overhead for no user benefit.

**Q: Why does it reject 'use HTTPS' as a security strategy?**
Because HTTPS is the bare minimum, not a strategy. A hardened security posture requires rate limiting with specific thresholds (100 req/min per IP), parameterized queries to prevent SQL injection, JWT with RS256 and rotation policy, CORS whitelisting, and data-at-rest encryption with a named algorithm (AES-256). Saying 'use HTTPS' is like saying 'lock the door' — it does not address the windows.

**Q: Why is 'maintenance window' blocked?**
Because zero-downtime is the production standard. Maintenance windows are an admission that your migration strategy cannot handle live traffic. Use the expand/contract pattern: add the new column, dual-write, backfill, switch reads, drop the old column. Each step is reversible. Each step handles live traffic. If your migration requires downtime, your architecture is not production-ready.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cto-architect-prover](https://vinkius.com/mcp/cto-architect-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CTO Architect Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cto-architect-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CTO Architect Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cto-architect-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
