# Mention MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mention)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Social media monitoring and alerts via Mention — track mentions and monitor brand sentiment.

## Description
Connect your **Mention** account to any AI agent and take full control of your social monitoring and brand alerts through natural conversation.

### What you can do

- **Alert Management** — List all active monitoring alerts and fetch detailed configuration metadata
- **Mention Tracking** — Retrieve recent social media mentions, filter for favorites, and search by text
- **Deep Inspection** — Fetch full content, metadata, and sentiment analysis for specific mentions
- **Brand Analytics** — Access volume and sentiment statistics for your monitoring alerts instantly
- **Account Visibility** — List authorized users and connected external social media accounts

### How it works

1. Subscribe to this server
2. Enter your Mention Access Token and Account ID
3. Start monitoring your brand from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_account_info**: Get account information
- **get_alert**: Get details for a specific alert
- **get_alert_statistics**: Get statistics for an alert
- **get_mention_details**: Get details for a specific mention
- **list_account_users**: List users associated with the account
- **list_alerts**: List all monitoring alerts
- **list_connected_external_accounts**: ) linked.

List connected social accounts
- **list_favorite_mentions**: List favorite mentions for an alert
- **list_mentions**: List mentions for an alert
- **search_mentions**: Search mentions by text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mention** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active alerts in my Mention account."

**🤖 AI Agent:**
> Retrieving alerts... I found 3 active alerts including 'Brand Monitor', 'Competitor A', and 'Industry Trends'.

---

**👤 You:**
> "Search mentions for 'artificial intelligence' in alert ID 123."

**🤖 AI Agent:**
> Searching mentions... I found 5 recent posts mentioning AI in your brand alert stream.

---

**👤 You:**
> "Show volume statistics for my primary brand alert."

**🤖 AI Agent:**
> Calculating statistics... You had 150 mentions today, a 10% increase compared to yesterday.


## ❓ FAQ

**Q: How do I find my Mention Access Token and Account ID?**
Log in to Mention, navigate to Developer settings to generate a Personal Access Token. Your Account ID is shown in your account settings.

**Q: What social platforms are monitored?**
Mention monitors news, blogs, forums, Twitter, Instagram, Facebook, and various other web sources.

**Q: Is my monitoring data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mention](https://vinkius.com/mcp/mention)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mention** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mention` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mention** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mention": {
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
