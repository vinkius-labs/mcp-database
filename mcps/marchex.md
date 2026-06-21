# Marchex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marchex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Marchex Conversation Intelligence — track calls, manage campaigns, and analyze performance.

## Description
Connect your **Marchex** account to any AI agent and take full control of your conversation intelligence through natural conversation.

### What you can do

- **Call Tracking** — Search for calls, fetch detailed metadata, and monitor statuses
- **Campaign Management** — List and inspect tracking campaigns and their configurations
- **Number Management** — Manage tracking phone numbers and account structures
- **Analytics** — Retrieve aggregated performance metrics and call analytics

### How it works

1. Subscribe to this server
2. Enter your Marchex Client ID and Secret
3. Start managing your conversation intelligence from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_account_details**: Get details for a specific account
- **get_call_analytics**: Get call analytics
- **get_call_details**: Get details for a specific call
- **get_campaign_details**: Get details for a specific campaign
- **get_number_details**: Get details for a specific number
- **list_accounts**: List all accounts
- **list_campaigns**: List all campaigns
- **list_numbers**: List all tracking numbers
- **list_users**: List all users
- **search_calls**: Search for phone calls


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marchex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for calls from last week."

**🤖 AI Agent:**
> Fetching call records... I found 15 calls. Notable entries include calls from +1234567890 with durations around 2 minutes.

---

**👤 You:**
> "List active tracking campaigns."

**🤖 AI Agent:**
> Querying campaigns... You have 3 active campaigns: 'Spring Sale', 'Google Ads', and 'Facebook Ads'.

---

**👤 You:**
> "Show call analytics for today."

**🤖 AI Agent:**
> Calculating analytics... Today you had 50 total calls with an average duration of 3m 45s.


## ❓ FAQ

**Q: How do I find my Marchex Client ID and Secret?**
Log in to the Marchex Developer Console and create an application to receive your credentials.

**Q: What call data can I access?**
You can access call metadata, duration, caller info, status, and aggregated performance metrics.

**Q: Is my integration secure?**
Absolutely. Your credentials are encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marchex](https://vinkius.com/mcp/marchex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marchex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `marchex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marchex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marchex": {
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
