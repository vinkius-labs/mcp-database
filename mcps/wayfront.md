# Wayfront MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wayfront)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage your parking operations with digital permits, enforcement tracking, and revenue analytics for parking facility operators.

## Description
Connect your **Wayfront** client portal (SPP) to any AI agent and streamline your service delivery workflows through natural conversation.

### What you can do

- **Client Management** — List all clients, retrieve detailed profile metadata, and create new client accounts programmatically
- **Order Tracking** — Query active orders, check their status, and update order progress directly from your agent
- **Billing & Invoices** — Monitor generated invoices to stay on top of your accounts receivable
- **Service Catalog** — List the services and products available in your portal
- **Ticketing** — Retrieve support tickets to monitor client communication and satisfaction
- **Team Overview** — List teams and departments to understand your internal structure

### How it works

1. Subscribe to this server
2. Enter your Wayfront Subdomain and API Key
3. Start managing your client portal resources from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **create_client**: Create a new client
- **get_client**: Get details for a specific client
- **get_order**: Get details for a specific order
- **list_clients**: List Wayfront clients
- **list_invoices**: List all Wayfront invoices
- **list_orders**: List Wayfront orders
- **list_services**: List available services
- **list_teams**: List organizational teams
- **list_tickets**: List support tickets
- **update_order**: Update an existing order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wayfront** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active orders in my Wayfront portal."

**🤖 AI Agent:**
> I've retrieved your orders. You have 8 active orders, including 'Order #1001' (Status: In Progress) and 'Order #1002' (Status: Pending Review). Which one would you like more details on?

---

**👤 You:**
> "Find support tickets from last week."

**🤖 AI Agent:**
> Analyzing tickets... I found 5 tickets from last week. Notable ones include 'Issue with billing' from client Alice and 'Login problem' from client Bob. Would you like the full text of Alice's ticket?

---

**👤 You:**
> "Get details for client '123'."

**🤖 AI Agent:**
> Client '123' is Marcus R. (marcus@example.com). They have 3 active orders and have been a client since Jan 2024. Their primary contact is through the portal dashboard.


## ❓ FAQ

**Q: Can I list all my clients from Wayfront using my AI agent?**
Yes! Use the `list_clients` tool. It will return a comprehensive list of all clients registered in your portal.

**Q: How do I check the status of a specific order?**
Simply provide the Order ID to the `get_order` tool. Your agent will fetch the full metadata, including its current status and client details.

**Q: Is it possible to update the status of an order through this integration?**
Yes, you can use the `update_order` action. Provide the Order ID and the new status to modify the record directly from your conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wayfront](https://vinkius.com/mcp/wayfront)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wayfront** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wayfront` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wayfront** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wayfront": {
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
