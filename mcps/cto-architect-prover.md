# CTO Architect Prover MCP Server

An AI proposed Kubernetes for 50 users, says 'use HTTPS' as a security strategy, and plans database migrations during maintenance windows. That is not architecture — that is Resume-Driven Development. This tool forces five CTO-level architectural axes: stack fitness, failure tolerance, security hardening, migration safety, and observability.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cto-architect-prover)

## Overview
**Category:** architecture
**Tools Count:** 1

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


## Available Tools
- **validate_cto_architect**: Think like a senior CTO who has been paged at 3 AM — not how the system works when everything is fine, but how it behaves when things BREAK. You must: (1) justify STACK FITNESS — match technology complexity to team size, budget, stage, and timeline. A 3-person seed team does not need Kubernetes. A monolith handles 10K concurrent users. Justify AGAINST constraints — "we chose React and Node" is not justification, (2) prove FAILURE TOLERANCE — name every redundancy mechanism, failover path, and circuit breaker. For each component (database, cache, queue, API gateway, external services): what happens when it crashes? How long until recovery? What is the blast radius? "Should work fine" is not tolerance — design for the CRASH, (3) harden SECURITY POSTURE — name specific controls with thresholds, not categories. Rate limiting: X req/min per IP. Auth: token type, algorithm, rotation schedule. Queries: parameterized via ORM, no string concatenation. CORS: whitelist, not wildcard. Encryption: algorithm, key rotation, scope. "We use HTTPS" is not hardening, (4) define MIGRATION SAFETY — expand/contract pattern, parallel writes during transition, API versioning (/v2 alongside /v1), deterministic rollback tested in staging. "Maintenance window" is blocked — zero-downtime ONLY, (5) prove OBSERVABILITY — health probes (/health/live, /health/ready), metric dashboards with alert thresholds (p99 latency, error rate, saturation), log aggregation with search, and specific RTO/RPO targets with tested recovery procedures. "Check the logs" and "we will monitor" are not observability. If rejected, your architecture has a production-critical gap.

Structured reflection tool for senior CTO-level production architecture validation. Forces the agent to justify stack fitness against constraints, prove failure tolerance with specific redundancy mechanisms, harden security with named controls and thresholds, define zero-downtime migration strategies, and prove observability with health probes and RTO/RPO targets. Catches Resume-Driven Development (Kubernetes for 50 users, microservices for a 3-person team — technology chosen for the resume, not the problem), Single Points of Failure ("should work fine" without naming redundancy for database, cache, load balancer, and external dependencies), Security Theater ("we use HTTPS and encryption" without rate limiting thresholds, token rotation, parameterized queries, CORS whitelist, and encryption algorithm specifics), Migration Amnesia ("we will migrate carefully" without expand/contract pattern, parallel writes, API versioning, or deterministic rollback — table locks in production are blocked), and Observability Voids ("we monitor the system" without health probes, metric dashboards, alert thresholds, log aggregation, or RTO/RPO targets — SSH to check logs is not monitoring). Call once per architecture decision or system design review


## Installation & Usage

To install and use the **CTO Architect Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cto-architect-prover](https://vinkius.com/mcp/cto-architect-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
