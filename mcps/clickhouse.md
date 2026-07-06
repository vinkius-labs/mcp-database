# ClickHouse MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clickhouse)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Query and manage ClickHouse databases — execute analytical SQL, monitor replication status, and manage schemas directly from your AI agent.

## Description
Connect your **ClickHouse** instance to any AI agent to perform lightning-fast OLAP queries and manage your data infrastructure through natural language.

### What you can do

- **Analytical Queries** — Execute read-only SELECT queries with automatic safety limits using the `select_query` tool.
- **Schema Management** — Create, alter, or drop tables and databases using the `execute_query` action for mutating operations.
- **Health Monitoring** — Instantly verify server availability with `ping` and check replication lag across clusters with `replicas_status`.
- **Performance Tuning** — Pass specific settings like `max_rows_to_read` or `max_execution_time` to optimize resource usage.

### How it works

1. Subscribe to this server
2. Enter your ClickHouse URL, Username, and Password
3. Start querying your big data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — quickly inspect table schemas and row counts without switching to a SQL IDE.
- **Analysts** — run complex aggregations and get instant summaries of large datasets.
- **DevOps** — monitor cluster health and replication status during maintenance or incidents.


## Available Tools (4)
- **replicas_status**: Check ClickHouse replica delay
- **select_query**: Automatically enforces readonly=1.

Execute a read-only SELECT query on ClickHouse
- **execute_query**: Execute a mutating query on ClickHouse
- **ping**: Check ClickHouse server health


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClickHouse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the ClickHouse server is online and reachable."

**🤖 AI Agent:**
> I've called the `ping` endpoint and the server is healthy and responding correctly.

---

**👤 You:**
> "Run a select_query to find the top 5 largest tables in the 'system' database."

**🤖 AI Agent:**
> I've executed the query on the system.parts table. The largest tables are: 'hits' (50GB), 'events' (42GB), 'logs' (30GB)... Would you like to see the full breakdown?

---

**👤 You:**
> "Use execute_query to create a new table called 'mcp_test' with an id column."

**🤖 AI Agent:**
> The `execute_query` action was successful. The table 'mcp_test' has been created in the default database with the specified schema.


## ❓ FAQ

**Q: Can I safely run analytical queries without accidentally modifying data?**
Yes. The `select_query` tool is strictly read-only and automatically enforces the `readonly=1` setting, ensuring that only SELECT, SHOW, and DESCRIBE operations are permitted.

**Q: How do I check if my ClickHouse cluster is healthy and synchronized?**
You can use the `ping` tool to check server reachability and the `replicas_status` tool to inspect replication delays and the status of your replicas.

**Q: Is it possible to create new tables or insert data using this server?**
Yes. For mutating operations like INSERT, CREATE, or ALTER, use the `execute_query` action. This tool allows you to modify the database schema and manage data records.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickhouse](https://vinkius.com/mcp/clickhouse)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ClickHouse** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clickhouse` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClickHouse** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clickhouse": {
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
