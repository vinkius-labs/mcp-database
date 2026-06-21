# HappyFox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/happyfox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate support ticketing via HappyFox — manage tickets, contacts, and help desk categories directly from any AI agent.

## Description
Connect your **HappyFox** help desk to any AI agent and take full control of your customer support workflows through natural conversation.

### What you can do

- **Ticket Management** — List all tickets, create new support requests, and retrieve detailed information for any case.
- **Staff Updates** — Add responses and updates to tickets directly from the chat to keep your team informed.
- **Contact Oversight** — List and search for customers (contacts) in your help desk database.
- **Categorization** — Access your ticket categories, statuses, and priorities to ensure proper routing.
- **Team Insights** — Retrieve lists of staff members and their assigned roles.
- **Search Capabilities** — Perform text-based searches across your entire ticket history.

### How it works

1. Subscribe to this server
2. Enter your HappyFox API Key, Auth Code, and Account Name
3. Start managing your help desk from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex ticketing tabs. Your AI assistant acts as a dedicated Support Coordinator or Help Desk Agent.

### Who is this for?

- **Support Managers** — instantly retrieve ticket statuses and staff workloads without digging through reports.
- **Customer Success Teams** — check client support history and add updates during follow-ups.
- **IT Support Staff** — automate the creation and tracking of internal technical tickets.


## Available Tools (10)
- **add_staff_update**: Add a staff response/update to a ticket
- **create_ticket**: Requires subject, text, category ID, and contact details.

Create a new support ticket
- **get_ticket**: Get detailed information about a specific ticket
- **list_categories**: List all ticket categories
- **list_priorities**: List all available ticket priorities
- **list_staff**: List all staff members
- **list_statuses**: List all available ticket statuses
- **list_tickets**: Use query parameters for filtering/pagination.

List all support tickets in HappyFox
- **list_contacts**: List all contacts (users) in the help desk
- **search_tickets**: Search for tickets using a text query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HappyFox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending tickets in the 'General' category."

**🤖 AI Agent:**
> I've retrieved your tickets. You have 4 pending items in 'General', including 'Login issue' (ID: 102), 'Billing question' (ID: 105), and 'API feedback' (ID: 110). Which one would you like to update?

---

**👤 You:**
> "Add a staff update to ticket ID 102: 'Looking into this now'."

**🤖 AI Agent:**
> Update added! I've successfully logged your response to ticket 102. The customer will be able to see this in their support portal. Would you like to change the ticket status to 'In Progress'?

---

**👤 You:**
> "Create a new ticket for 'App crash on startup' in the Technical category."

**🤖 AI Agent:**
> Process started! I found the 'Technical' category (ID: 5). To create the ticket, I'll need the customer's name and email address. Could you provide those?


## ❓ FAQ

**Q: How do I find my HappyFox API credentials?**
Log in to HappyFox, go to **Manage > Integrations > API**. You will be able to generate your **API Key** and **Auth Code** from there.

**Q: What is the 'Account Name'?**
The Account Name is the subdomain used to access your HappyFox instance (e.g., if you log in at `company.happyfox.com`, your account name is `company`).

**Q: Can I add updates to existing tickets?**
Yes! Use the `add_staff_update` tool. You just need to provide the `ticket_id` and the text of your update. This will appear as a staff response in the help desk.

**Q: Is the integration secure for managing support data?**
Absolutely. The integration uses industry-standard HTTP Basic authentication over HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/happyfox](https://vinkius.com/mcp/happyfox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HappyFox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `happyfox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HappyFox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "happyfox": {
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
