# Workato MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workato)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Monitor automation recipes, manage job executions, and audit app connections on Workato — the leading enterprise iPaaS platform.

## Description
Connect your **Workato** account to any AI agent and manage your enterprise integration infrastructure through natural conversation.

### What you can do

- **Recipe Monitoring** — List all automation recipes in your account and retrieve deep details including triggers, actions, and current status
- **Job Auditing** — List and monitor recent execution jobs for any specific recipe to check for errors or successful runs
- **Connection Management** — List all third-party application connections configured in your tenant and verify their current health
- **Folder Organization** — Browse your account's folder hierarchy to find where specific recipes and assets are stored
- **Connector Discovery** — List all managed connectors available in your instance to see which integration blocks are at your disposal
- **API Governance** — Retrieve all exposed API collections to see which workflows are currently accessible via REST endpoints
- **Tenant Insights** — Quickly find unique recipe, connector, and folder IDs required for advanced automation management

### How it works

1. Subscribe to this server
2. Enter your Workato API Token and Base URL (based on your region)
3. Start monitoring your automations through Claude, Cursor, or any MCP-compatible client

No more manual digging through complex iPaaS dashboards to check if a recipe ran successfully. Your AI agent becomes your automation analyst.

### Who is this for?

- **Automation Engineers** — monitor recipe performance and audit job execution history through simple chat commands
- **Operations Teams** — verify the health of app connections and manage folder structures without manual navigation
- **Product Owners** — quickly surface active API collections and available connectors for roadmap planning
- **Support Teams** — lookup recipe details and job statuses to troubleshoot integration issues rapidly


## Available Tools (7)
- **get_api_collections**: Lists all API collections exposed by Workato
- **get_recipe_details**: Retrieves details for a specific Workato recipe
- **list_app_connections**: Lists all application connections configured in Workato
- **list_managed_connectors**: Lists all managed connectors available in the tenant
- **list_workato_folders**: Lists all organizational folders in the account
- **list_recipe_jobs**: Lists recent execution jobs for a specific recipe
- **list_automation_recipes**: Lists all automation recipes in the Workato account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workato** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active recipes in my Workato account."

**🤖 AI Agent:**
> I found 8 active recipes: 1. 'Salesforce to Slack Sync' (ID: 12345), 2. 'NetSuite Invoice Automation' (ID: 67890), 3. 'Zendesk Ticket Triage' (ID: 11223), and 5 others. Which one would you like to audit?

---

**👤 You:**
> "Show me the last 5 jobs for the 'Salesforce to Slack Sync' recipe."

**🤖 AI Agent:**
> Retrieving jobs for recipe 12345… The last 5 jobs all completed successfully (Status: SUCCESS). The most recent run was 15 minutes ago and processed 12 records. No errors detected.

---

**👤 You:**
> "Are all my app connections healthy?"

**🤖 AI Agent:**
> Checking connections… Your Salesforce, Slack, and NetSuite connections are 'ACTIVE'. However, your Jira connection is 'DISCONNECTED'. Would you like me to pull the connection details to help you re-authenticate?


## ❓ FAQ

**Q: Can I check if my automations failed recently through the agent?**
Yes. The `list_recipe_jobs` tool allows your AI agent to retrieve the execution history for any recipe ID, showing you which jobs succeeded and which encountered errors so you can monitor health through chat.

**Q: How do I know if an app connection is still active?**
You can use the `list_app_connections` tool. It will return all configured connections in your Workato account along with their current status, helping you identify disconnected apps immediately.

**Q: Can I see which workflows are available as REST APIs?**
Absolutely. Use the `get_api_collections` tool to retrieve a list of all API collections exposed by your Workato tenant, showing you which recipes are ready for external invocation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workato](https://vinkius.com/mcp/workato)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Workato** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `workato` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Workato** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workato": {
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
