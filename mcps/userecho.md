# UserEcho MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/userecho)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Build a customer feedback community with idea voting, knowledge base, helpdesk, and live chat in one support ecosystem.

## Description
Connect your **UserEcho** account to any AI agent and simplify how you manage your community feedback, helpdesk tickets, and self-service content through natural conversation.

### What you can do

- **Helpdesk Management** — List all support tickets and retrieve detailed conversation history and status for specific issues.
- **Direct Ticketing** — Programmatically create new support tickets directly from your agent to accelerate customer assistance.
- **Knowledge Base Access** — List and query all articles in your help center to verify self-service documentation.
- **Forum Oversight** — List and monitor feedback and support forums to understand community trends and suggestions.
- **User Directory** — List account users and team members to manage your support organization structure.
- **Issue Tracking** — Monitor the progress of client requests and verify resolution times via AI.

### How it works

1. Subscribe to this server
2. Enter your UserEcho API Token and Subdomain (found in your developer settings)
3. Start managing your community feedback from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Support Managers** — quickly retrieve ticket histories and monitor team activity via simple AI commands.
- **Community Managers** — monitor forum feedback and verify article availability directly from the workspace.
- **Product Teams** — coordinate bug reports and feature requests coming from UserEcho forums.


## Available Tools (6)
- **list_account_users**: List account users
- **create_support_ticket**: Add a new ticket
- **get_ticket_details**: Get details for a specific ticket
- **list_kb_articles**: List knowledge base articles
- **list_forums**: List UserEcho forums
- **list_tickets**: List helpdesk tickets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UserEcho** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active support tickets in my account."

**🤖 AI Agent:**
> I've retrieved your support tickets. You have 5 active requests including 'Login issue', 'Billing inquiry', and 'Feature request: dark mode'. Which one would you like to see the history for?

---

**👤 You:**
> "Show me the details for ticket #88231."

**🤖 AI Agent:**
> I've fetched the details for ticket 88231. The status is currently 'Open' and it concerns a 'Broken checkout link'. The last comment was from the customer 2 hours ago. Shall I reply to them?

---

**👤 You:**
> "Create a support ticket: 'API Timeout error' with content 'Receiving 504 errors on the /v1/users endpoint'."

**🤖 AI Agent:**
> Success! The support ticket 'API Timeout error' has been created in your UserEcho account with ID TKT-10293. I've logged the technical details provided.


## ❓ FAQ

**Q: Can I see the full conversation history of a support ticket?**
Yes! Use the `get_ticket_details` tool and provide the Ticket ID. Your agent will retrieve the complete metadata and all conversation threads for that specific issue.

**Q: How do I list all the help center articles in my account?**
Run the `list_kb_articles` query. The agent will retrieve a complete list of all articles currently published in your UserEcho knowledge base.

**Q: Is it possible to create a new ticket via AI for a customer?**
Absolutely. Use the `create_support_ticket` action. Provide a header and the detailed content, and the agent will instantly log the request in your UserEcho helpdesk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/userecho](https://vinkius.com/mcp/userecho)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UserEcho** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `userecho` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UserEcho** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "userecho": {
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
