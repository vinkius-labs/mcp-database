# Omnisend Marketing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/omnisend-marketing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage omnichannel marketing via Omnisend — track email/SMS campaigns, contacts, and segments directly from your AI agent.

## Description
Connect your **Omnisend** account to your AI agent and streamline your email, SMS, and omnichannel marketing operations through natural conversation.

### What you can do

- **Campaign Management** — List all email and SMS campaigns and retrieve detailed performance and scheduling metadata.
- **Audience Oversight** — Access customer profiles, subscription statuses, and audience segment associations.
- **Segment Intelligence** — List saved audience segments and retrieve member counts for granular targeting.
- **Event Tracking** — Monitor custom tracking events triggered by your customers across their journey.
- **Form Monitoring** — View active and draft signup and popup forms configured in your account.
- **Order Data** — Access a history of e-commerce orders synced to your Omnisend audience.
- **Account Usage** — Check current billing and usage metrics, including email and SMS volumes.
- **Deep Inspection** — Fetch complete metadata for specific campaigns, contacts, or segments using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Omnisend API Key
3. Start managing your omnichannel marketing from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Marketers** — quickly check campaign statuses or audience segment sizes without opening the dashboard.
- **Growth Teams** — monitor custom event triggers and conversion data in real-time.
- **Marketing Operations** — automate the retrieval of usage metrics and order history for reporting.


## Available Tools
- **get_campaign_details**: Get specific campaign info
- **get_contact_details**: Get specific contact info
- **get_segment_details**: Get specific segment info
- **get_account_usage**: g. email/SMS volume).

Get account usage metrics
- **list_campaigns**: List marketing campaigns
- **list_contacts**: List marketing contacts
- **list_custom_events**: List custom tracking events
- **list_signup_forms**: List signup and popup forms
- **list_ecommerce_orders**: List e-commerce orders
- **list_audience_segments**: List audience segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Omnisend Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active email and SMS campaigns."

**🤖 AI Agent:**
> Retrieving campaigns... I found 10 active campaigns including 'Abandoned Cart SMS', 'Welcome Email Series', and 'Spring Clearance'. Would you like the details for the Abandoned Cart campaign?

---

**👤 You:**
> "How many members are in the 'VIP Customers' segment?"

**🤖 AI Agent:**
> Fetching segment info... The 'VIP Customers' segment currently has 2,450 active members. Shall I retrieve the detailed metadata for this segment?

---

**👤 You:**
> "Show me our account usage for this month."

**🤖 AI Agent:**
> Retrieving usage metrics... This month you have sent 45,000 emails and 1,200 SMS messages. You are currently at 75% of your monthly email volume limit. Would you like to see the upcoming scheduled campaigns?


## ❓ FAQ

**Q: How do I get an Omnisend API Key?**
Log in to your Omnisend account and navigate to Store Settings > API keys to create and retrieve your API key.

**Q: Can I see campaign performance metrics?**
Yes! Use the `get_campaign_details` tool with a specific campaign ID to retrieve metadata including high-level results and scheduling info.

**Q: Does this support SMS campaign tracking?**
Yes, the `list_campaigns` tool retrieves both email and SMS campaigns defined in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/omnisend-marketing](https://vinkius.com/mcp/omnisend-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Omnisend Marketing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `omnisend-marketing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Omnisend Marketing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "omnisend-marketing": {
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
