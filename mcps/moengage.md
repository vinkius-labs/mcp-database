# MoEngage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moengage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Engage mobile app users with personalized push notifications, in-app messages, and AI-optimized customer journeys across channels.

## Description
Connect your **MoEngage** account to any AI agent and manage customer engagement through natural conversation.

### What you can do

- **User Management** — Create/update user attributes and device data
- **Event Tracking** — Track custom user events and behaviors
- **Push Notifications** — Trigger transactional and marketing push messages
- **Campaign Management** — Launch and pause multi-channel campaigns
- **Analytics** — Retrieve campaign performance and user statistics

### How it works

1. Subscribe to this server
2. Enter your MoEngage Workspace ID and API Key
3. Start managing customer engagement from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketers** — orchestrate omnichannel campaigns
- **Product Teams** — track user behavior and engagement
- **Developers** — integrate server-side events and push notifications


## Available Tools (13)
- **list_campaigns**: List campaigns
- **check_moengage_status**: Verify connectivity
- **get_campaign_stats**: Get campaign stats
- **get_campaign**: Get campaign details
- **get_customer**: Get customer details
- **get_segment**: Get segment details
- **list_segments**: List segments
- **search_customers**: Search customers
- **send_push**: Send push notification
- **track_events_bulk**: Track events in bulk
- **track_event**: Track an event
- **update_device**: Update device info
- **upsert_customer**: Create or update customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MoEngage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show performance for the 'Spring Sale Push' campaign."

**🤖 AI Agent:**
> Campaign Analytics: 'Spring Sale Push'. Sent: 145,000. Delivered: 142,500 (98%). Clicks: 12,400 (8.7% CTR ⭐). Conversions: 3,200 Purchases ($45K revenue). Uninstalls attributed: 12.

---

**👤 You:**
> "Send a transactional push notification to user 8901."

**🤖 AI Agent:**
> Push notification sent! ✅ Target: User_8901. Title: 'Order Shipped 📦'. Message: 'Your order #1234 is on the way!'. Platform: iOS. Status: Success (Delivered to 1 device).

---

**👤 You:**
> "Track a 'Subscription Upgraded' event for user Sarah."

**🤖 AI Agent:**
> Event tracked! ✅ User ID: sarah@company.com. Event: 'Subscription Upgraded'. Properties: {plan: 'Pro', amount: 45.00, platform: 'Web'}. Profile updated successfully.


## ❓ FAQ

**Q: Can I trigger push notifications?**
Yes. Trigger personalized push notifications via the Transactional API to specific users or segments.

**Q: How does MoEngage authentication work?**
MoEngage uses HTTP Basic Auth using your **Workspace ID** and **API Key** against `api-01.moengage.com/v1` (adjust region if needed).

**Q: Can I track server-side user events?**
Yes. Post custom events (e.g., Purchase, Signup) directly to user profiles for segmentation and campaigns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moengage](https://vinkius.com/mcp/moengage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MoEngage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moengage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MoEngage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moengage": {
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
