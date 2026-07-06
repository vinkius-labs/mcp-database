# ntfy (Push Notifications) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ntfy-push-notifications)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Send and receive push notifications via ntfy topics directly from your AI agent to any device.

## Description
Connect your **ntfy** instance to any AI agent and manage real-time alerts and notifications through natural conversation. ntfy is an HTTP-based pub-sub service that allows you to send notifications to your phone or desktop via scripts or APIs.

### What you can do

- **Instant Publishing** — Send messages to any ntfy topic with custom titles, priorities, and tags (emojis).
- **Message Polling** — Retrieve cached messages from a topic to stay updated on previous alerts or system logs.
- **Rich Notifications** — Attach clickable URLs, custom icons, and even files to your push notifications.
- **Scheduled Alerts** — Use the delay parameter to schedule notifications for the future.
- **Advanced Formatting** — Send notifications with Markdown support for better readability on supported clients.

### How it works

1. Subscribe to this server
2. Enter your ntfy instance URL (e.g., `https://ntfy.sh`) and an optional access token
3. Start sending alerts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — Automate deployment alerts and system monitoring notifications directly from the terminal or IDE.
- **Developers** — Send debugging info or long-running task completions to your phone.
- **Power Users** — Create custom workflows that bridge AI agents with mobile push notifications without complex setups.


## Available Tools (2)
- **publish_message**: Topics are created on the fly.

Publish a push notification to a ntfy topic
- **poll_messages**: Poll cached messages from a ntfy topic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ntfy (Push Notifications)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a high priority notification to the 'server-alerts' topic saying 'Database backup completed successfully' with a checkmark tag."

**🤖 AI Agent:**
> I've published the message to the 'server-alerts' topic with priority 4 and the 'white_check_mark' tag. The notification has been sent successfully.

---

**👤 You:**
> "Poll the last 5 minutes of messages from the 'dev-updates' topic."

**🤖 AI Agent:**
> I've retrieved the cached messages for 'dev-updates' from the last 5 minutes. I found 2 messages: 'Build #402 started' and 'Build #402 finished'.

---

**👤 You:**
> "Schedule a notification to the 'reminders' topic in 1 hour saying 'Time for the standup meeting!'."

**🤖 AI Agent:**
> I've scheduled your notification for the 'reminders' topic. It will be delivered in approximately 1 hour.


## ❓ FAQ

**Q: Can I send emojis in my notifications?**
Yes! Use the `tags` parameter in the `publish_message` tool. You can provide a comma-separated list of emojis or tags like 'warning,skull' to display them in the notification.

**Q: How do I check for messages that were sent while I was away?**
You can use the `poll_messages` tool. By specifying the `topic` and optionally the `since` parameter, you can retrieve the history of cached messages from that topic.

**Q: Does this support self-hosted ntfy instances?**
Absolutely. During setup, you can provide your custom `NTFY_URL`. If your instance requires authentication, you can also provide your `NTFY_TOKEN`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ntfy-push-notifications](https://vinkius.com/mcp/ntfy-push-notifications)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ntfy (Push Notifications)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ntfy-push-notifications` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ntfy (Push Notifications)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ntfy-push-notifications": {
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
