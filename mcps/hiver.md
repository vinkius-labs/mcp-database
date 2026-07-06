# Hiver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hiver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Turn Gmail into a helpdesk with shared labels, email assignment, and SLA tracking that works inside the inbox your team already uses.

## Description
Connect your **Hiver** account to any AI agent and transform your Gmail-based customer support into an intelligent, automated operation through natural conversation.

### What you can do

- **Shared Inbox Management** — List all shared mailboxes and retrieve detailed metadata for active email conversations
- **Workflow Automation** — Programmatically update conversation statuses (open, pending, closed) and manage assignments across your team
- **Collaborative Drafting** — Create shared drafts within Gmail threads directly through your agent to orchestrate perfect replies
- **Tagging & Organization** — Search and apply tags to categorize threads and maintain a high-fidelity collaboration ecosystem
- **Team Visibility** — List and search for inbox members to understand who is available and manage workload distribution

### How it works

1. Subscribe to this server
2. Retrieve your API Key from the Hiver Admin Panel (Integrations > Developer APIs)
3. Start managing your shared support hub from Claude, Cursor, or any MCP client

No more context-switching between tools to check if a customer was replied to. Your AI acts as your dedicated inbox coordinator.

### Who is this for?

- **Support Teams** — instantly triage inboxes, assign urgent threads, and check status without opening Gmail
- **Operations Managers** — monitor team workload and conversation volume through automated reports and queries
- **Customer Success Leads** — ensure high-priority threads are tagged and assigned to the right account managers in seconds


## Available Tools (12)
- **get_api_status**: Check connection
- **get_conversation_details**: Read email thread
- **get_inbox_details**: Get mailbox info
- **list_inbox_conversations**: List shared threads
- **list_shared_inboxes**: List Hiver inboxes
- **list_inbox_tags**: Get mailbox tags
- **list_inbox_members**: List team members
- **search_tags_by_name**: Find tags
- **search_team_members**: Find members
- **test_hiver_auth**: Verify credentials
- **update_thread_status**: Modify conversation
- **create_shared_draft**: Draft team reply


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hiver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all shared inboxes in my Hiver account."

**🤖 AI Agent:**
> I've fetched your inboxes. You have access to: 'Support' (ID: inbox_1), 'Sales' (ID: inbox_2), and 'Operations' (ID: inbox_3). Which one should we check for new messages?

---

**👤 You:**
> "Show me the last 5 open conversations in the 'Support' inbox."

**🤖 AI Agent:**
> Scanning 'Support'... I found 5 active threads. The most urgent one is 'Issue with login' from 'user@example.com'. Would you like to see the full details or assign it to someone?

---

**👤 You:**
> "Assign conversation 'thread-123' to user 'user-456' and add the tag 'priority'."

**🤖 AI Agent:**
> Done! Conversation 'thread-123' has been assigned to user 'user-456' and tagged as 'priority'. Your team will see the updated status in Hiver immediately.


## ❓ FAQ

**Q: How do I find an inbox ID?**
Use the `list_shared_inboxes` tool to retrieve all shared mailboxes you have access to, along with their unique identifiers and names.

**Q: Can I assign a conversation to a specific teammate?**
Yes! Use the `update_thread_status` tool and provide the `assignee_id`. You can find valid user IDs using the `list_inbox_members` tool.

**Q: Does Hiver support collaborative drafting through AI?**
Yes, the `create_shared_draft` tool allows your AI agent to write directly into a Gmail thread, which your team can then review and send from the Hiver interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hiver](https://vinkius.com/mcp/hiver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hiver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hiver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hiver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hiver": {
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
