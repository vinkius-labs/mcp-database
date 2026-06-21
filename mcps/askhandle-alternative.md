# AskHandle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/askhandle-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage AI chat rooms, capture leads, and automate messaging workflows directly through AskHandle.

## Description
Connect your **AskHandle** account to any AI agent to manage your conversational AI infrastructure, lead generation, and messaging workflows through natural language.

### What you can do

- **Room Management** — List, create, and update chat rooms to organize different conversation sessions and user contexts.
- **Messaging & AI Interaction** — Send messages to specific rooms and receive AI-generated responses, perfect for testing or automating customer support.
- **Lead Generation** — Retrieve and manage leads captured through your chat interfaces, including filtering by specific dates.
- **Webhook Automation** — Subscribe to real-time events like new messages or leads to trigger external workflows and notifications.
- **Data Inspection** — Fetch detailed metadata for specific rooms, messages, or leads to analyze performance and user behavior.

### How it works

1. Subscribe to this server
2. Enter your AskHandle API Key
3. Start managing your chat infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Success Managers** — monitor active chat rooms and review lead data without leaving your workspace.
- **Developers** — test messaging logic and manage webhook subscriptions directly from your code editor.
- **Marketing Teams** — export and analyze lead lists captured through AI chat interactions for campaign follow-ups.


## Available Tools
- **create_lead**: Manually create a new lead
- **create_message**: Send a new message and get an AI response
- **create_room**: Create a new chat room
- **create_webhook**: Create a new webhook subscription
- **delete_lead**: Delete a lead record
- **delete_room**: Delete a specific room
- **delete_webhook**: Remove a webhook subscription
- **get_lead**: Retrieve a specific lead
- **get_message**: Retrieve a specific message
- **get_room**: Retrieve details of a specific room
- **get_webhook**: Retrieve a specific webhook
- **list_leads**: List all leads
- **list_messages**: List all messages
- **list_rooms**: List all chat rooms
- **list_webhooks**: List all active webhooks
- **update_lead**: Update lead information
- **update_room**: Update a specific room
- **update_webhook**: Update a webhook (e.g., change target URL)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AskHandle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active chat rooms."

**🤖 AI Agent:**
> I've retrieved your rooms. You have 3 active sessions: 'Support-User-A' (UUID: 8821), 'Sales-Inquiry' (UUID: 9932), and 'General-Help' (UUID: 1102). Which one would you like to inspect?

---

**👤 You:**
> "Send a message 'How can I help you today?' to room uuid '8821'."

**🤖 AI Agent:**
> Message sent to room 8821. The AI response was: 'Hello! I am looking for information about your pricing plans.'

---

**👤 You:**
> "Show me all leads captured since 2024-01-01."

**🤖 AI Agent:**
> I found 12 leads captured since January 1st. The most recent ones are 'John Doe' (john@example.com) and 'Jane Smith' (jane@example.com). Would you like the full details for any of them?


## ❓ FAQ

**Q: Can I send a message to a specific room and get an AI response?**
Yes! Use the `create_message` tool. You can provide the message body and the `room_uuid` to interact with a specific conversation session.

**Q: How do I filter leads by date?**
You can use the `list_leads` tool with the optional `start_date` and `end_date` parameters (formatted as YYYY-MM-DD) to retrieve leads from a specific period.

**Q: Is it possible to automate notifications for new leads?**
Absolutely. Use the `create_webhook` tool to subscribe to the `lead.added` event and point it to your target URL for real-time notifications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/askhandle-alternative](https://vinkius.com/mcp/askhandle-alternative)
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
3. Set Type to "SSE", enter `askhandle-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AskHandle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "askhandle-alternative": {
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
