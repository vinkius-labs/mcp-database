# MagicBell MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/magicbell)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage notifications and broadcasts via MagicBell — list, retrieve, and trigger multi-channel alerts directly from your AI agent.

## Description
Connect your **MagicBell** project to any AI agent to orchestrate multi-channel notification workflows. Trigger broadcasts, check delivery status, and manage communication logs through natural conversation.

### What you can do

- **Broadcast Management** — List all active and past broadcasts sent through your project to track communication history.
- **Detailed Inspection** — Fetch specific broadcast metadata, content, and processing status using unique UUIDs.
- **Trigger Notifications** — Create and send new broadcasts with custom titles, body content, and specific recipient filters.
- **Multi-channel Control** — Handle channel-specific overrides for email, SMS, and push notifications to ensure the right message reaches the right place.

### How it works

1. Subscribe to this server
2. Enter your MagicBell Project JWT
3. Start sending and monitoring notifications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — trigger system-wide announcements or feature updates without touching the technical dashboard.
- **Support & Ops Teams** — quickly verify if a specific broadcast was successfully processed and delivered to users.
- **Developers** — test notification payloads, categories, and overrides directly from your code editor during development.


## Available Tools
- **create_broadcast**: Create a new broadcast
- **get_broadcast**: Fetch a specific broadcast
- **list_broadcasts**: List all broadcasts in the project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MagicBell** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent broadcasts in my MagicBell project."

**🤖 AI Agent:**
> I've retrieved the broadcasts for your project. You have 3 recent entries: 'Welcome Campaign' (ID: 8a2...), 'System Alert' (ID: 4f1...), and 'Weekly Digest' (ID: 9c2...). Which one would you like to inspect?

---

**👤 You:**
> "Show me the details and status for broadcast ID 550e8400-e29b-41d4-a716-446655440000."

**🤖 AI Agent:**
> Inspecting broadcast 550e8400... The status is 'processed'. It was sent with the title 'Maintenance Notice' and reached 1,240 recipients across Email and Web Push channels.

---

**👤 You:**
> "Create a new broadcast titled 'Flash Sale' with content 'Get 50% off today only!' for all recipients."

**🤖 AI Agent:**
> I've successfully created the 'Flash Sale' broadcast. It is now being processed and triggered for your recipient list. You can track its progress using the generated ID: 771b92...


## ❓ FAQ

**Q: Can I send a notification to specific users or groups?**
Yes! When using the `create_broadcast` tool, you can provide an array of user IDs or emails in the `recipients` field to target specific individuals or segments.

**Q: How do I check if a broadcast has been successfully processed?**
You can use the `get_broadcast` tool with the unique broadcast ID. It will return the current processing status and metadata for that specific notification event.

**Q: Is it possible to customize the message content for different channels like Email or SMS?**
Absolutely. The `create_broadcast` tool includes an `overrides` parameter where you can specify different content or templates for specific channels (email, sms, push).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/magicbell](https://vinkius.com/mcp/magicbell)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MagicBell** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `magicbell` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MagicBell** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "magicbell": {
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
