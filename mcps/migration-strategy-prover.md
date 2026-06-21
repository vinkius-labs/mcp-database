# Migration Strategy Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/migration-strategy-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/migration-strategy-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/migration-strategy-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops](../categories/devops.md)

An AI recommended a big-bang database migration over the weekend. No dependency map — 7 services read from that database. No rollback plan — 'just restore from backup.' No data validation — 2.3 million records with timezone-dependent timestamps. The migration ran Saturday at 2 AM. By 4 AM, 3 downstream services were returning stale data, the backup was 6 hours old, and 14,000 customer records had corrupted timestamps. Monday morning: 72-hour incident. This tool forces risk assessment, rollback definition, data integrity verification, cutover planning, and stakeholder alignment.

## Description
AI agents recommend migrations without mapping what breaks. They skip rollback planning. They assume data consistency. They propose big-bang cutovers. They forget 12 teams depend on the system.

### The Problem

LLMs commit five migration failures that cause multi-day incidents:

- **Risk Unassessed** — 'Straightforward migration, no major risks.' No dependency map. No blast radius analysis. 7 services read from that database, 3 teams write to it, and the billing pipeline runs a nightly job against it. None of this was documented.
- **Rollback Undefined** — 'We can always restore from backup.' The backup is 6 hours old. The migration wrote 340,000 records during the window. Those records are gone. 'Just switch back' is not a rollback plan when data has been mutated.
- **Data Integrity Unproven** — 'Data migrates cleanly.' No row count comparison. No checksum verification. No referential integrity check. 14,000 records have timezone-corrupted timestamps because the source was UTC and the destination was America/New_York.
- **Cutover Missing** — 'Big bang over the weekend.' No traffic shifting. No canary percentage. No monitoring at each stage. No go/no-go criteria. The switch happened at 2 AM and the first alert fired at 4 AM — 2 hours of silent corruption.
- **Stakeholders Unaligned** — 'Everyone knows about the migration.' The support team found out Monday morning from customer tickets. The on-call engineer was not added to the escalation channel. The runbook was in someone's personal Notion.

### How It Works

5 Decision Pivots:

1. **riskAssessed** — Dependencies mapped, blast radius documented, failure scenarios enumerated, data volume quantified, timeline realistic.
2. **rollbackDefined** — Trigger metrics specified, step-by-step procedure written, timeline estimated, mutated data handling planned.
3. **dataIntegrityProven** — Row counts, checksums, referential integrity, edge cases (NULLs, unicode, timezones, precision).
4. **cutoverPlanned** — Strategy chosen (Strangler Fig/Blue-Green/Canary), traffic shifting percentages, monitoring at each stage, go/no-go gates.
5. **stakeholdersAligned** — All affected teams listed, customer notification if needed, shared timeline, escalation paths, published runbook.

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| riskAssessed = false | RISK_UNASSESSED | No dependency map. No blast radius. |
| rollbackDefined = false | ROLLBACK_UNDEFINED | 'Just switch back' is not a plan. |
| dataIntegrityProven = false | DATA_INTEGRITY_UNPROVEN | Assumed consistency. No validation. |
| cutoverPlanned = false | CUTOVER_MISSING | Big bang. No monitoring. No gates. |
| stakeholdersAligned = false | STAKEHOLDERS_UNALIGNED | Support found out from customer tickets. |
| All pivots pass | MIGRATION_PROVEN | Mapped, planned, verified, monitored, communicated. |

### Why It Works

- **Tool calls are obligations.** The agent cannot recommend a migration without mapping dependencies, defining rollback triggers, specifying data validation criteria, and listing affected teams.
- **Consistency engine catches contradictions.** If the agent claims `rollbackDefined=true` but says 'restore from backup,' the engine rejects with specific rollback procedure coaching.
- **Semantic traps detect hand-waving.** 'No major risks,' 'just switch back,' 'data will be consistent,' 'big bang cutover,' and 'everyone knows' trigger automatic rejection.


