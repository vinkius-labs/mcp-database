# Daktela MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/daktela)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Handle customer interactions across phone, email, chat, and social media from one omnichannel contact center platform.

## Description
Connect your **Daktela** omnichannel contact center to any AI agent and simplify how you coordinate customer support, track communication history, and manage CRM records through natural conversation.

### What you can do

- **Ticket Lifecycle** — Create, list, and query support tickets and cases to ensure customer issues are resolved promptly.
- **Omnichannel Activities** — Monitor real-time and past activities across calls, emails, and chats within your center.
- **CRM Control** — List and create contacts and accounts (companies) to maintain an organized customer directory.
- **Call & Email History** — Retrieve detailed logs of past phone interactions and email threads for audit and reporting.
- **Team & Queue Coordination** — List configured queues and system users to manage agent distribution effectively.
- **Profile Oversight** — Fetch your authenticated user profile and verify system configurations directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Daktela Domain and Access Token (found in your user settings)
3. Start managing your omnichannel communications from Claude, Cursor, or any MCP client

### Who is this for?

- **Support Team Leads** — quickly check ticket statuses and monitor queue volumes via simple AI commands.
- **Customer Service Agents** — create CRM contacts and log activities directly from the workspace.
- **Operations Managers** — verify call history and retrieve agent distribution metadata via the AI assistant.


## Available Tools (12)
- **create_contact**: Create a new CRM contact
- **create_ticket**: Create a new ticket
- **get_me**: Get current user information
- **get_ticket**: Get details of a specific ticket
- **list_accounts**: List CRM accounts
- **list_activities**: List recent activities in Daktela
- **list_call_history**: List call history
- **list_contacts**: List CRM contacts
- **list_email_history**: List email history
- **list_queues**: List contact center queues
- **list_tickets**: List support tickets
- **list_users**: List Daktela users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Daktela** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active activities in the contact center."

**🤖 AI Agent:**
> I've retrieved the activities log. You have 5 recent interactions: 2 inbound calls from 'John Doe', 1 pending email from 'Sarah Smith', and 2 active web chats. Which one would you like to see details for?

---

**👤 You:**
> "Create a support ticket: 'Login issue' for contact 'cont_10293'."

**🤖 AI Agent:**
> Ticket created! I've logged the support case 'Login issue' in Daktela and associated it with contact cont_10293. The ticket ID is tic_88231. Your support team has been notified.

---

**👤 You:**
> "Show me the email history for contact 'cont_5521'."

**🤖 AI Agent:**
> Fetching email interactions... For contact cont_5521, I found 3 recent email threads discussing 'Billing Inquiry' and 'Product Upgrade'. Would you like the full body of the latest message?


## ❓ FAQ

**Q: Can I see all the open tickets in my Daktela account?**
Yes! Use the `list_tickets` tool. Your agent will retrieve the complete directory of support cases, which you can then filter or summarize.

**Q: How do I create a new contact in the Daktela CRM?**
Use the `create_contact` action. Provide the first name, last name, and optional email or phone number to register the person in your CRM database instantly.

**Q: Is it possible to list the history of past phone calls via AI?**
Absolutely. Use the `list_call_history` query. The agent will retrieve a detailed log of past voice interactions, including participants and durations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/daktela](https://vinkius.com/mcp/daktela)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Daktela** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `daktela` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Daktela** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "daktela": {
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
