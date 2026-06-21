# Blip MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blip)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Build intelligent chatbots for WhatsApp, Messenger, and web that engage customers with conversational commerce flows.

## Description
### What you can do
- Send WhatsApp and Chatbot messages directly to your customers.
- Create, update, and retrieve detailed contact information.
- Monitor support tickets from Blip Desk and manage ongoing conversation threads.
- Analyze active conversations to trigger personalized workflows.

### How it works
1. Log in to your Blip portal and access your bot's settings.
2. Copy the API Key from the Connection Information area.
3. Securely connect your agent to start managing Blip communications instantly.

### Who is this for?
Customer Support teams managing tickets, Marketing teams triggering proactive messages, and Sales professionals following up on leads via WhatsApp.


## Available Tools
- **create_contact**: Create or update a Blip contact
- **delete_contact**: Delete a Blip contact
- **get_contact**: Get a Blip contact by ID
- **get_thread_messages**: Get messages from a Blip thread
- **get_ticket**: Get a Blip desk ticket by ID
- **list_contacts**: List Blip contacts
- **list_threads**: List Blip conversation threads
- **list_tickets**: List Blip desk tickets
- **ping_bot**: Ping the Blip bot
- **send_message**: Send a message to a Blip contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the details for ticket ID '12345' on Blip Desk."

**🤖 AI Agent:**
> I'll fetch the details for ticket '12345' from Blip Desk now.

---

**👤 You:**
> "Send a WhatsApp message saying 'Hello, your order is ready' to 5511999999999."

**🤖 AI Agent:**
> The message has been successfully sent to the specified contact.

---

**👤 You:**
> "List all active threads and summarize what users are asking."

**🤖 AI Agent:**
> Here are the active threads along with a brief summary of their content.


## ❓ FAQ

**Q: Can the AI Agent manage ongoing Chatbot threads?**
Yes, the agent can list active threads and retrieve their messages to understand the full context of a customer's conversation.

**Q: Is it possible to reply to customer support tickets on Blip Desk?**
The AI agent can retrieve and analyze tickets from Blip Desk and send direct messages to the user via the `send_message` tool to assist with resolutions.

**Q: Can I use the agent to send automated WhatsApp notifications?**
Absolutely. The agent can use the messaging capabilities to trigger plain text messages directly to phone numbers connected to your Blip router.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blip](https://vinkius.com/mcp/blip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blip** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blip` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blip** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blip": {
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
