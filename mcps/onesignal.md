# OneSignal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onesignal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Automate push notifications via OneSignal — send messages, manage segments, and track delivery stats directly from any AI agent.

## Description
Connect your **OneSignal** account to any AI agent and take full control of your customer engagement workflows through natural conversation.

### What you can do

- **Notifications Management** — Send, schedule, and cancel push notifications across mobile and web platforms.
- **Audience Targeting** — Target specific segments or individual player IDs to ensure the right message reaches the right user.
- **Delivery Analytics** — Fetch detailed reports and metrics for any notification to understand your engagement levels.
- **Device Management** — List, inspect, and manage registered devices (players) within your OneSignal applications.
- **App Overview** — List all your OneSignal apps and configurations to maintain a bird's-eye view of your notification infrastructure.

### How it works

1. Subscribe to this server
2. Enter your OneSignal REST API Key and App ID
3. (Optional) Provide your User Auth Key for account-level operations
4. Start engaging your users directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — instantly send campaign alerts or schedule upcoming announcements without touching the dashboard.
- **Support Teams** — check if a specific user received a notification by inspecting their player ID metadata.
- **Developers** — test notification payloads and verify device registrations directly from your development environment.


## Available Tools
- **cancel_notification**: Cancel a scheduled notification
- **create_notification**: Send a OneSignal notification
- **delete_player**: Delete a registered device
- **get_app**: Requires User Auth Key.

Get details for a specific OneSignal app
- **get_notification**: Get specific notification status
- **get_outcomes**: Get outcome data for the app
- **get_player**: Get specific player details
- **list_apps**: Requires User Auth Key.

List all OneSignal apps
- **list_notifications**: List notifications sent for the app
- **list_players**: List registered devices (players)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OneSignal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a push notification to all subscribed users saying 'Flash Sale: 50% off today only!'"

**🤖 AI Agent:**
> Notification sent successfully! It is being delivered to the 'Subscribed Users' segment. Notification ID: 493021-abcd-1234.

---

**👤 You:**
> "Check the delivery status of notification 550e8400-e29b-41d4-a716-446655440000."

**🤖 AI Agent:**
> I've retrieved the metrics. The notification reached 1,250 devices with a 98% success rate. 25 deliveries failed due to unsubscribed users.

---

**👤 You:**
> "List the last 5 registered devices for our app."

**🤖 AI Agent:**
> I've fetched the latest device registrations. Here are the 5 most recent players, including their device types (iOS/Android) and last active timestamps.


## ❓ FAQ

**Q: Can I target specific users instead of sending to everyone?**
Yes! Use the `create_notification` tool and provide a list of `include_player_ids`. This ensures the notification is only delivered to the specific devices you've identified.

**Q: How can I check if a scheduled notification was actually sent?**
You can use the `get_notification` tool with the Notification ID. It will return real-time delivery metrics, including the number of successful deliveries and current status.

**Q: Is it possible to manage multiple OneSignal apps?**
Yes. While the core operations use the primary App ID provided in credentials, you can use `list_apps` (requires User Auth Key) to see all your applications and their respective IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onesignal](https://vinkius.com/mcp/onesignal)
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
3. Set Type to "SSE", enter `onesignal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OneSignal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "onesignal": {
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
