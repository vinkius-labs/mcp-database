# OneSignal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onesignal-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send push notifications, emails, and in-app messages to millions of users with segmentation and A/B testing built in.

## Description
Connect your **OneSignal** account to any AI agent and take full control of your customer engagement and notification orchestration through natural conversation. OneSignal is the market leader for omnichannel delivery, and this integration allows you to dispatch real-time push notifications, manage audience segments, and monitor delivery analytics directly from your chat interface.

### What you can do

- **Omnichannel Dispatch Orchestration** — Send push notifications, emails, and SMS programmatically using advanced targeting and personalized content to ensure your message always lands.
- **Audience & User Intelligence** — Manage user profiles (players), update custom tags, and retrieve detailed device metadata directly from the AI interface to maintain a high-fidelity CRM.
- **Segment & Targeting Control** — Access and monitor your audience segments and apply dynamic targeting criteria via natural language to drive better engagement.
- **Performance & Outcome Oversight** — Retrieve granular delivery analytics, track successful/failed counts, and monitor custom outcomes using simple AI commands.
- **Operational Monitoring** — Track system responses and manage multiple applications to ensure your notification pipeline is always optimized.

### How it works

1. Subscribe to this server
2. Enter your OneSignal App ID and REST API Key from your dashboard
3. Start managing your omnichannel delivery from Claude, Cursor, or any MCP-compatible client

No more manual logging to check open rates or send emergency alerts. Your AI acts as a dedicated engagement coordinator or growth operations manager.

### Who is this for?

- **Growth Marketers** — quickly send promotional alerts and monitor campaign reach without switching apps.
- **Product Managers** — automate the delivery of transactional notifications and track user re-engagement via natural conversation.
- **Operations Teams** — streamline the retrieval of player metadata and monitor system alerts directly within the chat.


## Available Tools (12)
- **cancel_scheduled_alert**: Stop notification
- **send_push_notification**: Send proactive alert
- **remove_player**: Delete device record
- **get_api_status**: Check connection
- **get_app_details**: Get application info
- **get_notification_stats**: Check delivery metrics
- **get_player_details**: Get user profile
- **list_onesignal_apps**: Requires User Auth Key.

List your applications
- **list_recent_notifications**: List past alerts
- **list_app_outcomes**: Get campaign outcomes
- **list_app_segments**: List target groups
- **list_app_players**: List subscribed devices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OneSignal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 push notifications sent from OneSignal."

**🤖 AI Agent:**
> I've retrieved your notification history. You have 5 recent broadcasts including 'Black Friday Launch' (Status: Sent) and 'App Update'. Would you like to see the click-through rates for any of them?

---

**👤 You:**
> "Send a push notification to the segment named VIP Users with a promotional message."

**🤖 AI Agent:**
> Push notification sent successfully to the "VIP Users" segment. 4,287 devices targeted across iOS (2,103) and Android (2,184). The message "Exclusive early access to our summer collection is live" was delivered with a deep link to your promotion page. Estimated delivery time: under 30 seconds.

---

**👤 You:**
> "Show me the delivery and click-through analytics for notification ID ntf_8923."

**🤖 AI Agent:**
> Notification ntf_8923 "Flash Sale Alert" was sent to 12,450 subscribers. Delivered: 11,892 (95.5%). Opened: 3,214 (27% CTR). Clicked: 1,847 (14.8% click rate). iOS performed better with 31% CTR versus Android at 24%. Peak engagement was within the first 15 minutes after delivery.


## ❓ FAQ

**Q: Can my AI automatically find the Player ID for a specific user to send a test push?**
Yes! Use the `list_users` tool. Your agent will respond with complete metadata for registered devices, including unique Player IDs and tags, allowing you to trigger targeted pushes instantly.

**Q: How do I find my OneSignal App ID and REST API Key?**
Log in to OneSignal, select your app, navigate to **Settings** > **Keys & IDs**, and you will find your unique App ID and secret REST API key there.

**Q: Can I use the AI to cancel a scheduled notification?**
Absolutely. Use the `cancel_notification` tool with the Notification ID. The agent will instruct OneSignal to stop the broadcast immediately, provided it hasn't been fully delivered yet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onesignal-alternative](https://vinkius.com/mcp/onesignal-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OneSignal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `onesignal-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OneSignal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "onesignal-alternative": {
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
