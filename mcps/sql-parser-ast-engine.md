# SQL Parser AST Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sql-parser-ast-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Parse any SQL query into a structured AST — extract tables, columns, JOINs, and WHERE clauses programmatically. Supports 15+ dialects including MySQL, PostgreSQL, and BigQuery. Your SQL injection firewall.

## Description
A security agent receives a SQL query from user input. Is it safe? Does it access unauthorized tables? Is there a `DROP TABLE` hiding inside a subquery? An AI scanning the text will miss edge cases that a real parser catches.

This MCP parses SQL into a complete Abstract Syntax Tree — every table, column, JOIN, WHERE clause, subquery, and function call becomes a structured, inspectable object. Then it can rebuild valid SQL from the AST.

### The Superpowers

- **SQL Injection Detection:** Decompose any query to inspect for unauthorized operations, table access, and injection patterns.
- **15+ Dialects:** MySQL, PostgreSQL, MariaDB, SQLite, BigQuery, Snowflake, Hive, TransactSQL, and more.
- **Bidirectional:** Parse SQL→AST and rebuild AST→SQL with full fidelity.
- **Table & Column Extraction:** List every table and column referenced in a query — essential for data governance.


## Available Tools (1)
- **parse_sql**: This is essential for security agents checking for SQL injection, DevOps agents auditing query performance, or any workflow that needs to understand SQL without executing it. Supported dialects: MySQL, PostgreSQL, MariaDB, SQLite, BigQuery, Snowflake, Hive, FlinkSQL, Noql, TransactSQL.

Parses SQL queries into an AST and extracts tables, columns, and WHERE clauses. Supports 15+ dialects (MySQL, PostgreSQL, BigQuery, Snowflake, etc.)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SQL Parser AST Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "A user submitted this SQL query through our API. Parse it and check if it accesses any tables beyond 'orders' and 'products'."

**🤖 AI Agent:**
> Tables extracted: orders, products, users. ⚠️ 'users' table access detected — not in allowed list.

---

**👤 You:**
> "Extract all columns referenced in this BigQuery analytics query for our data governance audit."

**🤖 AI Agent:**
> 14 columns extracted across 3 tables with full table.column qualified names.

---

**👤 You:**
> "Validate this PostgreSQL migration query for syntax errors before deploying to production."

**🤖 AI Agent:**
> AST parsed successfully — no syntax errors. Query is valid PostgreSQL.


## ❓ FAQ

**Q: Can this detect SQL injection attempts?**
Yes. Parse the query into AST and inspect the node types. If user input resulted in unexpected DROP, DELETE, UNION, or subquery nodes, the injection is exposed structurally — no regex guessing.

**Q: Which SQL dialects are supported?**
15+: MySQL, PostgreSQL, MariaDB, SQLite, BigQuery, Snowflake, Hive, TransactSQL, FLINKSQL, FlinkSQL, PostgresQL, and more.

**Q: Can I rebuild SQL from the AST?**
Yes. Parse SQL→AST, modify the AST programmatically (add WHERE clauses, change table names), and rebuild valid SQL. Full round-trip support.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sql-parser-ast-engine](https://vinkius.com/mcp/sql-parser-ast-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SQL Parser AST Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sql-parser-ast-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SQL Parser AST Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sql-parser-ast-engine": {
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
