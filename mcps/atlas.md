# Atlas MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/atlas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage customer support and ticketing with Atlas.so — track conversations, customers, and articles via AI.

## Description
The **Atlas MCP Server** provides a seamless natural language interface to your Atlas.so customer support platform. Empower your AI agent to manage your entire support operation, from ticket auditing to customer oversight and knowledge base access.

### Key Features

- **Ticket Management** — List all active support tickets, retrieve detailed conversation metadata, and create new tickets directly from your chat.
- **Customer Oversight** — Access and manage your customer database, including names, emails, and internal IDs.
- **Knowledge Base Access** — List help center articles to provide accurate information based on your organization's documentation.
- **Team Monitoring** — View a list of team users (agents) to understand your support capacity.
- **Real-time Support Analytics** — Quickly audit active conversations and customer needs using simple natural language commands.
- **Secure API Integration** — Uses your Atlas.so API Token for safe and authenticated access to your support data.

### Who is this for?

- **Support Leads** — Quickly check ticket statuses and team activity without navigating complex web dashboards.
- **Product Managers** — Review recent customer tickets and feedback regarding specific features or updates.
- **Customer Success Managers** — Retrieve customer history and help articles to provide better assistance during client interactions.


## Available Tools (8)
- **create_ticket**: Create a new support ticket
- **get_account_check**: Verify Atlas account connection
- **get_customer**: Get details for a specific customer
- **get_ticket**: Get details for a specific ticket
- **list_articles**: List help center articles
- **list_customers**: List all customers in Atlas
- **list_tickets**: List all support tickets in Atlas
- **list_users**: List team users (agents)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Atlas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active support tickets in Atlas."

**🤖 AI Agent:**
> I've retrieved your active tickets. You have 10 open issues, including 'Login Problem' and 'Billing Inquiry'.

---

**👤 You:**
> "Show me the details for ticket ID 'tick_12345'."

**🤖 AI Agent:**
> Ticket 'tick_12345' is titled 'Payment Failed'. The current status is 'Open' and it was created by 'John Doe' (john@example.com).

---

**👤 You:**
> "Find all help articles related to 'Pricing'."

**🤖 AI Agent:**
> I've found 3 articles related to pricing: 'Subscription Plans', 'Annual vs Monthly Billing', and 'Refund Policy'.


## ❓ FAQ

**Q: How do I find my Atlas.so API Token?**
Log in to your Atlas dashboard, go to **App Configuration > Data > API**, and you will find your API Token there.

**Q: Can I see help center articles via this server?**
Yes, use the `list_articles` tool to retrieve a list of articles from your Atlas help center.

**Q: How are customer IDs handled?**
Atlas uses unique internal IDs for customers. You can discover these IDs by using the `list_customers` tool or searching for a specific customer by email.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/atlas](https://vinkius.com/mcp/atlas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Atlas** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `atlas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Atlas** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "atlas": {
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
