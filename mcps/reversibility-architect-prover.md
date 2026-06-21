# Reversibility Architect Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reversibility-architect-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/reversibility-architect-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/reversibility-architect-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops](../categories/devops.md)

LLMs suggest irreversible architectural changes. This engine is a 6-pivot cognitive trap that forces the agent to map data rollbacks, blast radius, and canary deployments before executing.

## Description
The easiest way for an AI to break production is to propose a destructive database migration or a big-bang deployment. The Reversibility Architect Prover forces the AI to think like an SRE.

### The Semantic Trap

Before executing a deployment, the agent must pass a strict 6-pivot validation:

1. **dataMigrationReversible** — Prove that down-migrations won't destroy data.
2. **rollbackCriteriaDefined** — Define the exact metrics (e.g. 5xx errors > 2%) that trigger an abort.
3. **blastRadiusIsolated** — Prove that a failure won't cascade.
4. **downtimeEstimated** — Be honest about maintenance windows.
5. **featureFlagStrategy** — Prove it's not an all-or-nothing release.
6. **postMortemSimulation** — Imagine it failed. Why did it fail?


## Available Tools
- **validate_reversibility**: You must: (1) DATA MIGRATION — can we revert data changes without loss? Expand-then-contract, not rename-then-pray. Add columns before removing old ones, (2) ROLLBACK CRITERIA — define EXACT, MEASURABLE thresholds that trigger automatic rollback. Error rate > X% for Y minutes. Latency > Zms. Not "if something goes wrong", (3) BLAST RADIUS — how many users are affected if this fails? Canary (1% → 10% → 50% → 100%). Never all users simultaneously, (4) DOWNTIME — test time estimates on PRODUCTION-scale data. Development database timing is fiction for production, (5) FEATURE FLAGS — user-facing changes require a kill switch. Flag to 0% in 30 seconds vs redeploy in 15 minutes. (6) POST-MORTEM SIMULATION — imagine the change failed at 2 AM. Can the on-call engineer roll back without waking up the team? If rejected, the change is not safe to deploy.

Structured reflection tool that forces rollback planning, blast radius mapping, and data preservation analysis before any architectural or deployment change ships. Based on the "Pre-Mortem" methodology (Klein, 1998), change management frameworks (ITIL v4), and deployment safety patterns (Accelerate, Forsgren/Humble/Kim 2018). Catches Irreversible Migration (data migration with no rollback path — migration: "ALTER TABLE users RENAME COLUMN username TO display_name." Deployed. Application code updated to use display_name. Bug discovered: the migration broke a reporting service that queries username. Rollback attempt: "ALTER TABLE users RENAME COLUMN display_name TO username." But: the updated application code expects display_name. Now BOTH the old code and new code are broken. Reversible approach: (1) ADD column display_name. (2) Backfill display_name = username. (3) Update application to read from display_name. (4) Verify for 1 week. (5) THEN drop username column. At any point between steps 1-4, the old code still works. Rule: expand-then-contract. Never rename. Never delete until the old path is confirmed dead), Undefined Abort Criteria (no clear threshold for when to stop and rollback — "We will monitor and roll back if something goes wrong." What is "something"? Error rate > what%? Latency > how many ms? For how long? At 2 AM when the deploy finishes, the on-call engineer sees error rate at 3.2%. Is that "something wrong"? The baseline was 2.8%. Is 0.4% increase significant? Without defined criteria: the engineer waits. Error rate climbs to 5.1%. Still waiting. 8.3%. Now it is clearly wrong — but 45 minutes have passed and 12,000 users were affected. Defined criteria: "Auto-rollback if: error_rate > 4% for > 2 minutes, OR p95_latency > 800ms for > 5 minutes, OR any 5xx > 50/minute." These are measurable, automatable, and remove human judgment from a 2 AM decision), Unbounded Blast Radius (the change affects ALL users simultaneously — "Deploy the new payment flow to production." All users. All regions. At once. The new flow has a subtle bug: it rounds currency to 2 decimal places BEFORE tax calculation instead of after. For a $99.99 item at 8.25% tax: Correct: $99.99 × 1.0825 = $108.239175 → rounded: $108.24. Buggy: $100.00 (rounded) × 1.0825 = $108.25. Difference: $0.01 per transaction. At 50,000 transactions/day: $500/day in overcharges. Customer complaints start immediately — but ALL 50,000 daily users are affected. With canary deployment (1% → 10% → 50% → 100%): 1% = 500 users. Error detected at $5/day overcharge. Blast radius: 500 users × 1 day = 500 affected transactions (refundable). Without canary: 50,000 users × 3 days (time to detect + fix) = 150,000 affected transactions), Downtime Surprise (no estimation of unavailability during the change — "The migration should be quick." Migration: add an index to a 200M-row table. Development database (100K rows): 3 seconds. "Quick." Production database (200M rows): 4.5 hours. The table is locked for writes during index creation. Every user action that writes to this table fails for 4.5 hours. Fix: CREATE INDEX CONCURRENTLY (PostgreSQL) — does not lock the table but takes 6 hours. Or: scheduled maintenance window with user notification. Or: create index on a replica, then promote. The time estimate MUST be tested on production-scale data — not development-scale), and All-or-Nothing Deploy (no incremental rollout or feature flag strategy — "Deploy the redesigned dashboard." Old dashboard: removed. New dashboard: 100% of users. Discovery: the new dashboard loads 3.2 seconds (old: 1.1 seconds). Performance regression. Users complain. Rollback: redeploy the old code. Time: 15 minutes (build + deploy + cache clear). During those 15 minutes: every user sees the slow dashboard. With feature flag: dashboard_v2 flag set to 0% → 5% → 25% → 100%. At 5%: performance regression detected. Flag set to 0% — takes 30 seconds. Zero downtime. Zero redeployment. Instant rollback. Feature flags are not optional for user-facing changes — they are the rollback mechanism). Call once per deployment, migration, architecture change, or infrastructure modification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reversibility Architect Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Data: drop column. Rollback: restore backup."

**🤖 AI Agent:**
> Verdict: DATA_CORRUPTION_RISK. A backup restore implies data loss between the backup and the rollback. You must use additive migrations only.

---

**👤 You:**
> "Data: Additive only. Rollback: On error. Blast: Whole app. Down: None. Flag: Deploy all."

**🤖 AI Agent:**
> Verdict: ALL_OR_NOTHING_DEPLOY. You failed to use feature flags or a canary strategy.

---

**👤 You:**
> "Data: Additive migration. Rollback: 5xx > 1%. Blast: Search service only. Down: Zero. Flag: Canary 1%. Sim: Fails if redis times out."

**🤖 AI Agent:**
> Verdict: REVERSIBILITY_PROVEN. Architecture is safe to deploy.


## Installation & Usage

To install and use the **Reversibility Architect Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reversibility-architect-prover](https://vinkius.com/mcp/reversibility-architect-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
