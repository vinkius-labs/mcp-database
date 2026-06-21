# FreeScout MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freescout)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your FreeScout helpdesk — list mailboxes, handle conversations, reply to customers, and manage users directly via AI.

## Description
Connect your **FreeScout** helpdesk to any AI agent to streamline your customer support workflows. FreeScout is the leading open-source helpdesk, and this MCP server allows you to interact with it using natural language.

### What you can do

- **Mailbox Management** — List and inspect all mailboxes in your installation to organize incoming requests.
- **Conversation Handling** — Create, update, and delete conversations, or list them by mailbox to stay on top of tickets.
- **Customer Interaction** — Send replies directly to customers or add internal notes for team collaboration.
- **Customer & User Directory** — Manage customer profiles and list team members (users) to assign tasks efficiently.
- **Thread Inspection** — View the full history of messages and threads within any conversation for complete context.

### How it works

1. Subscribe to this server
2. Enter your FreeScout API Key and your instance's Base URL
3. Start managing tickets and customers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Teams** — quickly summarize long threads and draft replies without leaving your AI workspace.
- **Support Managers** — monitor mailbox activity and reassign conversations to the right team members.
- **Developers** — integrate support data into your workflow to track bugs and customer feedback directly.


## Available Tools
- **add_note**: Add an internal note to a conversation
- **add_reply**: Send a reply to the customer in a conversation
- **list_conversations**: List conversations in a mailbox
- **create_conversation**: Create a new conversation
- **create_customer**: Create a new customer
- **list_customers**: List customers
- **delete_conversation**: Delete a conversation
- **get_conversation**: Retrieve conversation details
- **get_customer**: Retrieve customer details
- **get_mailbox**: Retrieve a specific mailbox
- **get_user**: Retrieve agent details
- **list_mailboxes**: List all mailboxes
- **list_threads**: List threads in a conversation
- **update_conversation**: Update a conversation (status, assignee, etc.)
- **update_customer**: Update customer information
- **list_users**: List all users/agents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FreeScout** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my mailboxes in FreeScout."

**🤖 AI Agent:**
> I've retrieved your mailboxes. You have: 'Support' (ID: 1), 'Sales' (ID: 2), and 'Billing' (ID: 3). Which one would you like to check?

---

**👤 You:**
> "Show me the latest conversations in mailbox 1."

**🤖 AI Agent:**
> Found 3 recent conversations in the Support mailbox. One is regarding 'Login Issue' (ID: 502) and another about 'API Access' (ID: 505). Would you like to see the threads for any of these?

---

**👤 You:**
> "Add an internal note to conversation 502 saying 'Checking with the dev team'."

**🤖 AI Agent:**
> Internal note added successfully to conversation 502. Your team will see it in the FreeScout dashboard.


## ❓ FAQ

**Q: How do I reply to a customer conversation using the AI?**
You can use the `add_reply` tool. Just provide the Conversation ID and the body of your message, and the agent will send it to the customer via FreeScout.

**Q: Can I update the status or assignee of a ticket?**
Yes! Use the `update_conversation` tool. You can change the status (active, pending, closed, spam) or provide an `assignee_id` to route the ticket to a specific team member.

**Q: Is it possible to add internal notes that the customer won't see?**
Absolutely. Use the `add_note` tool to post internal comments on a conversation. These are visible to your team in FreeScout but are never sent to the customer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freescout](https://vinkius.com/mcp/freescout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FreeScout** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `freescout` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FreeScout** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freescout": {
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
