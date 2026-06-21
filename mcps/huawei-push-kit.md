# Huawei Push Kit / 华为推送服务 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/huawei-push-kit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Huawei's essential device push platform — send notifications to HMS devices via AI.

## Description
Empower your AI agent to orchestrate your device communication and mobile engagement with **Huawei Push Kit** (华为推送服务), the essential notification layer for the Huawei Mobile Services (HMS) ecosystem. By connecting Huawei Push to your agent, you transform complex message sending, topic orchestration, and conditional targeting into a natural conversation. Your agent can instantly send high-priority notifications to specific tokens, broadcast updates to millions of topic subscribers, and manage complex boolean conditions for precise targeting without you ever needing to navigate the comprehensive AppGallery Connect console. Whether you are automating system alerts or coordinating a global marketing update, your agent acts as a real-time push coordinator, providing accurate and fast results from a single, authorized source.

### What you can do

- **Targeted Orchestration** — Send notifications directly to unique device tokens with custom data payloads.
- **Topic Broadcasting** — Reach massive audiences by pushing messages to specific HMS topics.
- **Conditional Targeting** — Execute precise notification flows based on complex topic combinations.
- **Operational Discovery** — Verify token formats, check topic compliance, and monitor API connectivity.
- **System Management** — Verify your configured App ID and automate system update notifications.

### How it works

1. Subscribe to this server
2. Enter your Huawei HMS App ID and App Secret
3. Start managing your device communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & Backend Engineers** — automate system alerts and monitor push delivery health through natural language.
- **Growth & Marketing Teams** — coordinate global update broadcasts and target specific user segments directly from your workspace.
- **Developers** — integrate professional-grade HMS push capabilities into your AI-driven daily routines.
- **Huawei Cloud Power Users** — integrate your existing HMS workflows into your AI-driven daily routines.


## Available Tools
- **list_topic_subscriptions**: List topics a device is subscribed to
- **push_to_condition**: Example: "'topicA' in topics && 'topicB' in topics".

Send push notification based on topic conditions
- **push_to_token**: Requires the device push token.

Send push notification to a device token
- **push_to_topic**: Send push notification to a topic
- **subscribe_to_topic**: Subscribe device tokens to a topic
- **unsubscribe_from_topic**: Unsubscribe device tokens from a topic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Huawei Push Kit / 华为推送服务** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a push notification to token 'ABCD...1234' with title 'Good Morning' and body 'Don't forget your tasks today'."

**🤖 AI Agent:**
> I've successfully sent the notification to the device token. The Huawei request ID is `1234567890`. Should I also send this update to your global announcement topic?

---

**👤 You:**
> "Broadcast a system update notification to the 'all_users' topic for version '2.5.0'."

**🤖 AI Agent:**
> I've initiated the broadcast to all devices subscribed to the `all_users` topic. The message 'Version 2.5.0 is now ready for download' has been successfully submitted to Huawei Push Kit. Would you like me to monitor the delivery status?

---

**👤 You:**
> "Check the connectivity status of our Huawei Push and OAuth gateways."

**🤖 AI Agent:**
> I've performed a diagnostic check. Both the Huawei OAuth authentication gateway and the Push Kit API are responding normally. Your App ID is correctly configured. Is there anything else you'd like to audit?


## ❓ FAQ

**Q: How do I find my Huawei HMS App ID and Secret?**
Log in to the [Huawei AppGallery Connect console](https://developer.huawei.com/consumer/en/service/josp/agc/index.html), select your project and app, and navigate to [Project Settings] -> [General Information] to find your App ID and App Secret.

**Q: Does this server handle OAuth 2.0 token management?**
Yes! The server automatically retrieves and caches the required access_token using your App Secret. It handles periodic refreshes silently, so you can focus on sending notifications.

**Q: Can I target specific user segments with conditions?**
Yes! Use the `push_to_condition` tool. You can define boolean logic expressions involving topics, such as "'news' in topics && 'sport' in topics", to target highly specific audiences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/huawei-push-kit](https://vinkius.com/mcp/huawei-push-kit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Huawei Push Kit / 华为推送服务** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `huawei-push-kit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Huawei Push Kit / 华为推送服务** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "huawei-push-kit": {
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
