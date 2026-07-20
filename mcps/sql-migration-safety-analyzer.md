# SQL Migration Safety Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sql-migration-safety-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Validate SQL migrations for structural risks, rollback integrity, and unbounded deletions.

## Description
Prevent destructive database changes by analyzing SQL migration strings before execution. This MCP server provides specialized tools to identify high-risk DDL operations like `DROP` or `RENAME`, verify that every structural change has a corresponding rollback statement using `validate_rollback_integrity`, and detect dangerous, unbounded deletions with `scan_for_unbounded_deletions`. Use `analyze_migration_security` to perform an initial safety check on your migration scripts.


## Available Tools (3)
- **analyze_migration_security**: Analyze a SQL migration string for structural risks
- **scan_for_unbounded_deletions**: Detect high-risk data manipulation commands
- **validate_rollback_integrity**: Ensure every structural change in the migration has a matching reversal command


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SQL Migration Safety Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this migration for security risks: 'DROP TABLE users;'"

**🤖 AI Agent:**
> The migration is unsafe. The `analyze_migration_security` tool identified a destructive operation: 'DROP TABLE users'.

---

**👤 You:**
> "Is my rollback script complete for this migration: 'ALTER TABLE orders ADD COLUMN status TEXT;'?"

**🤖 AI Agent:**
> The tool `validate_rollback_integrity` indicates that the change is uncovered because there is no corresponding command to drop the column in your rollback script.

---

**👤 You:**
> "Scan this SQL for unbounded deletions: 'DELETE FROM logs;'"

**🤖 AI Agent:**
> A critical risk was detected. The `scan_for_unbounded_deletions` tool found a DELETE statement without a WHERE clause, which could wipe the entire logs table.


## ❓ FAQ

**Q: How can I check if my migration script contains dangerous DROP commands?**
You can use the `analyze_migration_security` tool. It scans your SQL string for destructive DDL patterns and reports them.

**Q: What does it mean if a migration is flagged as having missing rollbacks?**
It means the tool detected structural changes (like `ALTER` or `RENAME`) that do not have a matching reversal command in your provided rollback script, which you can verify with `validate_rollback_integrity`.

**Q: Can this tool detect dangerous DELETE statements?**
Yes, the `scan_for_unbounded_deletions` tool specifically looks for `DELETE` or `TRUNCATE` commands that lack a `WHERE` clause or are otherwise high-risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sql-migration-safety-analyzer](https://vinkius.com/mcp/sql-migration-safety-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SQL Migration Safety Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sql-migration-safety-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SQL Migration Safety Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sql-migration-safety-analyzer": {
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
