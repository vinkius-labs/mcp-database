# Freshchat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshchat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer conversations, track messages, and oversee agents via AI agents with Freshchat.

## Description
Connect your **Freshchat** account to any AI agent to automate your customer messaging and conversation management through the Model Context Protocol (MCP). Freshchat is a modern messaging software built for sales and support teams to engage with customers across web, mobile, and social channels. This MCP server enables you to track active chats, send real-time messages, and retrieve detailed user profiles directly through natural conversation.

### Key Features

- **Conversation Oversight** — List all active chats, fetch detailed conversation metadata, and monitor chat statuses (open, resolved) instantly.
- **Real-time Messaging** — Post new messages to existing conversations to keep your support workflows moving fast.
- **User & Customer Data** — Access detailed profile information for chat participants and search for users by email address.
- **Support Team Insights** — List all support agents and team members to maintain full context of who is online and available.
- **Channel & Group Management** — Access configured messaging channels and agent groups to understand your routing logic.
- **Message History** — Retrieve the full message history for any specific conversation ID for audit and reporting.
- **Multi-Region Support** — Seamlessly connect to your specific Freshchat data center (US, EU, IN, AU).

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freshchat Region Domain and API Token (found in Settings > API Tokens)
3. Start managing your customer messaging from Claude, Cursor, or any MCP client

### Who is this for?

- **Support Leads** — quickly check for open conversations or list agent availability without leaving your primary workspace.
- **Customer Success Managers** — get a real-time overview of customer interactions and user profiles via simple AI commands.
- **Sales Engineers** — automate the sending of follow-up messages or verify chat history for lead qualification.


## Available Tools (12)
- **get_agent_profile**: Get agent metadata
- **get_conversation_details**: Get chat metadata
- **get_chat_user_details**: Get user metadata
- **list_support_agents**: List support agents
- **list_chat_channels**: List chat channels
- **list_conversations**: List active chats
- **list_agent_groups**: List agent groups
- **list_chat_messages**: List messages in a chat
- **list_chat_users**: List chat participants
- **search_chat_users**: Find user by email
- **send_chat_message**: Post a new message
- **check_account_status**: Verify account configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshchat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open conversations in my Freshchat account."

**🤖 AI Agent:**
> Retrieving chats... I found 4 open conversations, including one with 'John Doe' regarding 'Billing' and another with 'Sarah' about 'API Integration'.

---

**👤 You:**
> "Find the Freshchat user with the email 'customer@example.com'."

**🤖 AI Agent:**
> Searching users... I found a record for 'Alice Smith' (ID: user_abc123) associated with that email. She has 2 past conversations in your account.

---

**👤 You:**
> "Send a message to conversation 'conv_987': 'I am looking into this for you'."

**🤖 AI Agent:**
> Message sent! Your update has been successfully posted to conversation 'conv_987'. The customer will see your reply in their chat widget.


## ❓ FAQ

**Q: How do I get an API Token for Freshchat?**
Log in to Freshchat, navigate to Settings > API Tokens, and click on 'Generate Token' to retrieve your Bearer Token.

**Q: What is my 'Region Domain'?**
Your domain depends on where your account is hosted (e.g. 'api.freshchat.com' for US, 'api.eu.freshchat.com' for Europe).

**Q: Can I send files or images through the agent?**
Currently, the 'send_chat_message' tool focuses on sending text content. Supporting rich media typically requires separate upload operations.

**Q: Is it possible to see the chat history of a customer?**
Yes! Use the 'list_chat_messages' tool and provide the Conversation ID. The agent will retrieve the historical message history for that thread.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshchat](https://vinkius.com/mcp/freshchat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freshchat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freshchat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freshchat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freshchat": {
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
