# Front MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/front)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage shared inboxes, track conversations, and collaborate on emails via AI agents with Front.

## Description
Connect your **Front** account to any AI agent to automate your customer communication and shared inbox workflows through the Model Context Protocol (MCP). Front is a customer operations platform that enables teams to manage shared emails, SMS, and chats collaboratively. This MCP server enables you to track active conversations, assign messages, and fetch thread histories directly through natural conversation.

### Key Features

- **Shared Inbox Management** — List all accessible shared inboxes and retrieve the specific conversations routed to them.
- **Conversation Tracking** — Search and list all customer conversations, checking their current status (open, archived) and assigned owners.
- **Message Threading** — Fetch the complete message history for any specific conversation to maintain context before replying.
- **Collaborative Replies** — Draft and send replies to active conversations directly from your chat interface on behalf of a teammate.
- **Status Automation** — Programmatically update conversation statuses (e.g., archiving resolved issues) to keep inboxes clean.
- **Team & Contact Discovery** — List all workspace teammates and customer contacts to ensure accurate routing and messaging.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Front API Token (found in your Developer Settings)
3. Start managing your shared inboxes from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Support** — quickly check open conversations in the support inbox and fetch message history without leaving your agent.
- **Operations Teams** — automate the archiving of specific conversation types or verify teammate assignments.
- **Account Managers** — get a real-time overview of client communications and send quick follow-ups via simple AI commands.


## Available Tools (12)
- **list_all_conversations**: List all conversations
- **list_inbox_threads**: List inbox conversations
- **list_shared_inboxes**: List shared inboxes
- **list_conversation_messages**: List thread messages
- **list_inbox_teammates**: List Front teammates
- **search_conversations**: g. "inbox:inb_123 is:open").

Search all conversations
- **send_inbox_reply**: Send a reply
- **update_conversation_status**: g., archived, open) or assignee of a conversation.

Update conversation
- **verify_api_status**: Verify connection
- **get_conversation_details**: Get conversation metadata
- **get_inbox_details**: Get inbox metadata
- **list_address_book**: List contacts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Front** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all shared inboxes in my Front account."

**🤖 AI Agent:**
> Retrieving inboxes... I found 3 shared inboxes: 'Support' (ID: inb_123), 'Sales' (ID: inb_456), and 'General Info' (ID: inb_789).

---

**👤 You:**
> "Search for open conversations in the Support inbox."

**🤖 AI Agent:**
> Searching conversations... I found 4 open conversations matching your query. Two are currently assigned to 'John', and two remain unassigned.

---

**👤 You:**
> "Archive conversation 'cnv_987'."

**🤖 AI Agent:**
> Conversation updated! I have successfully changed the status of conversation cnv_987 to 'archived'. It will no longer appear in the open queue.


## ❓ FAQ

**Q: How do I get an API Token for Front?**
Log in to your Front account, click the gear icon (Settings), go to 'Developers' > 'API Tokens', and create a new token with 'Shared Resources' scope.

**Q: Can I search for specific types of conversations?**
Yes, use the 'search_conversations' tool. It accepts standard Front search syntax, such as 'is:open' or 'inbox:support'.

**Q: Is it possible to reply to an email via the agent?**
Yes! Use the 'send_inbox_reply' tool. You must provide the Conversation ID, the message body, and the Teammate ID of the sender.

**Q: How do I archive a conversation?**
Use the 'update_conversation_status' tool and set the status parameter to 'archived'. This updates the global status for the shared inbox.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/front](https://vinkius.com/mcp/front)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `front` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Front** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "front": {
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
