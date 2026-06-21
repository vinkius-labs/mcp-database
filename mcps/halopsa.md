# HaloPSA MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/halopsa)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [helpdesk-ticketing](../categories/helpdesk-ticketing.md)

Automate service desk workflows via HaloPSA — manage tickets, clients, users, and assets directly from any AI agent.

## Description
Connect your **HaloPSA** instance to any AI agent and take full control of your service desk and PSA workflows through natural conversation.

### What you can do

- **Ticket Management** — List all tickets, retrieve detailed information, and create new support requests effortlessly.
- **Client & User Oversight** — Access lists of clients (customers) and users defined in your system to ensure data accuracy.
- **Asset Tracking** — Monitor the hardware and software assets managed within HaloPSA.
- **Team Coordination** — Browse your organizational teams and sites to facilitate better resource allocation.
- **Financial Insights** — Retrieve lists of invoices and customer contracts for quick status checks.
- **Action Execution** — Perform updates on tickets, add internal notes, or change statuses directly from the chat.

### How it works

1. Subscribe to this server
2. Enter your HaloPSA Client ID, Client Secret, Resource URL, and Auth URL
3. Start managing your service desk from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex PSA tabs. Your AI assistant acts as a dedicated Service Desk Coordinator or Operations Specialist.

### Who is this for?

- **Service Desk Agents** — instantly retrieve ticket details and add notes during customer interactions.
- **Operations Managers** — automate the process of checking asset lists and team assignments.
- **IT Directors** — maintain a real-time overview of support volume and contract statuses.


## Available Tools (11)
- **create_ticket**: Create a new ticket in HaloPSA
- **get_ticket**: Get detailed information about a specific ticket
- **list_assets**: List all assets defined in HaloPSA
- **list_clients**: List all clients (customers) in HaloPSA
- **list_contracts**: List all customer contracts
- **list_invoices**: List all invoices in HaloPSA
- **list_sites**: List all sites/locations
- **list_teams**: List all teams configured in the service desk
- **list_tickets**: List all tickets in HaloPSA
- **list_users**: List all users in the HaloPSA instance
- **perform_ticket_action**: Perform an action on a ticket (e.g., add note, change status)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HaloPSA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open tickets assigned to me."

**🤖 AI Agent:**
> I've retrieved your tickets. You currently have 3 open items: 'Internet connectivity issue' (ID: 1021), 'Printer setup request' (ID: 1025), and 'Software license renewal' (ID: 1030). Which one would you like to update?

---

**👤 You:**
> "Add an internal note to ticket ID 1021: 'Waiting for vendor feedback'."

**🤖 AI Agent:**
> Action performed! I've successfully added the internal note to ticket 1021. Would you like to change its status to 'On Hold' as well?

---

**👤 You:**
> "Show me the asset list for Client 'Acme Corp'."

**🤖 AI Agent:**
> Accessing assets... I found 5 assets linked to Acme Corp, including 3 Laptops (MacBook Pro), 1 Server (PowerEdge), and 1 Firewall (FortiGate). Shall I list the serial numbers for these items?


## ❓ FAQ

**Q: How do I set up my HaloPSA API credentials?**
Log in as an Administrator, go to **Configuration > Integrations > Halo API**. In 'View Applications', create a new app with the 'Agent' login type and grant the necessary permissions. You will receive your Client ID and Client Secret there.

**Q: What are the Resource and Auth URLs?**
The Resource URL is typically `https://your-tenant.halopsa.com/api` and the Auth URL is `https://your-tenant.halopsa.com/auth`. Replace 'your-tenant' with your actual HaloPSA instance name.

**Q: Can I perform actions on tickets, like changing status?**
Yes! Use the `perform_ticket_action` tool by providing the ticket ID and the specific action ID configured in your Halo instance. You can also add an optional note.

**Q: Is the integration secure?**
Yes, it uses industry-standard OAuth2 Client Credentials flow. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/halopsa](https://vinkius.com/mcp/halopsa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HaloPSA** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `halopsa` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HaloPSA** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "halopsa": {
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
