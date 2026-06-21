# Snowflake MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snowflake)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/snowflake-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/snowflake-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Bring your absolute data cloud into your AI editor. Execute queries, list warehouses, and map complex schemas natively.

## Description
Connect your **Snowflake** AI Data Cloud with your AI agent to radically accelerate the way you query large datasets and audit cloud data warehouses. Navigate through deep hierarchical trees of databases, tables, and internal stages natively by chatting with your IDE. Keep your SQL robust by validating commands directly against the live engine.

### What you can do

- **Execute Queries in Chat** — Tell your bot to `execute_sql` based on human prompts or test new complex table joins safely right inside Cursor or Claude
- **Map Infrastructures** — Quickly retrieve spatial contexts by pulling `list_databases`, traversing downwards through `list_schemas` to target specific columns
- **Audit Compute Cost** — Keep a firm grip on active clusters running by auditing running instances using `list_warehouses`
- **Diagnose Operations** — Monitor long-tail data workloads or data engineering pipelines using the `get_query_status` method asynchronously

### How it works

1. Subscribe to this AI integration server
2. Introduce your explicit Snowflake Account identifier (e.g. `abc123.us-east-1`)
3. Inject your Snowflake OAuth token or JWT Token (key pair) authentication string
4. Ask Claude or Cursor to look into the Sales Database schema

Stop juggling browser instances to paste a quick query in Snowflake Snowsight. Stay strictly inside your local codebase while examining the exact table data types.

### Who is this for?

- **Data Engineers** — validate that raw datasets correctly land in internal environments (`list_stages`) straight from your IDE window
- **Analytics Engineers / dbt** — generate highly accurate SQL modeling by letting your agent examine the `list_tables` definitions live
- **Software Architects** — write an agentic script pulling raw diagnostic query metrics without downloading hefty SDK kits locally


## Available Tools
- **list_databases**: Lists all databases in the Snowflake account
- **list_schemas**: Lists all schemas within a specific database
- **list_tables**: Lists all tables within a specific schema
- **execute_sql**: Prefers read-only statements whenever possible.

Executes a SQL query on Snowflake
- **list_warehouses**: Lists all virtual warehouses
- **list_stages**: Lists all internal and external stages
- **get_query_status**: Retrieves the status of an asynchronous query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snowflake** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all running virtual warehouses I can access in my Snowflake account."

**🤖 AI Agent:**
> I've called `list_warehouses` for your targeted Snowflake footprint.

**Running Clusters Detected**:
1. `COMPUTE_WH` – Size: X-Small | State: SUSPENDED
2. `ANALYTICS_WH` – Size: Large | State: STARTED
3. `ETL_LOAD_WH` – Size: Medium | State: STARTED

Would you like me to run an analytical snippet under `ANALYTICS_WH` now?

---

**👤 You:**
> "Write a query to grab the top 5 most engaged users from our schema and execute it."

**🤖 AI Agent:**
> No problem! I constructed this query to target exactly that and executed it against the system:
`SELECT user_id, email, activity_score FROM prod_schema.users ORDER BY activity_score DESC LIMIT 5;`

**Snowflake Output Data**:
1. alice@example.com (Score: 980)
2. john84@test.io (Score: 964)
3. m_reyes@corp.com (Score: 941)
[...]

Do you want me to format this as a markdown table or save the dataset?

---

**👤 You:**
> "Retrieve the schema mapping for the MASTER_DB. I need to know all nested tables before doing table joints."

**🤖 AI Agent:**
> Using `list_schemas`, `MASTER_DB` contains main partitions:
1. `PUBLIC`
2. `ANALYTICS_GOLD`

Digging into `ANALYTICS_GOLD` using `list_tables`:
- `dim_customers` (Type: BASE TABLE)
- `dim_geography` (Type: BASE TABLE)
- `fct_sales_records` (Type: BASE TABLE)
- `vw_live_revenue` (Type: VIEW)

I am ready to help build your exact JOINS. For example, `fct_sales_records.customer_id` directly joins on `dim_customers.id`.


## Installation & Usage

To install and use the **Snowflake** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snowflake](https://vinkius.com/mcp/snowflake)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
