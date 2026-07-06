# Freshsuccess MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshsuccess)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Manage customer success, track health scores, and oversee account usage via AI agents with Freshsuccess.

## Description
Connect your **Freshsuccess** (Freshdesk Customer Success) account to any AI agent to automate your customer retention and engagement operations through the Model Context Protocol (MCP). Freshsuccess empowers Customer Success Managers (CSMs) to prevent churn, increase expansion revenue, and proactively manage accounts. This MCP server enables you to track health scores, update user metadata, and log custom metrics directly through natural conversation.

### Key Features

- **Account Oversight** — List all customer accounts, retrieve detailed profiles including health scores, and map assigned CSMs instantly.
- **User & Engagement Tracking** — Access detailed end-user profiles, monitor product usage, and upsert records to ensure accurate data.
- **Proactive Alerts** — Monitor configured customer success alerts (e.g., drop in usage, poor health) to prioritize interventions.
- **Task Management** — Retrieve pending CSM tasks and to-dos to keep your team aligned on retention efforts.
- **Custom Metric Logging** — Post specific product usage values or custom metrics directly to accounts and users to influence health scoring.
- **Data Synchronization** — Ensure your CRM and CS platforms are perfectly aligned by automating record updates.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freshsuccess Region Domain and API Key (found in your Settings)
3. Start managing your customer success data from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Success Managers** — quickly check account health scores or active alerts without navigating the dashboard.
- **CS Operations** — automate the logging of custom metrics and verify user mappings via simple AI commands.
- **Account Executives** — get a real-time overview of customer adoption before renewal conversations.


## Available Tools (11)
- **get_account_health**: Get account metadata
- **get_user_health**: Get user metadata
- **list_cs_accounts**: List customer accounts
- **list_cs_alerts**: g. drop in usage).

List active alerts
- **list_custom_metrics**: List defined metrics
- **list_cs_tasks**: List pending tasks
- **list_cs_users**: List account users
- **post_metric_value**: Record custom metric
- **upsert_cs_account**: Create/Update account
- **upsert_cs_user**: Create/Update user
- **check_api_status**: Verify API connection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshsuccess** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active customer success alerts."

**🤖 AI Agent:**
> Retrieving alerts... I found 3 active alerts, including a 'Drop in Login Frequency' for Acme Corp and a 'Support Ticket Spike' for Globex.

---

**👤 You:**
> "Show me the health score for account 'acc_123'."

**🤖 AI Agent:**
> Fetching account health... Account 'acc_123' (Example Inc.) currently has a Health Score of 85 (Green). They are assigned to CSM Sarah Jenkins.

---

**👤 You:**
> "Post a custom metric 'api_calls' with value 150 for user 'user_987'."

**🤖 AI Agent:**
> Metric recorded! I have successfully posted the value 150 for the 'api_calls' metric to user ID user_987. This will factor into their engagement score.


## ❓ FAQ

**Q: How do I get an API Key for Freshsuccess?**
Log in to your Freshsuccess account, navigate to Settings > Third-party integrations > API, and generate or copy your active token.

**Q: What is my 'Region Domain'?**
Your domain depends on where your account is hosted (e.g. 'api-us.freshsuccess.com' for US Data Center, 'api-eu.freshsuccess.com' for Europe).

**Q: Can I update an account's metadata using the agent?**
Yes! Use the 'upsert_cs_account' tool. Provide the unique Account ID and the new name to instantly update the record in Freshsuccess.

**Q: Is it possible to log custom product metrics?**
Absolutely. You can use the 'post_metric_value' tool to send raw numeric data for specific accounts or users to influence their health scores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshsuccess](https://vinkius.com/mcp/freshsuccess)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freshsuccess** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freshsuccess` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freshsuccess** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freshsuccess": {
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
