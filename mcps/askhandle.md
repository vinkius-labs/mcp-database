# AskHandle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/askhandle)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Integrate custom AI agents with AskHandle.

## Description
The AskHandle MCP server enables your AI agent to manage chat rooms, messages, leads, and webhooks. Interact with your AskHandle AI agents and capture visitor information directly from your conversation.


## Available Tools (12)
- **create_lead**: Create a new lead
- **create_room**: Create a new chat room
- **create_webhook**: Create a new webhook subscription
- **delete_webhook**: Delete a webhook subscription
- **get_me**: Check API connectivity and get account context
- **list_leads**: List all leads captured
- **list_messages**: List messages, optionally filtered by room
- **list_rooms**: List all chat rooms
- **list_webhooks**: List all configured webhooks
- **retrieve_lead**: Get details of a specific lead
- **retrieve_room**: Get details of a specific chat room
- **send_message**: Send a message to a chat room


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AskHandle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active chat rooms in AskHandle."

**🤖 AI Agent:**
> Fetching active rooms... You currently have 5 active sessions. The latest is 'Support Query - Ticket #402'.

---

**👤 You:**
> "Send a message 'Hello' to room 'ROOM_ID'."

**🤖 AI Agent:**
> Message 'Hello' successfully sent to room 'ROOM_ID'.

---

**👤 You:**
> "List all captured leads."

**🤖 AI Agent:**
> I've retrieved your leads. You have 24 new leads from this week, including 'Acme Corp' and 'TechLogix'.


## ❓ FAQ

**Q: What are 'Rooms' in AskHandle?**
Rooms represent chat sessions or conversation contexts between a user and an AI agent.

**Q: How are leads captured?**
Leads can be captured automatically by your AI agent during a conversation or created programmatically via the API.

**Q: Is it possible to manage webhooks directly from the chat?**
Yes, you can register new webhooks to receive real-time notifications about events in AskHandle directly using the AI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/askhandle](https://vinkius.com/mcp/askhandle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AskHandle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `askhandle` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AskHandle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "askhandle": {
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
