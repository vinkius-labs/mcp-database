# journy.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/journyio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage SaaS growth, users, and accounts via journy.io API.

## Description
Empower your AI agents with journy.io's SaaS growth platform. This MCP server allows you to list and retrieve users and accounts, track events, manage audience segments, and view growth goals directly through the journy.io API. Ideal for automating customer success and growth marketing workflows.


## Available Tools (10)
- **get_account**: Use this to understand the status and lifecycle of a specific business customer.

Retrieves details for a specific account
- **get_me**: Use for system authentication verification.

Gets details about your own authenticated API identity
- **get_user**: Includes custom properties, event history summary, and account associations. Use this for deep intelligence on a specific user before an interaction.

Retrieves details for a specific user
- **list_accounts**: Includes account health metrics and identifiers. Use this to provide a business-level overview of the customer base.

Lists all accounts (companies) tracked in journy.io
- **list_campaigns**: Use to analyze which campaigns are successfully driving high-value users.

Lists all tracked marketing campaigns
- **list_events**: g., "Logged In", "Plan Upgraded"). Use this to understand user behavior patterns and active features.

Lists all tracked events
- **list_goals**: Use this to track progress toward business objectives like user activation or retention.

Lists all growth goals configured in journy.io
- **list_properties**: Use this to understand what metadata is available for users and accounts (e.g., "industry", "setup_wizard_completed").

Lists all defined properties for users and accounts
- **list_segments**: g., "Churn Risk", "Power Users"). Useful for identifying cohorts for targeted growth actions.

Lists all defined audience segments
- **list_users**: Returns user IDs, names, and health scores. Use this to identify key individuals for growth analysis or success management.

Lists all users tracked in journy.io


## 💬 Prompt Examples

Here are some examples of how you can interact with the **journy.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active users in journy.io."

**🤖 AI Agent:**
> I'll fetch the list of users currently tracked in your journy.io account.

---

**👤 You:**
> "Show me the details for account ID '456'."

**🤖 AI Agent:**
> I'll retrieve the full profile and health metrics for that specific account.

---

**👤 You:**
> "Check recent tracked events."

**🤖 AI Agent:**
> I'll look up the latest interactions and events captured by journy.io.


## ❓ FAQ

**Q: How do I get journy.io API credentials?**
Log in to your journy.io account, navigate to Settings > API, and find your API Key.

**Q: Can I see user properties?**
Yes, the list_properties and get_user tools allow you to retrieve all data points associated with your tracked users.

**Q: Does it support event tracking?**
Yes, you can list tracked events using the list_events tool to monitor user interactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/journyio](https://vinkius.com/mcp/journyio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **journy.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `journyio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **journy.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "journyio": {
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
