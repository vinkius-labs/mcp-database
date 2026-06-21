# SQL Parser AST Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sql-parser-ast-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sql-parser-ast-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sql-parser-ast-engine-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **SQL Parser AST Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sql-parser-ast-engine](https://vinkius.com/mcp/sql-parser-ast-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
