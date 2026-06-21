# Jiguang Aurora / 极光 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jiguang-aurora)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Dominant push notification platform in China — manage device segments, schedules, and delivery reports via AI.

## Description
Empower your AI agent to orchestrate your push notification infrastructure with **Jiguang Aurora** (极光), the premier CPaaS provider in China. By connecting Jiguang to your agent, you transform complex device targeting, scheduled messaging, and multi-platform delivery into a natural conversation. Your agent can instantly send targeted push notifications, retrieve detailed device metadata by Registration ID, manage complex delivery schedules, and audit real-time message reports without you ever needing to navigate the comprehensive Jiguang portal. Whether you are automating user verification or coordinating large-scale promotional alerts, your agent acts as a real-time messaging assistant, keeping your communication flow accurate and your users informed.

### What you can do

- **Push Orchestration** — Send customized push notifications to specific users or segments with full support for deep-linking.
- **Device Management** — Retrieve detailed metadata for specific devices and update tags or aliases to refine your targeting.
- **Schedule Control** — Create and manage scheduled push tasks to ensure your messages reach users at the perfect moment.
- **Delivery Auditing** — Access real-time reports for message receipt and user engagement metrics.
- **Operational Insights** — Monitor your account quota and API usage limits to ensure system-wide communication health.

### How it works

1. Subscribe to this server
2. Enter your Jiguang App Key and Master Secret
3. Start managing your push infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Operations** — automate system notifications and monitor delivery status through natural language queries.
- **Marketing Leads** — coordinate scheduled campaigns and audit user behavior directly from your AI-powered workspace.
- **DevOps Engineers** — monitor API quotas and system communication health via a unified AI interface.
- **Jiguang Power Users** — integrate your existing push workflows into your AI-driven daily routines.


## Available Tools (10)
- **create_schedule**: Create a scheduled push
- **delete_schedule**: Delete a scheduled task
- **get_account_quota**: Get API quota and usage
- **get_device_info**: Get device information
- **get_message_status**: Get detailed message status
- **get_push_report**: Get push delivery report
- **get_user_report**: Get user activity report
- **list_schedules**: List scheduled push tasks
- **send_push**: Send push notification
- **update_device**: Update device tags and alias


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jiguang Aurora / 极光** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a push notification to Registration ID '1a0918c...'."

**🤖 AI Agent:**
> I've sent the targeted push notification to the specified device. The message ID is '8821'. Would you like me to check the delivery status in a few minutes?

---

**👤 You:**
> "Schedule a push task for tomorrow at 10 AM."

**🤖 AI Agent:**
> Done! I've created a scheduled push task. It is set to trigger tomorrow at 10:00 AM. You can find this task in your schedule list with ID '9920'.

---

**👤 You:**
> "Show me the user activity report for the last 7 days."

**🤖 AI Agent:**
> I've retrieved the user activity report. Over the last 7 days, you had an average of 12,500 daily active users and 450 new device registrations. Should I break this down by platform (iOS/Android)?


## ❓ FAQ

**Q: How do I find my Jiguang App Key and Master Secret?**
Log in to the [Jiguang portal](https://www.jiguang.cn/), create an application, and you will find your App Key and Master Secret in the application overview or settings section.

**Q: Can I target specific users with an alias?**
Yes. Jiguang allows you to set an 'alias' for each device. You can then use the `send_push` tool with that alias in the audience payload to send targeted notifications to specific individuals.

**Q: Is it possible to track if a message was received?**
Yes! Use the `get_push_report` tool with your message IDs to retrieve delivery statistics, including the count of devices that successfully received the notification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jiguang-aurora](https://vinkius.com/mcp/jiguang-aurora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jiguang Aurora / 极光** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jiguang-aurora` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jiguang Aurora / 极光** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jiguang-aurora": {
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