## Available Tools
- **validate_migration_strategy**: You must: (1) INVENTORY RISKS — map every dependency, blast radius, and failure scenario. Include data volume, transformation complexity, timeline with buffer. "Straightforward migration" is never an assessment, (2) DEFINE ROLLBACK — specify trigger metrics (error rate >X%, latency >Yms, data lag >Z min), step-by-step procedure, data reconciliation plan, and whether rollback is reversible. "Just switch back" is not rollback, (3) PROVE DATA INTEGRITY — row counts, checksums, referential integrity, edge cases (NULLs, Unicode, timezones, precision). If you did not verify it, it is not verified, (4) PLAN CUTOVER — incremental traffic shifting with monitoring at each stage. Strangler Fig / Blue-Green / Canary / Big-Bang with go/no-go criteria. "Over the weekend" is not a strategy, (5) ALIGN STAKEHOLDERS — upstream producers, downstream consumers, on-call teams, customer notification, shared runbook, escalation path. "Everyone knows" is never alignment. If rejected, fix the specific migration gap before executing.

Structured reflection tool for system migration strategy — forces comprehensive risk inventory, trigger-based rollback planning, data integrity verification, incremental cutover design, and stakeholder alignment before any migration executes. Catches Risk Unassessed (starting a migration without mapping blast radius — a team migrated a PostgreSQL 12 database to PostgreSQL 16 on a Saturday. They tested the migration on a staging database with 50,000 rows. Production had 340 million rows. The migration took 47 hours instead of the estimated 4. During migration, 3 downstream services that polled the database every 30 seconds began queueing requests — by hour 8, the message queue had 2.4 million unprocessed events. The blast radius included: the billing system (invoices frozen), the notification service (800,000 queued emails), and the analytics pipeline (48-hour data gap). "No major risks" is never an assessment — every migration has dependencies you have not found yet), Rollback Undefined (having no rollback plan or defining "just switch back" — a monolith-to-microservices migration cut over 3 services on Monday. By Wednesday, the new payment service had processed $2.3M in transactions. A critical bug was discovered Thursday. "Roll back" meant: reconcile $2.3M in transactions written to the new database schema that the old schema cannot read. 47 hours of manual reconciliation by 6 engineers. Rollback must define: trigger metrics (error rate >X%, latency >Yms), exact procedure (not "switch back"), data reconciliation for the transition period, and whether rollback is even possible — some migrations are one-way), Data Integrity Unproven (migrating data without verification beyond "it looks right" — a cloud migration moved 89 million user records. Post-migration count matched. Two weeks later: 340,000 records had truncated Unicode characters in names (Turkish İ → I, German ß → ss, Japanese characters → ?). Row count verification alone is insufficient. Checksums catch bit-level corruption. Referential integrity checks catch broken FK relationships. Edge case testing catches encoding, timezone, NULL handling, and precision loss. If you did not verify it, it is not verified), Cutover Missing (planning a "big bang over the weekend" instead of incremental traffic shifting — big bang migrations have a binary outcome: success or total failure with no middle ground. A Strangler Fig pattern routes 1% → 5% → 25% → 50% → 100% of traffic, with monitoring and go/no-go criteria at each stage. Blue-Green gives instant rollback by switching load balancer targets. Canary catches issues at 1% traffic before they affect 100% of users. The cutover strategy IS the risk mitigation), and Stakeholders Unaligned (migrating without telling downstream teams — a database migration changed column types from VARCHAR(255) to TEXT. The analytics team's ETL pipeline had VARCHAR(255) constraints hardcoded. Pipeline broke silently — 3 days of missing analytics data before anyone noticed. Every migration has upstream producers and downstream consumers. Each must be identified by name, notified with timeline, and given a shared runbook). Call once per migration plan before execution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Migration Strategy Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We need to migrate our PostgreSQL database from AWS RDS to Google Cloud SQL. It should be straightforward — just dump and restore. We can do it over the weekend during low traffic."

**🤖 AI Agent:**
> RISK_UNASSESSED — 'Straightforward' and 'just dump and restore' are not risk assessments. Questions you have not answered: How many services query this database? What are the connection string dependencies? Do any use RDS-specific features (IAM auth, pg_cron, RDS Proxy)? What is the data volume? How long does the dump take? What about in-flight transactions during dump? Network latency difference between AWS and GCP for dependent services? Map every dependency before planning the migration.

---

**👤 You:**
> "Risk: 7 services read (auth, billing, analytics, notifications, reporting, API gateway, admin panel). 2 services write (API gateway, billing). RDS-specific: pg_cron for 3 nightly jobs, RDS Proxy for connection pooling, IAM auth for 2 services. Data: 48GB, 142M rows, 23 tables, 47 foreign keys. Estimated dump: 35 min. Failure scenarios: (1) connection string misconfiguration — 40%, (2) pg_cron jobs not migrated — 30%, (3) timezone mismatch in timestamp columns — 20%. Timeline: 2 sprints including testing. Rollback: trigger at error rate >0.5% or p99 >500ms on any dependent service. Procedure: (1) stop writes to new DB, (2) re-point connection strings to old RDS via env vars — 3 min per service, (3) replay any writes from new→old via change capture log, (4) disable Cloud SQL. Duration: 25 minutes. One-way risk: none, old RDS stays warm for 7 days post-cutover. Data: row counts per table, MD5 checksums on id+updated_at for all 142M rows, FK validation script, timezone verification (all UTC). Dual-write window: 48 hours before cutover comparing writes. Edge cases: NULL handling in 3 columns, unicode in user.name, timestamp precision (microseconds vs milliseconds). Cutover: Blue-Green with pgbouncer. Phase 1: read replica on Cloud SQL, 10% read traffic, monitor for 24h. Phase 2: 50% reads, monitor 24h. Phase 3: 100% reads, monitor 48h. Phase 4: write cutover with 2-minute maintenance window, dual-write for 1h, then old RDS read-only. Go/no-go: error rate <0.1%, latency delta <50ms, zero data discrepancy in dual-write. Stakeholders: Platform team (owns migration), API team (connection strings), Billing team (write path), Analytics (nightly jobs), Support (customer notification if >2min downtime), On-call SRE (added to #migration-war-room). Runbook in Confluence, reviewed by all leads. Go/no-go decision: VP Engineering."

**🤖 AI Agent:**
> MIGRATION_PROVEN — Production-grade migration strategy validated. Risk: 7 readers + 2 writers mapped with RDS-specific dependencies (pg_cron, RDS Proxy, IAM auth). Rollback: trigger at 0.5% error / 500ms p99, 25-min procedure, old RDS warm for 7 days. Data: 142M row checksums, FK validation, dual-write comparison, timezone/unicode/precision edge cases. Cutover: Blue-Green via pgbouncer, 4-phase with 24-48h monitoring at each, 2-min write window, go/no-go at <0.1% error + <50ms delta. Stakeholders: 6 teams in war room, Confluence runbook reviewed, VP Engineering go/no-go. This migration survives a Saturday 2 AM failure.

---

**👤 You:**
> "Risk: Migrating monolith to 5 microservices. Dependencies: database shared by all modules, 3 third-party integrations, message queue. Blast radius: all customer-facing features. Timeline: 3 months. Rollback: if something goes wrong, we can always roll back to the monolith. Data: we will validate after the migration is complete."

**🤖 AI Agent:**
> ROLLBACK_UNDEFINED — Risk assessment passes (dependencies mapped, blast radius identified). But rollback fails: 'we can always roll back to the monolith' is not a plan. When you extract 5 services, the monolith's database schema has diverged. The message queue has new topics. The third-party integrations now call service endpoints, not monolith routes. Define: (1) what specific metric triggers rollback, (2) how you re-converge diverged schemas, (3) how you handle data written to new service databases, (4) rollback timeline. Also: DATA_INTEGRITY_UNPROVEN — 'validate after' means finding corruption in production instead of preventing it.


## Installation & Usage

To install and use the **Migration Strategy Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/migration-strategy-prover](https://vinkius.com/mcp/migration-strategy-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
