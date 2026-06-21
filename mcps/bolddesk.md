# BoldDesk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bolddesk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Empower your customer support via BoldDesk — manage tickets, contacts, and agents directly from any AI agent.

## Description
Connect your **BoldDesk** customer service account to any AI agent and orchestrate your support ticketing and help desk workflows through natural conversation.

### What you can do

- **Ticket Oversight** — List all support tickets and retrieve detailed history, including private notes and public replies.
- **Ticketing Automation** — Create and update tickets directly from your workspace to streamline issue tracking.
- **Customer Communication** — Add internal notes or reply to customers directly through the AI agent.
- **Contact Management** — Access and manage your customer directory and individual user profiles.
- **Agent Coordination** — List and retrieve details for support agents to monitor team activity and assignments.

### How it works

1. Subscribe to this server
2. Enter your BoldDesk API Key and Domain
3. Start managing your help desk from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Leads** — quickly check ticket statuses and agent assignments without manual dashboard searches.
- **Customer Success Managers** — retrieve customer histories and profiles straight from their workflow tools.
- **Developers** — integrate support ticketing into their automated business processes using natural language.


## Available Tools
- **add_ticket_note**: Add a private note to a ticket
- **create_ticket**: Create a new support ticket
- **get_agent**: Get details of a specific agent
- **get_contact**: Get details of a specific contact
- **get_ticket**: Get details of a specific ticket
- **list_agents**: List all support agents
- **list_contacts**: List all customer contacts
- **list_tickets**: List all support tickets
- **reply_to_ticket**: Add a public reply to a ticket
- **update_ticket**: Update an existing ticket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BoldDesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active tickets in BoldDesk."

**🤖 AI Agent:**
> I've retrieved your active tickets. You have 5 open tickets, including 'Login Issue' (ID: 102) and 'Billing Inquiry' (ID: 105). Which one would you like more details on?

---

**👤 You:**
> "Create a new ticket: 'API Timeout' for user sarah@example.com."

**🤖 AI Agent:**
> Ticket created successfully! Subject: 'API Timeout', ID: 108. Sarah will receive a confirmation email shortly.

---

**👤 You:**
> "Add a private note to ticket 102: 'Needs review from engineering team'."

**🤖 AI Agent:**
> Private note added to ticket 102. The engineering team will see it in the internal dashboard.


## ❓ FAQ

**Q: Can I check the status of a specific support ticket?**
Yes! Use the `get_ticket` tool with the Ticket ID. Your agent will fetch the latest status, priority, and the full conversation history directly from BoldDesk.

**Q: How do I add a private note to a ticket for my team?**
Simply ask the agent to `add_ticket_note` and provide the Ticket ID and the content of your note. This will be added as a private internal note invisible to the customer.

**Q: Does the integration allow creating a ticket for a new user?**
Yes. When using `create_ticket`, if the requester email does not exist in your contact list, BoldDesk will automatically create a new contact profile for that user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bolddesk](https://vinkius.com/mcp/bolddesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BoldDesk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bolddesk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BoldDesk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bolddesk": {
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
