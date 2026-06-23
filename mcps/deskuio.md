# Desku.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deskuio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Unify customer support across email, chat, and social with AI-assisted ticket resolution that speeds up response times.

## Description
Connect your **Desku.io** account to any AI agent and take full control of your customer support operations and helpdesk workflows through natural conversation.

### What you can do

- **Ticket Orchestration** — List and manage support tickets programmatically, including updating statuses (open, pending, closed) and retrieving detailed metadata
- **Conversation Intelligence** — Access complete message history for any ticket to provide high-fidelity context for replies and internal notes
- **Direct Engagement** — Programmatically add new replies or internal collaborator notes to tickets to streamline customer resolutions
- **Customer Lifecycle** — Access detailed customer profiles and monitor their entire ticket history to maintain perfectly coordinated support journeys
- **Agent Coordination** — Retrieve directories of support staff to understand team availability and assignments directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Desku.io profile settings
3. Start managing your helpdesk and customer relationships from Claude, Cursor, or any MCP client

No more manual ticket searching or complex dashboard navigation. Your AI acts as your dedicated support engineer and CX coordinator.

### Who is this for?

- **Support Teams** — instantly respond to high-priority tickets and summarize customer histories using natural language commands
- **Customer Success Managers** — monitor user profiles and track resolution times without leaving your communication tools
- **Operations Leads** — automate agent assignment tracking and manage customer data through simple AI queries


## Available Tools (9)
- **create_conversation**: Reply to a ticket
- **create_ticket**: Create a new ticket
- **get_customer**: Get customer details
- **get_ticket**: Get ticket details
- **list_agents**: List support agents
- **list_conversations**: List conversation history for a ticket
- **list_customers**: List support customers
- **list_tickets**: io account.

List support tickets
- **update_ticket**: Update a ticket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Desku.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active support tickets in Desku."

**🤖 AI Agent:**
> I've retrieved your support pipeline. You have 3 active tickets, including '#1024: Payment Failure' and '#1025: API Setup'. Would you like the full message history for the payment issue?

---

**👤 You:**
> "Show the conversation history for ticket #1024."

**🤖 AI Agent:**
> Fetching transcript... Ticket #1024 involves a customer reporting a 404 error during checkout. Agent Sarah replied with a fix 1 hour ago. The status is currently 'open'. Shall I add an internal note for Sarah?

---

**👤 You:**
> "Reply to ticket #1025: 'We have updated your API limits'."

**🤖 AI Agent:**
> Reply successfully sent! I've updated ticket #1025 with your message. The customer will be notified, and I've also updated the internal activity log. Need help with anything else?


## ❓ FAQ

**Q: How do I find my Desku API Key?**
Log in to Desku.io, click your profile picture, navigate to **Profile Settings**, and you will find your API Key at the bottom.

**Q: Can I add internal notes for other agents?**
Yes! Use the `create_conversation` tool and specify that the message is an internal note to coordinate with your team privately.

**Q: How do I see who is assigned to a ticket?**
The `get_ticket` tool retrieves complete metadata including the assigned agent ID and their current status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deskuio](https://vinkius.com/mcp/deskuio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Desku.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deskuio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Desku.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deskuio": {
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
