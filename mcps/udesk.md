# Udesk / 沃丰科技 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/udesk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Comprehensive customer service platform — manage tickets, customers, and knowledge base via AI.

## Description
Empower your AI agent to orchestrate your customer service operations with **Udesk**, the premier helpdesk platform in China. By connecting Udesk to your agent, you transform complex ticket management, customer profile auditing, and knowledge base retrieval into a natural conversation. Your agent can instantly list support tickets, retrieve detailed customer information, browse knowledge base articles, and even monitor agent activity without you ever needing to navigate the comprehensive web portal. Whether you are troubleshooting high-priority issues or coordinating support teams, your agent acts as a real-time service assistant, keeping your data accurate and your customers satisfied.

### What you can do

- **Ticket Orchestration** — List all support tickets and retrieve detailed subject and content metadata.
- **Customer Profile Control** — Browse helpdesk customers and retrieve detailed contact and organization information.
- **Agent Management** — List all support agents and identify functional groups within the service team.
- **Knowledge Retrieval** — Browse and retrieve articles from the internal knowledge base to accelerate resolution.
- **Activity Auditing** — Retrieve historical reply chains for tickets to monitor service quality.

### How it works

1. Subscribe to this server
2. Enter your Udesk Subdomain, Admin Email, and API Token
3. Start managing your customer service through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Managers** — monitor ticket progress and audit agent performance through natural language queries.
- **Customer Success Leads** — retrieve detailed customer profiles and interaction histories directly from your AI-powered workspace.
- **Service Operations** — oversee agent groups and coordinate cross-functional support via a unified AI interface.
- **Udesk Power Users** — integrate your existing service workflows into your AI-driven daily routines.


## Available Tools (10)
- **create_ticket**: Create a new ticket
- **get_customer**: Get customer details
- **get_organization**: Get organization details
- **get_ticket**: Get ticket details
- **get_ticket_replies**: Get ticket reply history
- **list_agents**: List support agents
- **list_articles**: List knowledge base articles
- **list_customers**: List helpdesk customers
- **list_groups**: List agent groups
- **list_tickets**: List helpdesk tickets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Udesk / 沃丰科技** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active helpdesk tickets."

**🤖 AI Agent:**
> I've retrieved your Udesk tickets. You have 15 open incidents, including 'Server Down in Region A' and 'Billing Inquiry - Client B'. Would you like to check the latest replies for any of them?

---

**👤 You:**
> "Show me the details for customer 'mario@example.com'."

**🤖 AI Agent:**
> I've retrieved the profile for Mario. He is a VIP customer from the 'Global Partners' organization with 12 historical tickets. Would you like to see his active ticket history?

---

**👤 You:**
> "Check the knowledge base for articles about 'Refund Policy'."

**🤖 AI Agent:**
> I've found 3 articles in the Udesk knowledge base matching your query. The primary guide 'Standard Refund Procedures' was last updated 2 days ago. Should I retrieve the full content for you?


## ❓ FAQ

**Q: How do I find my Udesk API Token?**
Log in to your Udesk admin backend, go to [Admin] → [Settings] → [Validation Info], and you will find your Open API Token there. Ensure you have administrator privileges.

**Q: Can I see ticket reply histories through this server?**
Yes. Use the `get_ticket_replies` tool with a specific ticket ID to retrieve the entire historical chain of comments and messages for that incident.

**Q: Is it possible to list support agents and their groups?**
Yes! You can use the `list_agents` and `list_groups` tools to see all members of your support organization and how they are structured into functional teams.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/udesk](https://vinkius.com/mcp/udesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Udesk / 沃丰科技** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `udesk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Udesk / 沃丰科技** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "udesk": {
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
