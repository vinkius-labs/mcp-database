# WorkWave MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workwave)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage service orders, customer accounts, and field technicians on WorkWave — the field service management platform.

## Description
Connect your **WorkWave Service** account to any AI agent and manage your field service operations through natural conversation.

### What you can do

- **Service Orders** — Browse and list all work requests, retrieve full details for specific orders, and update lifecycle statuses (e.g., InProgress, Completed)
- **Customer Accounts** — List all field service accounts and retrieve comprehensive details including contact info, billing history, and service locations
- **Field Personnel** — List all registered technicians and field staff, and retrieve profile details to check roles, skills, and contact info
- **Equipment Inventory** — Monitor and audit managed assets and equipment used across your field service operations directly from your agent
- **Site Discovery** — Retrieve physical service locations and job site addresses, including geographical coordinates for routing purposes
- **Operational Insights** — Quickly find unique account, order, employee, and location IDs required for automated field service workflows
- **Health Monitoring** — Verify the connectivity and status of your WorkWave API integration to ensure real-time data sync

### How it works

1. Subscribe to this server
2. Enter your WorkWave API Key
3. Start managing your field operations through Claude, Cursor, or any MCP-compatible client

No more manual digging through complex dispatching dashboards to check a job status. Your AI agent becomes your field service coordinator.

### Who is this for?

- **Dispatchers & Schedulers** — monitor job queues and update service order statuses through simple chat commands
- **Operations Managers** — audit customer accounts, verify technician profiles, and manage equipment inventory without manual navigation
- **Service Technicians** — quickly lookup order details and site locations while on the go through conversation
- **Customer Support Teams** — retrieve account billing history and service status to provide rapid assistance to field customers


## Available Tools
- **get_account_details**: Retrieves details for a specific customer account
- **get_api_health**: Checks the health and connectivity of the WorkWave API integration
- **get_employee_profile**: Retrieves profile details for a specific employee
- **get_order_details**: Retrieves details for a specific service order
- **list_field_service_accounts**: Lists customer accounts in the WorkWave Service platform
- **list_field_employees**: Lists technicians and field staff registered in WorkWave
- **list_service_equipment**: Lists managed equipment and assets used in field service
- **list_service_locations**: Lists physical service locations and job sites
- **list_service_orders**: Lists service orders and work requests
- **update_order_status**: g. mark as Pending, InProgress, or Completed).

Updates the lifecycle status of a service order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WorkWave** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active service orders in WorkWave."

**🤖 AI Agent:**
> I found 8 active service orders: 1. #ORD-101 (Status: Pending), 2. #ORD-102 (Status: InProgress), 3. #ORD-103 (Status: Pending), and 5 others. Which one would you like to see the details for?

---

**👤 You:**
> "Update order #ORD-101 status to 'InProgress'."

**🤖 AI Agent:**
> Success! I've updated the status of service order #ORD-101 to 'InProgress'. The change is now reflected in your WorkWave dashboard.

---

**👤 You:**
> "Find the profile for technician ID 'tech-555'."

**🤖 AI Agent:**
> Profile for tech-555: Name: Alice Johnson, Role: Senior Technician, Skills: HVAC, Electrical, Plumbing. Contact: alice@example.com. Would you like me to check her current assigned jobs?


## ❓ FAQ

**Q: Can I update the status of a work order through the agent?**
Yes. The `update_order_status` tool allows your AI agent to change the lifecycle status of any service order (e.g., to 'InProgress' or 'Completed') so you can manage dispatching directly through chat.

**Q: How do I see the contact details for a field technician?**
You can use the `get_employee_profile` tool. Simply provide the unique employee ID, and your agent will return their full profile details, including contact information and assigned skills.

**Q: Is it possible to list all service locations for a customer?**
Absolutely. Using the `list_service_locations` tool, you can retrieve a list of all physical sites and addresses registered in your WorkWave instance, helping you coordinate where jobs need to be performed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workwave](https://vinkius.com/mcp/workwave)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WorkWave** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `workwave` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WorkWave** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workwave": {
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
