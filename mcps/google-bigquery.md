# Google BigQuery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-bigquery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Empower your AI agent to query massive datasets via BigQuery — execute Standard SQL, track active jobs, and inspect table schemas natively.

## Description
Connect your **Google BigQuery** data warehouse to any AI agent and empower it to act as a fractional data analyst. Traverse structured schemas, audit data pipelines, and execute complex aggregations over petabytes of data purely through conversational prompts.

### What you can do

- **Execute Queries** — Prompt natively structural Data Analytics requests and allow the LLM to write, run, and summarize exact `Standard SQL` instantly
- **Discover Schemas** — Inspect deep table column mappings, discovering strict clustering logic and native partitioning limits
- **Audit Workloads** — Paginate recent cluster jobs, identify heavily delayed computations globally, and read bytes explicitly processed by runs
- **Dataset Topologies** — Traverse nested datasets logically mapping GCP access properties recursively
- **Performance Troubleshooting** — Read exact job error traces directly confirming syntax failures natively

### How it works

1. Subscribe to this server
2. Enter your GCP Project ID and an active OAuth/Service Account Token
3. Start querying terabytes of rows securely from Claude, Cursor, or your preferred agent workspace

Stop switching into the GCP Console for quick data validations. Check database constraints and summarize recent daily logs all from your chat.

### Who is this for?

- **Data Engineers** — troubleshoot failing scheduled queries and explore undocumented columns securely on-the-fly
- **Marketing Analysts** — request customer cohorts using conversational logic that natively translates to optimized SQL
- **Backend Developers** — rapidly confirm if application background pipelines successfully inserted the necessary rows without breaking flow


## Available Tools
- **list_datasets**: List all explicit Datasets in the active GCP project
- **get_dataset**: Get exact details of a specific BigQuery dataset
- **list_tables**: List explicit Tables natively contained within a Dataset
- **get_table**: Get explicit metadata and schema details of a pure BigQuery Table
- **execute_query**: Run an explicit BigQuery Standard SQL command
- **list_jobs**: List recent explicit BigQuery runtime Jobs securely
- **get_job**: Get complete details of a specific BigQuery Job run


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google BigQuery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the table schema for `users_prod` in the `analytics` dataset."

**🤖 AI Agent:**
> Schema fetched. `users_prod` contains 12 columns, notably `user_id` (STRING, required), `signup_timestamp` (TIMESTAMP, partitioned), and `plan_tier` (STRING). Would you like to check some sample rows?

---

**👤 You:**
> "Find out the top 3 countries with the most signups this month in the `users` table."

**🤖 AI Agent:**
> Executing SQL... The query completed successfully processing 12MB. The top 3 countries are: 1) United States (12,400), 2) Brazil (8,900), 3) Japan (4,150).

---

**👤 You:**
> "Did the overnight cron job compute successfully or did it fail?"

**🤖 AI Agent:**
> Listing recent jobs. Job `cron_transform_01` (ID: 11a0ab3-xxx) failed globally at 03:00AM. Root cause trace indicates native `Unrecognized name: user_account_id` syntax failure halting workflow explicitly mapped.


## ❓ FAQ

**Q: Can my AI write its own queries if I just ask it a business question?**
Yes! The agent will typically use `list_tables` and `get_table` to study the columns first. Then, realizing constraints, it will natively invoke `execute_query` running an optimized Standard SQL string to fetch exactly what you asked for.

**Q: Will my prompt fail if it returns millions of rows?**
It might hit the context window boundaries of the chosen foundational LLM. Good practice suggests instructing your AI to always append `LIMIT 100` initially or run macro aggregations (like `COUNT()` or `SUM()`) natively inside BigQuery first.

**Q: How do I check if a query was expensive after it ran?**
Use the `list_jobs` or `get_job` endpoints. They expose metadata directly from Google's history returning the `totalBytesProcessed` flag so your agent can estimate overhead intelligently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-bigquery](https://vinkius.com/mcp/google-bigquery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google BigQuery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-bigquery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google BigQuery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-bigquery": {
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
