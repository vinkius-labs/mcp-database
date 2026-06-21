# Migration Strategy Prover MCP Server

An AI recommended a big-bang database migration over the weekend. No dependency map — 7 services read from that database. No rollback plan — 'just restore from backup.' No data validation — 2.3 million records with timezone-dependent timestamps. The migration ran Saturday at 2 AM. By 4 AM, 3 downstream services were returning stale data, the backup was 6 hours old, and 14,000 customer records had corrupted timestamps. Monday morning: 72-hour incident. This tool forces risk assessment, rollback definition, data integrity verification, cutover planning, and stakeholder alignment.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/migration-strategy-prover)

## Overview
**Category:** devops
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Migration Strategy Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/migration-strategy-prover](https://vinkius.com/mcp/migration-strategy-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
