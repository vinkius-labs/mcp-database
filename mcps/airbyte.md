# Airbyte MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airbyte)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Monitor your Airbyte data pipelines via AI — track sync jobs, list sources, and check connections instantly.

## Description
Connect your **Airbyte** data integration instance to your AI agent to unlock conversational monitoring for your ETL/ELT pipelines. Let your agent audit your modern data stack automatically without touching the dashboard.

### What you can do

- **Monitor Connections** — Retrieve the full list of your configured connections linking sources to destinations
- **Track Jobs** — View historical synchronization runs, success rates, and identify failing sync jobs instantly
- **Audit Sources & Destinations** — List all your active data origins (like Postgres, Stripe) and targets (Snowflake, BigQuery)
- **Granular Inspection** — Fetch detailed UUID configuration and statuses for a specific source or active connection
- **Workspace Analytics** — Verify your active Airbyte workspaces and general environment configurations

### How it works

1. Subscribe to this server
2. Enter your Airbyte API URL and API Key
3. Let your agent run diagnostic queries via Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — let the agent check yesterday's sync job success rate or debug a failing database connection
- **Analytics Engineers** — quickly list configured warehouse destinations and verify infrastructure paths
- **Data Analysts** — get a high-level summary of all active data sources pumping into the main data lake


## Available Tools (7)
- **list_sources**: List all Airbyte sources
- **get_source**: Get details of a specific Airbyte source
- **list_destinations**: List all Airbyte destinations
- **list_connections**: List all Airbyte sync connections
- **get_connection**: Get details of a specific Airbyte connection
- **list_jobs**: List synchronization jobs for a connection
- **list_workspaces**: List workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airbyte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the sync history and job status for connection ID `e5f1b2c3...` to see if the nightly run failed."

**🤖 AI Agent:**
> I checked the recent jobs for that connection. The nightly sync run at 02:00 AM failed due to a missing Postgres credential timeout. The previous run at 01:00 AM succeeded. Would you like to review the specific failing logs?

---

**👤 You:**
> "Show me all the configured data destinations in our primary Airbyte workspace."

**🤖 AI Agent:**
> You have 3 active destinations in your workspace. 1) Snowflake Data Cloud (ID: ...a12), 2) Google BigQuery Prod, and 3) An Amazon S3 bucket used for raw JSON dumps.

---

**👤 You:**
> "List all active Airbyte connections handling our Stripe source."

**🤖 AI Agent:**
> I found 2 active connections reading from your Stripe source (ID: ...9ff). The first one syncs billing data to Snowflake every 10 minutes. The second pushes invoice records to an S3 log bucket daily.


## ❓ FAQ

**Q: Does this work with Airbyte Cloud and Self-Hosted Enterprise instances?**
Yes. You are required to pass the URL parameter during setup. You can use 'https://api.airbyte.com/v1' for Airbyte Cloud, or point it directly to your private self-hosted API endpoint hostname.

**Q: Can the agent create new connections or trigger sync jobs automatically?**
Currently, this core MCP exposes read-only tools designed to safely list, track, and monitor your infrastructure without accidentally mutating mission-critical data warehouse state during conversational usage.

**Q: How do I find a specific Connection ID to check its jobs?**
Simply ask the agent to run the list connections tool first! It will output all active connections alongside their UUIDs, which you can then ask the agent to dive deeper into.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airbyte](https://vinkius.com/mcp/airbyte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Airbyte** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `airbyte` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Airbyte** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airbyte": {
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
