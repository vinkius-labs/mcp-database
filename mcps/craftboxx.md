# Craftboxx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/craftboxx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Equip your AI agent to manage craft orders, appointments, and resources directly via the Craftboxx API.

## Description
Integrate **Craftboxx**, the specialized software for craft businesses, directly into your AI workflow. Manage your orders, schedule field appointments, and track company resources using natural language.

### What you can do

- **Order Management** — List and retrieve details for craft orders, and create new orders instantly.
- **Appointment Scheduling** — Monitor field work appointments and employee schedules.
- **Resource Tracking** — Manage vehicles, machines, and material inventory via chat.
- **Business Insights** — Get real-time statistics on your company's performance and task status.

### How it works

1. Connect the Craftboxx integration to your AI assistant.
2. Authorize using your Craftboxx API Key (found in Settings > API).
3. Optimize your craft business operations through intuitive conversation.

### Who is this for?

- **Craft Business Owners** — Get a quick overview of active orders and business stats on the go.
- **Operations Managers** — Coordinate employee schedules and resource allocation efficiently.
- **Project Leads** — Quickly check order details and material availability during planning.


## Available Tools
- **create_order**: Create a new craft order
- **get_business_stats**: Retrieve high-level statistics for your business
- **get_order_details**: Get details for a specific craft order
- **list_appointments**: List scheduled appointments and field work
- **list_customers**: List customers and business partners
- **list_employees**: List all employees and team members
- **list_materials**: List materials and inventory items
- **list_orders**: List all craft orders in Craftboxx
- **list_vehicles_resources**: List vehicles, machines, and other resources
- **list_tasks**: List all open and completed tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Craftboxx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active craft orders for this week."

**🤖 AI Agent:**
> I've found 5 active orders for this week, including 'Roof Repair - Main St' and 'Electrical Wiring - Office Block'. Would you like to see the assigned employees for these?

---

**👤 You:**
> "Show me the appointments scheduled for tomorrow."

**🤖 AI Agent:**
> Tomorrow you have 3 appointments: 08:00 - Customer Consultation (ID: 123), 11:30 - Site Survey (ID: 124), and 15:00 - Maintenance Check (ID: 125). Should I provide details for any of them?

---

**👤 You:**
> "What is the status of company vehicle 'Sprinter - B-CX 101'?"

**🤖 AI Agent:**
> The vehicle 'Sprinter - B-CX 101' is currently 'Available' and located at the 'Central Depot'. Its last maintenance was on February 10th. Would you like to assign it to a new order?


## ❓ FAQ

**Q: How do I get a Craftboxx API Key?**
Log in to your Craftboxx account, navigate to **Settings > API**, and you can generate or retrieve your API Key from that section.

**Q: Can I assign tasks to employees?**
Yes, you can use the create_order tool or list employees to see who is available and manage task distribution through conversational commands.

**Q: Does Craftboxx support resource management?**
Yes, the integration allows you to list company resources like vehicles and machines, helping you track their allocation to different orders or appointments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/craftboxx](https://vinkius.com/mcp/craftboxx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Craftboxx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `craftboxx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Craftboxx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "craftboxx": {
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
