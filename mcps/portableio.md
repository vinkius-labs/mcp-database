# Portable.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/portableio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Portable ETL pipelines directly via your AI agent — monitor flows, sync runs, and destination details seamlessly.

## Description
Connect your **Portable.io** account to your favorite AI agent and take orchestrate your data pipelines through natural language.

### What you can do

- **Data Flows** — List configured integration flows and view complex mapping details
- **Sync Runs** — Monitor execution history, track successful row counts, and spot failure logs
- **Destinations & Connectors** — Retrieve all supported SaaS extractors and targeted data warehouses (like Snowflake or BigQuery)
- **Account Status** — Check your workspace bounds and execution limits instantly

### How it works

1. Subscribe to this server
2. Enter your Portable API Key
3. Command your pipelines via Claude, Cursor, or any MCP-compatible agent

### Who is this for?

- **Data Engineers** — troubleshoot pipeline runs and check mappings without switching context
- **Analytics Teams** — trace delayed warehouse loads and investigate connector configurations
- **Ops Managers** — monitor synchronization health across multiple SaaS environments


## Available Tools
- **list_flows**: List all integration flows configured in Portable
- **get_flow**: Get complete configuration details of a specific data flow
- **list_runs**: List historical execution runs for a specific data flow
- **list_connectors**: List available pre-built API data source connectors
- **list_destinations**: g., Snowflake, BigQuery) currently authorized to receive raw data writes from active flows.

List all configured data warehouse destinations
- **get_account**: Retrieve the exact workspace and account billing details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portable.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active ETL flows running in my Portable workspace."

**🤖 AI Agent:**
> I found 3 active flows. 'Stripe to Snowflake' runs every hour. 'Hubspot to BigQuery' runs daily. 'Shopify Orders' is paused. Would you like to view the recent execution runs for the Stripe sync?

---

**👤 You:**
> "Show the recent runs for flow ID 4087 and tell me if any failed."

**🤖 AI Agent:**
> For flow 4087, the last 4 runs were successful, processing exactly 12,045 rows. However, the run on Tuesday at 4 AM failed with 'API Rate Limit Exceeded' from the source connector. Should I pull the destination configuration details?

---

**👤 You:**
> "What destinations are currently configured to receive data?"

**🤖 AI Agent:**
> You have 2 active destinations connected: 'Production Warehouse' (BigQuery) and 'Analytics Replica' (Snowflake). Connecting new flows will write directly into the authorized schemas on these platforms.


## ❓ FAQ

**Q: Can my AI check why a recent data ingestion failed?**
Yes. Ask the agent to list the historical runs for a specific flow ID. It will return the execution logs, row counts, and error details, allowing the AI to pinpoint exactly where and why the sync pipeline broke without navigating a UI dashboard.

**Q: Which destinations and sources can the agent inventory?**
Your agent maps your entire active landscape. It can retrieve both the explicit warehouse targets (e.g. your authorized BigQuery and Snowflake environments) and the vast catalog of pre-built SaaS API connectors available in your Portable environment.

**Q: How can I check my workspace extraction limits?**
Simply ask the AI to retrieve your account details. It immediately pulls the absolute billing limits, extraction caps, and active feature toggles applied to your organization, providing a clear footprint of your usage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portableio](https://vinkius.com/mcp/portableio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Portable.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `portableio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Portable.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "portableio": {
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
