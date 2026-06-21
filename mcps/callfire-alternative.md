# CallFire MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/callfire-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Run voice broadcasts, send bulk text messages, and manage call tracking campaigns for high-volume outreach at scale.

## Description
Connect your **CallFire** account to any AI agent and manage your voice and SMS communication workflows through natural conversation.

### What you can do

- **Contact Management** — List all contacts and retrieve individual contact profiles with phone numbers and metadata
- **Call Tracking** — Browse all inbound and outbound calls with duration, status, and call recording details
- **SMS History** — Review sent and received text messages with delivery status and timestamps
- **Campaign Monitoring** — List all broadcast campaigns (voice and text) and inspect individual campaign configurations and performance
- **Webhook Management** — View all configured webhooks and inspect their delivery settings and event triggers

### How it works

1. Subscribe to this server
2. Enter your CallFire API Login (username) and API Password from your account settings
3. Start managing your communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — check call history, review SMS delivery rates, and monitor campaign reach without leaving the AI workspace
- **Marketing Operations** — monitor broadcast campaign performance and contact engagement metrics
- **Customer Support** — quickly search for calls and messages by contact ID for case investigation


## Available Tools
- **get_call**: Get a specific call
- **get_campaign**: Get a specific broadcast campaign
- **get_contact**: Get a specific contact
- **get_text**: Get a specific text message
- **get_webhook**: Get a specific webhook
- **list_calls**: List all calls
- **list_campaigns**: List all broadcast campaigns
- **list_contacts**: List all contacts
- **list_texts**: List all text messages
- **list_webhooks**: List all webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CallFire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active broadcast campaigns and their delivery rates."

**🤖 AI Agent:**
> You have 3 active campaigns. 1) 'Spring Promo SMS' (campaign_4201) — 12,400 messages sent, 98.2% delivery rate, 340 replies received. 2) 'Appointment Reminders' (campaign_4189) — 3,200 calls completed, 67% answered. 3) 'Survey Follow-up' (campaign_4195) — 1,800 texts sent, 94% delivered. Would you like to inspect a specific campaign or check the associated webhooks?

---

**👤 You:**
> "List all text messages sent in the last 24 hours and highlight any that failed delivery."

**🤖 AI Agent:**
> Retrieved 847 text messages in the last 24 hours. Delivery breakdown: 812 delivered (95.8%), 28 pending (3.3%), 7 failed (0.8%). Failed messages: 3 to invalid numbers (text_90112, text_90178, text_90234), 2 carrier-blocked (text_90301, text_90445), 2 opt-out recipients (text_90389, text_90501). Would you like to inspect the full content of any failed message?

---

**👤 You:**
> "How many contacts do I have and are there any with missing phone numbers?"

**🤖 AI Agent:**
> You have 4,231 contacts total. 4,189 have valid phone numbers (99.0%). 42 contacts are missing phone numbers — these were imported from a CSV on March 15. The top 5 contacts by interaction volume: 'Apex Industries' (contact_8901, 47 calls), 'Green Valley Corp' (contact_8234, 38 calls), and 'Metro Health' (contact_7912, 31 calls). Would you like to view details for any contact?


## ❓ FAQ

**Q: Can I review the full history of calls and text messages for a specific contact?**
Yes. Use `list_calls` to browse all call records and `get_call` with a specific Call ID for full details including duration, recording URL, and disposition. For SMS, use `list_texts` to browse messages and `get_text` for individual message content and delivery status.

**Q: Does CallFire require two separate credentials?**
Yes. CallFire uses HTTP Basic Authentication with an **API Login** (username) and an **API Password**. Both are generated in your CallFire account under Settings > API Access. They are separate from your dashboard login credentials.

**Q: Can I monitor my active broadcast campaigns and their delivery status?**
Yes. The `list_campaigns` tool retrieves all voice and text broadcast campaigns with their status (active, paused, finished). Use `get_campaign` with a Campaign ID to inspect configuration details, delivery rates, and audience targeting. Combine with `list_webhooks` to verify event-driven notifications are configured correctly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/callfire-alternative](https://vinkius.com/mcp/callfire-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CallFire** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `callfire-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CallFire** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "callfire-alternative": {
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
