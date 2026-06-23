# Coalesce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coalesce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Enable your AI agent to manage Snowflake data pipelines, trigger transformations, and monitor jobs via the Coalesce API.

## Description
Connect your AI to **Coalesce**, the data transformation platform built for Snowflake with a column-aware approach.

### What you can do

- **Environment Management** — List all environments in your Coalesce organization and inspect their configurations.
- **Job Monitoring** — Check the status of the last run for any environment and view execution logs.
- **Trigger Transformations** — Start transformation jobs on demand with optional node selectors to target specific pipelines.

### How it works

1. Add the Coalesce integration to your AI toolset.
2. Provide your API Token (from Organization Settings > API Tokens).
3. Manage your data pipelines via natural language.

### Who is this for?

- **Data Engineers** — Trigger and monitor pipeline runs without opening the Coalesce UI.
- **Analytics Engineers** — Check job statuses and debug failed transformations from chat.
- **Data Team Leads** — Get quick overviews of environment health and recent job results.


## Available Tools (8)
- **get_environment**: Retrieve detailed information about a specific environment
- **get_job_details**: Retrieve detailed information about a specific job
- **get_run_status**: Check the current status and progress of a triggered run
- **list_environments**: Retrieve all environments configured in your Coalesce organization
- **list_jobs**: Retrieve a list of jobs, optionally filtered by environment
- **list_nodes**: Retrieve metadata about transformation nodes in a specific environment
- **trigger_job**: Trigger a specific job in an environment
- **trigger_run**: Trigger a new run for a specific environment and optionally a job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coalesce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all environments in my Coalesce organization."

**🤖 AI Agent:**
> You have 3 environments:
1. 'Production' (env-001) — Last run: success, 2h ago
2. 'Staging' (env-002) — Last run: success, 5h ago
3. 'Development' (env-003) — Last run: failed, 1h ago
Would you like to check the failed run details?

---

**👤 You:**
> "Trigger job 'job-yyyy' in environment 'env-xxxx'."

**🤖 AI Agent:**
> Job 'job-yyyy' triggered in environment 'env-xxxx'. Run ID: run-8k3m. Status: running. Estimated completion: ~4 minutes.

---

**👤 You:**
> "What is the status of the ongoing production data pipeline?"

**🤖 AI Agent:**
> The production pipeline (Run ID: run-9g1l) is currently at 85%. All dimension tables have refreshed successfully, and the fact nodes are currently materializing in Snowflake.


## ❓ FAQ

**Q: How do I get my Coalesce API token?**
In the Coalesce UI, go to **Organization Settings > API Tokens** and generate a new token. Copy it and paste it below.

**Q: Does this work with Snowflake?**
Yes. Coalesce is built specifically for Snowflake. The API triggers jobs that run directly on your Snowflake instance.

**Q: What is a Node Selector?**
A Node Selector lets you filter which transformation nodes to include in a run, based on name, type, or tags.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coalesce](https://vinkius.com/mcp/coalesce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coalesce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coalesce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coalesce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coalesce": {
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
