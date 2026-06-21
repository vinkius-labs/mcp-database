# Zapier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zapier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Monitor automated workflows, audit app connections, and search for Zap templates on Zapier — the leader in AI orchestration.

## Description
Connect your **Zapier** account to any AI agent and manage your automation infrastructure through natural conversation.

### What you can do

- **Workflow Monitoring** — List all Zaps in your account and retrieve deep details including triggers, actions, and current live status
- **Execution Auditing** — Retrieve the job history for any specific Zap to monitor recent runs and check for task successes or failures
- **App Connectivity** — List all third-party applications (e.g., Slack, Gmail, Salesforce) currently authenticated and available for your automations
- **Template Discovery** — Search the Zapier directory for pre-made workflow ideas by providing queries like 'Slack to Trello'
- **Account Insights** — Verify your authenticated user profile, plan limits, and account ownership directly from your agent
- **Deep Discovery** — Quickly find unique Zap and App IDs required for advanced automation management and reporting
- **Status Verification** — Monitor whether your Zaps are turned on or off to ensure your critical business workflows are operational

### How it works

1. Subscribe to this server
2. Enter your Zapier API Key
3. Start monitoring your Zaps and connections through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex automation dashboards to check if a workflow is running. Your AI agent becomes your automation analyst.

### Who is this for?

- **Automation Engineers** — monitor Zap performance and audit execution history through simple chat commands
- **Operations Teams** — verify connected app health and manage workflow statuses without manual navigation
- **Product Owners** — quickly surface automation templates and verify connectivity for strategic integration planning
- **Support Teams** — lookup Zap details and history to troubleshoot integration issues rapidly


## Available Tools
- **get_zap**: Retrieves comprehensive configuration for a specific Zap
- **list_apps**: g. Slack, Gmail) are authenticated and available for automation.

Lists all third-party applications currently connected to the Zapier account
- **get_profile**: Retrieves details about the authenticated Zapier user and account
- **search_templates**: Provide a query string like "Slack to Trello".

Searches the Zapier directory for pre-made workflow templates
- **list_zaps**: Lists all Zaps (automated workflows) in the Zapier account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zapier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Zaps in Zapier."

**🤖 AI Agent:**
> I found 5 Zaps in your account: 1. 'New Lead to Slack' (Status: ON, ID: 12345), 2. 'Shopify to Xero Sync' (Status: ON, ID: 67890), 3. 'Email to Trello' (Status: OFF, ID: 11223), and 2 others. Which one would you like to audit?

---

**👤 You:**
> "What is the history for the 'New Lead to Slack' Zap?"

**🤖 AI Agent:**
> Retrieving history for Zap 12345… The last 5 runs were all successful. The most recent execution was 10 minutes ago and successfully sent a lead notification to the #sales-alerts channel.

---

**👤 You:**
> "Search for templates to sync Gmail attachments to Dropbox."

**🤖 AI Agent:**
> I found several templates for Gmail to Dropbox sync. Popular options: 1. 'Save new Gmail attachments to a specific Dropbox folder', 2. 'Create Dropbox text files from new Gmail emails'. Would you like the details for these templates?


## ❓ FAQ

**Q: Can I check if a specific Zap failed recently through the agent?**
Yes. The `get_zap_history` tool allows your AI agent to retrieve the job history for any specific Zap ID, showing you which runs succeeded and which encountered task failures so you can monitor health through chat.

**Q: How do I find out which third-party apps are connected to my account?**
You can use the `list_connected_apps` tool. It will return all applications currently authenticated in your Zapier account, such as Slack, Google Sheets, or Gmail, so you can see what is available for automation.

**Q: Is it possible to search for workflow ideas via conversation?**
Absolutely. Use the `search_zap_templates` tool and provide a query string. Your agent will search the Zapier directory and return pre-made template ideas to help you build new automated flows quickly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zapier](https://vinkius.com/mcp/zapier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zapier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zapier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zapier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zapier": {
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
