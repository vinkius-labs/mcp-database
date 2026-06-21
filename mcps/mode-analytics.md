# Mode Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mode-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Manage collaborative data analysis via Mode Analytics — list spaces, query reports, and trigger report runs directly from any AI agent.

## Description
Connect your **Mode Analytics** workspace to any AI agent and take full control of your data science and business intelligence workflows through natural conversation.

### What you can do

- **Workspace Oversight** — List all spaces and members to maintain visibility over your analytical environment.
- **Report Discovery** — List and retrieve detailed metadata for reports across different spaces.
- **Live Execution** — Trigger new report runs directly through the agent, including support for custom parameters.
- **Query Auditing** — List the underlying SQL queries for any report to understand data lineage and logic.
- **Definition Tracking** — List calculated field definitions to ensure consistency in your metrics.

### How it works

1. Subscribe to this server
2. Enter your Mode API Token, API Secret, and Workspace slug
3. Start interacting with your data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly check report run status or audit SQL queries without leaving your IDE.
- **Business Intelligence Managers** — monitor workspace activity and report usage during planning phases.
- **Growth Teams** — trigger updated data runs for specific campaigns directly from your chat interface.


## Available Tools
- **run_mode_report**: Trigger a new run for a report
- **get_mode_account**: Get authenticated account details
- **get_mode_report_run**: Get details for a report run
- **get_mode_report**: Get details for a specific report
- **list_mode_definitions**: List calculated field definitions
- **list_mode_members**: List workspace members
- **list_mode_queries**: List SQL queries in a report
- **list_mode_report_runs**: List runs for a report
- **list_mode_reports**: List reports in a space
- **list_mode_spaces**: List Mode Analytics spaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mode Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all reports in the 'Marketing Analytics' space."

**🤖 AI Agent:**
> I've retrieved 8 reports from the 'Marketing Analytics' space, including 'Campaign ROI', 'Leads by Channel', and 'Monthly Web Traffic'.

---

**👤 You:**
> "Run the report with token 'rep_12345' and check its latest status."

**🤖 AI Agent:**
> Report run has been triggered. Status is currently 'enqueued'. I'll check back in a moment to see if it has completed.

---

**👤 You:**
> "Show me the SQL query used in the 'Churn Analysis' report."

**🤖 AI Agent:**
> I've fetched the queries for that report. It uses a SELECT statement from the 'events' table joined with 'subscriptions' to calculate monthly churn rates.


## ❓ FAQ

**Q: How do I find my API Token and Secret?**
In Mode, click on your name in the top left, go to **My Account** > **API Tokens**. There you can create and manage your API keys.

**Q: What is the Workspace slug?**
The Workspace slug is the unique identifier for your organization in the Mode URL (e.g., `app.mode.com/org_name`). The `org_name` part is your workspace slug.

**Q: Can I provide parameters when running a report?**
Yes! The `run_mode_report` action accepts an optional `parameters` field where you can provide a JSON string of keys and values used by the report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mode-analytics](https://vinkius.com/mcp/mode-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mode Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mode-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mode Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mode-analytics": {
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
