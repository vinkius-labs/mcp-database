# Front MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/front-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage shared inboxes across email, SMS, and social with team collaboration tools that keep customer conversations organized.

## Description
Connect your **Front** account to any AI agent and take full control of your team's customer communication and shared inbox workflows through natural conversation.

### What you can do

- **Conversation Orchestration** — List and manage customer conversations programmatically, including updating statuses (open, archived, spam) and assigning teammates
- **Message Intelligence** — Retrieve complete message histories and metadata for any conversation to perform deep analysis and sentiment tracking
- **Omnichannel Support** — Monitor multiple communication streams including Email, Chat, and SMS from a single unified AI interface
- **Team Collaboration** — Manage team contacts and retrieve teammate profiles to coordinate internal routing and workload distribution
- **Operational Visibility** — Get a comprehensive overview of shared inboxes and active channels using natural language commands

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from Front (Settings > Developers > API Tokens)
3. Start managing your unified inbox from Claude, Cursor, or any MCP client

No more manual toggling between different communication channels. Your AI acts as your dedicated support and communication coordinator.

### Who is this for?

- **Support Teams** — instantly triage high-volume inboxes and assign urgent conversations using natural language
- **Customer Success Managers** — retrieve full interaction histories and update contact details without leaving your workspace
- **Operations Leads** — monitor channel activity and manage team assignments across shared mailboxes


## Available Tools
- **reply_to_conversation**: Send a message
- **get_contact_info**: Get contact details
- **get_conversation_details**: Get conversation info
- **get_api_status**: Check connection
- **get_message_content**: Read message details
- **list_active_channels**: ).

List communication channels
- **list_team_contacts**: List your contacts
- **list_conversations**: List team conversations
- **list_shared_inboxes**: List team inboxes
- **list_conversation_messages**: Get message history
- **search_conversations_by_query**: Find conversations
- **update_conversation_status**: Modify conversation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Front** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open conversations in my shared inbox."

**🤖 AI Agent:**
> I've retrieved 5 open conversations. Notable threads include 'Issue with pricing' (ID: cnv_123) and 'New feature request' (ID: cnv_456). Which one should I provide details for?

---

**👤 You:**
> "Show me the message history for conversation 'cnv_123'."

**🤖 AI Agent:**
> Scanning cnv_123... I found 4 messages. The latest was an email from 'John Doe' asking about Enterprise discounts. Would you like the full content of the last message?

---

**👤 You:**
> "Reply to conversation 'cnv_123' saying 'I will check that for you right now'."

**🤖 AI Agent:**
> Done! I've sent your reply to conversation cnv_123. The customer will see your message in their inbox immediately.


## ❓ FAQ

**Q: How do I create an API Token in Front?**
Log in to Front, go to **Settings** > **Developers** > **API Tokens**, and click **Create Token**. Ensure you select the appropriate scopes for your needs.

**Q: Can I search for conversations by status?**
Yes! The `list_conversations` tool allows you to filter results by statuses like 'open', 'archived', 'deleted', or 'spam'.

**Q: How do I send a reply via AI?**
Use the `reply_to_conversation` tool by providing the `conversationId` and your message body. You can also specify an `author_id` to send as a specific teammate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/front-alternative](https://vinkius.com/mcp/front-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Front** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `front-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Front** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "front-alternative": {
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
