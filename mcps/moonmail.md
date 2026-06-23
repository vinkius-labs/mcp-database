# MoonMail MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moonmail)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing via MoonMail — track campaigns, subscriber lists, and engagement directly from your AI agent.

## Description
Connect your **MoonMail** account to your AI agent and optimize your email marketing operations through natural conversation.

### What you can do

- **Campaign Management** — List all email campaigns, create new ones, and trigger delivery to your audience.
- **Subscriber Growth** — Access your subscriber lists, add new contacts, and manage audience segments.
- **Engagement Insights** — Monitor real-time performance metrics (opens, clicks) and tracking events for your campaigns.
- **Recipients Tracking** — Fetch the list of all individual recipients for specific campaign IDs.
- **List Oversight** — View all mailing lists and their current subscriber counts to stay organized.

### How it works

1. Subscribe to this server
2. Enter your MoonMail API Key
3. Start managing your newsletters from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketers** — quickly check how a recent campaign is performing or add a new subscriber.
- **Content Creators** — initialize and send new campaigns directly from your chat.
- **Growth Teams** — automate subscriber additions and monitor analytics events in real-time.


## Available Tools (10)
- **add_subscriber**: Add a subscriber to a list
- **create_campaign**: Create a new email campaign
- **get_campaign_stats**: Get campaign performance metrics
- **get_events**: Get email analytics events
- **list_campaign_recipients**: List recipients of a campaign
- **list_campaigns**: List MoonMail campaigns
- **list_subscribers**: List members of a list
- **list_lists**: List subscriber lists
- **list_segments**: List audience segments
- **send_campaign**: Send an email campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MoonMail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email campaigns and their status."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 4 active campaigns: 'Weekly Newsletter' (Status: Sent), 'Summer Promo' (Status: Draft), and 2 others. Would you like to see the engagement stats for the Weekly Newsletter?

---

**👤 You:**
> "How is my 'New Feature Announcement' campaign performing?"

**🤖 AI Agent:**
> Fetching stats for 'New Feature Announcement' (ID: cmp_123)... The campaign has a 32% open rate and a 5.4% click-through rate so far. Would you like to see the list of recipients who clicked the primary link?

---

**👤 You:**
> "Add alex@example.com to the 'VIP Customers' list."

**🤖 AI Agent:**
> Subscribing contact... I've successfully added alex@example.com to your 'VIP Customers' list (ID: lst_987). They are now ready to receive future campaigns sent to this list.


## ❓ FAQ

**Q: How do I get a MoonMail API Key?**
Log in to MoonMail and navigate to Settings > API Keys to generate your key. This token is required for all API operations.

**Q: Can I send a campaign through this server?**
Yes! Use the `send_campaign` tool with a valid Campaign ID to trigger the delivery process.

**Q: How do I see how many people opened my email?**
Use the `get_campaign_stats` tool with the Campaign ID to retrieve the open rate, click rate, and other engagement metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moonmail](https://vinkius.com/mcp/moonmail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MoonMail** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moonmail` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MoonMail** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moonmail": {
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
