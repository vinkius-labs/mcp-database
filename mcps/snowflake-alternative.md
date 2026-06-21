# Snowflake MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snowflake-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/snowflake-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/snowflake-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Execute SQL queries, manage databases, and analyze data on Snowflake with AI agents.

## Description
Connect your **Snowflake** account to any AI agent to automate your data cloud operations and analytical workflows. Snowflake provides a premier platform for data warehousing and analysis, and this integration allows you to execute SQL statements, browse database schemas, and monitor session contexts through natural conversation.

### What you can do

- **SQL Query Orchestration** — Execute any SQL statement programmatically and retrieve real-time data results for immediate analysis.
- **Database & Schema Oversight** — List and search through databases, schemas, and tables to maintain a clear overview of your data architecture directly from the AI interface.
- **Warehouse & Resource Control** — Access and monitor available warehouses and user roles to ensure your analytical environment is properly configured.
- **Metadata Intelligence** — Describe table structures and retrieve session context metadata via natural language commands to facilitate data exploration.
- **Operational Monitoring** — Track statement execution status and cancel long-running queries to ensure your data cloud resources are used efficiently.

### How it works

1. Subscribe to this server
2. Enter your Snowflake Account Identifier and Token (JWT or OAuth2)
3. Start managing your data cloud from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly retrieve query results and explore table schemas without switching between SQL editors.
- **BI Engineers** — automate the retrieval of database metadata and monitor warehouse usage via natural conversation.
- **Data Scientists** — streamline the exploration of large datasets and track session contexts directly within the chat.


## Available Tools
- **cancel_sql**: Cancel a running SQL statement
- **describe_table**: Get table schema details
- **execute_sql**: Returns the first partition of results or a handle for long-running queries.

Execute a SQL statement in Snowflake
- **get_session_context**: Get current session context
- **get_statement_status**: Check the status of a SQL statement
- **list_databases**: List all accessible databases
- **list_roles**: List security roles
- **list_schemas**: List schemas in a database
- **list_tables**: List tables in a schema or database
- **list_users**: List Snowflake users
- **list_warehouses**: List compute warehouses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snowflake** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tables in the 'SALES' schema of the 'PROD' database."

**🤖 AI Agent:**
> I've retrieved the tables for you. The 'SALES' schema contains 5 tables: 'ORDERS', 'CUSTOMERS', 'INVOICES', 'PRODUCTS', and 'TRANSACTIONS'. Which one would you like to describe?

---

**👤 You:**
> "Show me the warehouse usage and query performance metrics for all active Snowflake warehouses."

**🤖 AI Agent:**
> 4 active warehouses. "ANALYTICS_WH" (X-Large): 78% utilization, 234 queries today, avg execution 4.2s, $89 credit usage. "ETL_WH" (Large): 45% utilization, 56 queries, avg 12.3s, $34 credits. "REPORTING_WH" (Medium): 23% utilization, 890 queries, avg 1.8s, $12 credits. "DEV_WH" (Small): 12% utilization, 45 queries, avg 3.4s, $4 credits. Total credits today: $139. Auto-suspend: all enabled (5 min idle). Queued queries: 0. Failed queries: 3 (timeout on ANALYTICS_WH). Storage: 12.4 TB used.

---

**👤 You:**
> "Run a SQL query to get the top 10 customers by revenue from the sales table this quarter."

**🤖 AI Agent:**
> Query executed on ANALYTICS_WH (1.2s). Top 10 customers by Q2 2025 revenue: 1) Meridian Corp: $234,000 (45 orders). 2) TechVentures: $189,000 (23 orders). 3) DataFlow: $156,000 (67 orders). 4) ScaleUp: $123,000 (34 orders). 5) CloudBridge: $98,000 (12 orders). 6-10: combined $345,000. Total Q2 revenue: $1.45M. Top 10 = 78% of total revenue. Rows scanned: 45,678. Credits used: 0.02. Query ID: 01abc-def-234.


## Installation & Usage

To install and use the **Snowflake** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snowflake-alternative](https://vinkius.com/mcp/snowflake-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
