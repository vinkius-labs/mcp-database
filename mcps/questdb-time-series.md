# QuestDB (Time-Series) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/questdb-time-series)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

High-performance time-series database for fast SQL queries, data ingestion, and real-time analytics directly from your AI agent.

## Description
Connect your **QuestDB** instance to any AI agent to perform high-speed time-series analysis and data management using natural language.

### What you can do

- **SQL Execution** — Run complex SQL queries, DDL, and DML operations optimized for time-series data.
- **High-Speed Ingestion** — Import tabular data (CSV/TSV) directly into tables with automatic schema creation and partitioning.
- **Data Export** — Extract large datasets in CSV or Parquet formats for external analysis or reporting.
- **Health Monitoring** — Instantly check server status and version information to ensure your database is operational.

### How it works

1. Subscribe to this server
2. Provide your QuestDB URL and optional credentials (Username/Password or Token)
3. Start querying and managing your time-series data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — Quickly inspect table schemas, run migrations, and verify data ingestion pipelines.
- **Analysts** — Perform ad-hoc time-series analysis and export results without writing complex scripts.
- **DevOps Teams** — Monitor database health and perform maintenance tasks through a conversational interface.


## Available Tools
- **execute_sql**: Use this for standard SELECT, INSERT, or DDL operations.

Execute SQL statements (queries, DDL, DML) on QuestDB
- **export_data**: Useful for extracting large datasets.

Export query results as CSV or Parquet
- **import_data**: Automatically creates tables and columns if they do not exist.

Import tabular data (CSV, TSV) into a table
- **ping**: Health check and version information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QuestDB (Time-Series)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the QuestDB server is online and show me the version."

**🤖 AI Agent:**
> I've pinged the server. It is currently online and running QuestDB version 8.1.0.

---

**👤 You:**
> "Execute a query to find the average temperature from the 'sensors' table for the last hour."

**🤖 AI Agent:**
> Executing SQL... The average temperature for the last hour is 22.5°C based on 1,200 data points in the 'sensors' table.

---

**👤 You:**
> "Export the last 1000 rows of the 'trades' table as a CSV file."

**🤖 AI Agent:**
> I've initiated the data export. You can now download the CSV containing the last 1000 trade records.


## ❓ FAQ

**Q: Can I execute standard SQL queries and DDL commands like creating tables?**
Yes! Use the `execute_sql` tool to run any valid QuestDB SQL statement, including SELECT, INSERT, and table definitions. You can also include parameters like `explain` to see the execution plan.

**Q: How do I import a CSV file into a new or existing table?**
Use the `import_data` tool. Provide the target table name and the raw CSV data. The tool can automatically create the table structure and handle partitioning if specified.

**Q: Is there a way to export large query results for use in other tools?**
Absolutely. The `export_data` tool allows you to run a query and receive the output in CSV or Parquet format, which is ideal for large-scale data extraction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/questdb-time-series](https://vinkius.com/mcp/questdb-time-series)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QuestDB (Time-Series)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `questdb-time-series` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QuestDB (Time-Series)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "questdb-time-series": {
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
