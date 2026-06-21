# Atera MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/atera)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage IT operations with Atera — track agents, tickets, and customers via AI.

## Description
The **Atera MCP Server** provides your AI agent with a powerful interface to your IT management platform. Streamline your MSP or IT department operations by monitoring remote agents, managing support tickets, and auditing customer data using simple natural language.

### Key Features

- **Agent Monitoring** — List and retrieve detailed information about monitored devices, including OS, IP addresses, and real-time statuses.
- **Helpdesk Management** — Create, list, and audit support tickets to ensure timely resolution of IT issues.
- **Customer & Contact Oversight** — Access your organizational structure, including customers (companies) and individual end-user contacts.
- **Alert Tracking** — Monitor recent system alerts to proactively identify and address potential hardware or software failures.
- **Inventory Intelligence** — Quickly audit your IT inventory without navigating complex web dashboards.
- **Secure API Integration** — Uses your Atera `X-API-KEY` for safe and authenticated communication with your IT data.

### Who is this for?

- **IT Administrators** — Quickly check server or workstation statuses and manage support queues using AI.
- **MSP Technicians** — Monitor alerts and update ticket statuses directly from your chat interface.
- **Operations Managers** — Retrieve customer and contact data for reporting and strategic planning.


## Available Tools (9)
- **create_ticket**: Create a new support ticket
- **get_account_check**: Verify Atera account connection
- **get_agent**: Get details for a specific agent
- **get_customer**: Get details for a specific customer
- **get_ticket**: Get details for a specific ticket
- **list_agents**: List all monitored agents (devices) in Atera
- **list_alerts**: List recent system alerts
- **list_customers**: List all customers (organizations)
- **list_tickets**: List all support tickets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Atera** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active IT agents in Atera."

**🤖 AI Agent:**
> I've retrieved your agents. You have 45 monitored devices, with 42 currently online and 3 offline.

---

**👤 You:**
> "Show me the last 5 support tickets created."

**🤖 AI Agent:**
> I've found the 5 most recent tickets. The latest is 'VPN Connection Issue' (ID: 1234) with High priority, created for 'Acme Corp'.

---

**👤 You:**
> "Check for any active system alerts."

**🤖 AI Agent:**
> There are 2 active alerts: a 'Disk Space Low' warning for 'Server-01' and a 'Service Offline' alert for 'Web-Gateway'.


## ❓ FAQ

**Q: How do I find my Atera API Key?**
Log in to Atera, go to **Admin > Data Management > API**, and you can generate and copy your API Key there.

**Q: What is an 'Agent ID'?**
An Agent ID is a unique numeric identifier for a device monitored by Atera. You can find these IDs by using the `list_agents` tool.

**Q: Can I create a ticket for a specific customer?**
Yes, use the `create_ticket` tool and provide the optional `customerId` parameter to link the ticket to a specific organization in your Atera account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/atera](https://vinkius.com/mcp/atera)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Atera** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `atera` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Atera** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "atera": {
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
