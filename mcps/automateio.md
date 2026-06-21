# Automate.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/automateio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage Automate.io workflows seamlessly — audit your bots, connections, and execution runs directly from your AI agent.

## Description
Connect your **Automate.io** account to any AI agent and take full control of your integration workflows and platform boundaries through natural conversation.

### What you can do

- **Bots & Workflows** — List and inspect the structural rules, triggers, and action metadata for all your automated bots
- **Execution Runs** — Trace chronological execution attempts (successes and failures) for any specific workflow endpoint
- **App Connections** — Audit explicitly attached OAuth tokens or API keys verifying connectivity to external SaaS platforms
- **Supported Apps** — Discover global metadata bounding specific applications that the underlying Automate engine natively supports
- **Usage Metrics** — Retrieve live billing usage statistics to view how many workflow executions occurred against your account quota

### How it works

1. Subscribe to this server
2. Enter your Automate.io API Key
3. Start monitoring your integration flows locally from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Integration Engineers** — debug failed execution runs remotely without needing to log blindly into the dashboard layer
- **Operations Teams** — check billing quotas and trace structural issues on critical workflows
- **IT Admins** — easily audit all connected SaaS applications and active endpoints associated with the company account


## Available Tools
- **list_bots**: List all Automate.io bots
- **get_bot**: Get explicit details of a single bot configuration
- **list_bot_runs**: List chronological execution runs for a bot
- **list_connections**: List all authorized integration app connections
- **list_apps**: List explicitly available supported integrations
- **get_usage**: Retrieve the active account billing usage statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Automate.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize my Automate.io usage numbers and check if I'm near limit."

**🤖 AI Agent:**
> I checked your account usage metadata. You've executed 8,402 workflow runs out of a 10,000 allowance for this cycle. You have approximately 15% quota remaining before the next reset period in 5 days.

---

**👤 You:**
> "List the last 5 execution logs for the 'Slack to CRM' bot."

**🤖 AI Agent:**
> I queried bot execution chronologies. The last 4 runs succeeded seamlessly, moving contacts correctly. However, the exact run from 2:00 PM failed: `API Token Expired` from the destination CRM endpoint.

---

**👤 You:**
> "Audit our external SaaS connections currently attached to Automate."

**🤖 AI Agent:**
> I found 4 existing connections securely mapped inside your account: 1. Salesforce (OAuth active) 2. Slack (OAuth active) 3. Google Sheets (OAuth degraded warning) 4. Mailchimp (API Key). I recommend refreshing the Google Sheets token immediately.


## ❓ FAQ

**Q: Can I diagnose why a specific Automate.io bot failed recently?**
Yes. Grab the Bot ID and ask your agent to list its recent execution runs. The agent fetches chronological logs highlighting success status and precise internal failures, saving you endless clicks on the dashboard log pages.

**Q: Can I check my quota limit proactively using my AI Agent?**
Absolutely. You can request your current usage statistics at any moment. Your agent checks raw configurations against execution quotas so you can anticipate upgrades before critical workflows freeze unexpectedly.

**Q: Is it possible to list which explicit apps my organization has connected?**
Yes. The list connections tool will surface every external SaaS platform that has an attached OAuth token or active API Key inside your Automate.io environment. Essential tool to trace orphaned security keys across integrations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/automateio](https://vinkius.com/mcp/automateio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Automate.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `automateio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Automate.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "automateio": {
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
