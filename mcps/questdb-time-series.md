# QuestDB (Time-Series) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/questdb-time-series)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/questdb-time-series-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/questdb-time-series-mcp)
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


## Installation & Usage

To install and use the **QuestDB (Time-Series)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/questdb-time-series](https://vinkius.com/mcp/questdb-time-series)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
