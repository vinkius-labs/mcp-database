# Chatwoot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chatwoot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage customer engagement via Chatwoot — track conversations, reply to messages, and manage contacts directly from any AI agent.

## Description
Connect your **Chatwoot** account to any AI agent and take full control of your customer support and engagement through natural conversation. Streamline how you manage chats across Web, WhatsApp, Facebook, and more.

### What you can do

- **Conversation Oversight** — List and retrieve details for all active and resolved conversations natively
- **Live Replying** — Send messages to customers in active chat sessions flawlessly
- **Contact Management** — List and retrieve detailed customer contact information and history securely
- **Inbox Intelligence** — Monitor all configured inboxes, including Web widgets and social integrations flawlessly
- **Agent Tracking** — List all support agents and manage team availability in real-time
- **Message History** — Access complete chat histories to understand customer context directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chatwoot Access Token, Account ID, and Base URL
3. Start managing your customer support from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Managers** — monitor team performance and review chat histories using natural language
- **Customer Success Teams** — engage with customers and manage contact profiles without opening the dashboard
- **Small Business Owners** — quickly reply to customer inquiries across multiple channels straight from their chat interface
- **Developers** — automate message routing and contact synchronization


## Available Tools
- **get_contact_details**: Get detailed information for a specific customer contact
- **get_conversation_details**: Get detailed information for a specific conversation
- **list_support_agents**: List all support agents in the account
- **list_chatwoot_contacts**: List all customer contacts
- **list_woot_conversations**: List all conversations in the account
- **list_chatwoot_inboxes**: List all configured inboxes (Web, WhatsApp, etc)
- **get_chat_history**: Retrieve the message history for a specific conversation
- **send_chat_message**: Send a message to a customer in a specific conversation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chatwoot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active conversations in Chatwoot."

**🤖 AI Agent:**
> Retrieving your active conversations... I found 3 chats from 'John Doe' (Web), 'Sarah Smith' (WhatsApp), and 'Mike Miller' (Facebook). Which one would you like to open?

---

**👤 You:**
> "What did the customer in conversation ID 555 say last?"

**🤖 AI Agent:**
> Checking conversation 555... The last message from 'Sarah Smith' was: 'Hi, I haven't received my order confirmation email yet. Can you help?'

---

**👤 You:**
> "Reply to conversation 555: 'I'll look into this right now for you, Sarah.'"

**🤖 AI Agent:**
> Sending your reply to conversation 555... The message has been delivered to Sarah Smith via WhatsApp.


## ❓ FAQ

**Q: Can I reply to a WhatsApp message through the agent?**
Yes! Use the `send_chat_message` tool with the conversation ID. As long as your WhatsApp inbox is connected to Chatwoot, the agent will deliver your reply.

**Q: How do I see the full history of a chat?**
Use the `get_chat_history` tool with the unique conversation ID. Your agent will fetch all previous messages, allowing you to review the entire interaction.

**Q: Where do I find my Chatwoot Access Token?**
Log in to Chatwoot, click on your profile avatar in the bottom left, and select 'Profile Settings'. Scroll to the bottom to find your personal 'Access Token'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chatwoot](https://vinkius.com/mcp/chatwoot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chatwoot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chatwoot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chatwoot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chatwoot": {
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
