# Database Architect Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/task-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

An AI agent designed a database schema with no indexes on search columns, no foreign keys, and a VARCHAR(255) for every field. Query response time went from 200ms to 14 seconds after 500K rows. Table locks during updates froze the application for 8 minutes. This tool forces 3NF normalization, index strategies mapped to access patterns, explicit foreign key constraints, and partition planning for high-volume tables.

## Description
LLMs generate database schemas that work on day one with 100 rows. By month three with 500K rows, queries take 14 seconds, UPDATE statements lock the entire table, and orphaned records pile up because nobody defined foreign keys. The schema worked. The architecture didn't.

### The Problem

AI-generated database schemas commit four structural violations that compound over time:

- **Normalization Violations** — Storing user addresses inside the orders table. Duplicating email columns across three tables. The agent treats normalization as optional. Every duplicate is a future inconsistency.
- **Query Blindness** — No indexes on `WHERE` clauses. No composite indexes for multi-column filters. The schema has 20 tables and zero index definitions. Every query becomes a full table scan at scale.
- **Orphaned Relations** — No foreign keys. No cascade rules. Delete a user and their 10,000 orders remain as ghost data. Referential integrity is not enforced — it's hoped for.
- **Scaling Ignorance** — INT for a primary key that will exceed 2.1 billion. VARCHAR(255) for a field that stores 'yes' or 'no'. No partition strategy for tables growing at 1M rows/month. The schema breaks silently at scale.

### How It Works

4 Decision Pivots govern the schema validation:

1. **normalizationChecked** — Is the schema in 3NF? Are denormalization decisions explicitly justified with access pattern rationale?
2. **indexesProposed** — Does every `WHERE`, `JOIN`, and `ORDER BY` column have a corresponding index? Are composite indexes defined for multi-column queries?
3. **relationshipsEnforced** — Are foreign keys defined with explicit `ON DELETE` and `ON UPDATE` cascade rules? No implicit relationships.
4. **scalabilityAddressed** — Are datatypes sized for growth (BIGINT vs INT)? Are partition strategies defined for tables exceeding 10M rows?

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| normalizationChecked = false | NORMALIZATION_VIOLATED | Redundant data. Inconsistencies guaranteed at scale. |
| indexesProposed = false | QUERY_BLIND | No index strategy. Full table scans at scale. |
| relationshipsEnforced = false | ORPHAN_PRONE | No foreign keys. Data integrity is a wish, not a constraint. |
| scalabilityAddressed = false | SCALE_UNPLANNED | Schema breaks at volume. Integer overflows and full scans incoming. |
| All pivots pass | SCHEMA_PROVEN | Normalized, indexed, constrained, and scaled for production. |

### Why It Works

- **Tool calls are obligations.** The agent cannot claim indexes are defined without naming them. Filling the fields IS the schema design.
- **Consistency engine catches contradictions.** Claiming `indexesProposed=true` but listing zero index definitions triggers rejection.
- **Semantic traps detect lazy answers.** 'The ORM handles indexing,' 'we'll optimize later,' or 'the database auto-manages constraints' all trigger automatic rejection.


## Available Tools (1)
- **validate_database_schema**: Think like a DBA who has been woken at 3 AM by a slow query alert on a 50M row table — every missing index is a future incident, every missing FK is a future data corruption, every wrong datatype is a future migration emergency. You must: (1) justify NORMALIZATION — each table has a single responsibility. Redundant columns must be explicitly justified as intentional denormalization with the specific read performance reason. "We store user_email in orders for convenience" is not justification — "Denormalized for invoice generation: 50K invoices/day, join would add 12ms per invoice at scale" is, (2) define INDEXES against real ACCESS PATTERNS — which queries run most frequently? Which queries are slowest? Composite indexes for multi-column WHERE + ORDER BY. Covering indexes for read-heavy paths. Partial indexes for filtered subsets. "We will add indexes later" means a production incident, (3) enforce RELATIONSHIPS — foreign keys on every reference column, explicit ON DELETE rules (CASCADE, SET NULL, RESTRICT — never default), ON UPDATE rules, unique constraints, check constraints. Every missing FK is a data corruption vector, (4) plan for SCALE — estimate row counts at 1 year, 3 years. Choose datatypes accordingly (BIGINT vs INT, TIMESTAMPTZ vs TIMESTAMP, UUID vs SERIAL). Plan partitioning for tables >10M rows. Plan archival for time-series data, (5) design MIGRATION SAFETY — how will this schema evolve? Expand/contract for column changes. CREATE INDEX CONCURRENTLY for production indexes. No ALTER TABLE ... ADD COLUMN NOT NULL without default on large tables. Backward-compatible migrations only. If rejected, your schema has a production-critical flaw.Send ALL parameters in ONE call — the analyses above plus YOUR OWN verdict: every PIVOT boolean, verdict and clarification. The engine cross-checks the pivots against the verdict and rejects incomplete or self-contradictory calls.

Structured reflection tool for production-grade database schema architecture. Forces the agent to justify normalization decisions, define indexes against measured access patterns, enforce referential integrity with explicit cascade rules, plan for data volume growth, and design migration safety for schema evolution. Catches Schema Bloat (unnormalized tables with redundant columns — storing user_email in 5 tables instead of joining on user_id. Each copy is a consistency bug waiting to happen), Query Blindness (no indexes defined against actual access patterns — "we will optimize later" means a full table scan on 10M rows in production at 3 AM), Orphaned Relationships (no foreign keys, no ON DELETE rules — deleting a user leaves orphaned orders, payments, and sessions that corrupt reports and break cascading logic), Scalability Ignorance (INT for a primary key that will exceed 2.1B rows, VARCHAR(255) for every string, no partitioning strategy for tables that grow 1M rows/month), and Migration Blindness (no plan for schema evolution — adding a NOT NULL column to a 50M row table locks writes for 45 minutes without expand/contract strategy). Call once per schema design or database migration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Database Architect Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a users table."

**🤖 AI Agent:**
> Verdict: QUERY_BLIND. You admitted access patterns aren't defined. Define real indexes instead of assuming the database will magically scale.

---

**👤 You:**
> "I added indexes but forgot foreign keys."

**🤖 AI Agent:**
> Verdict: RELATIONSHIPS_ORPHANED. Your relational strategy is dangerous. Define explicit foreign keys.

---

**👤 You:**
> "Schema is normalized, indexed, has FKs, and sized for 10M rows."

**🤖 AI Agent:**
> Verdict: SCHEMA_PROVEN. Schema architecture validated successfully. You demonstrated a resilient approach.


## ❓ FAQ

**Q: Does this Prover generate SQL queries automatically?**
No. The AI agent generates the code. This tool validates the relational architectural design, forcing index plans, relationship rules, and scaling bounds before writing SQL.

**Q: Can I use this for non-relational schemas (like MongoDB)?**
Yes. The core validation concepts (access pattern indexing, scaling capacity, and references) apply equally to document schemas and key-value distributions.

**Q: How does the tool enforce schema consistency?**
The engine uses structured decision pivots. If the proposed layout misses index patterns or foreign keys, the validation engine rejects the execution step.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/task-planner](https://vinkius.com/ai-agent-connect/task-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Database Architect Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `task-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Database Architect Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "task-planner": {
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
