# Track-POD MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/track-pod)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Optimize delivery routes, capture electronic proof of delivery, and track driver performance for logistics operations.

## Description
Connect your **Track-POD** delivery automation account to any AI agent and simplify how you coordinate your logistics, track orders, and manage your fleet through natural conversation.

### What you can do

- **Order Management** — List all delivery orders and create new unscheduled tasks with client details and addresses.
- **Route Oversight** — List and monitor active or planned delivery routes to ensure on-time fulfillment.
- **Fleet Coordination** — Query your directory of drivers and vehicles to understand availability and distribution.
- **Real-time Tracking** — Fetch detailed metadata for specific orders using their unique order numbers.
- **Operational Monitoring** — Verify API connectivity and check rate limits directly from the agent.
- **Logistics Insights** — Retrieve high-level summaries of your delivery ecosystem status.

### How it works

1. Subscribe to this server
2. Enter your Track-POD API Key (found in your settings under API)
3. Start managing your delivery machine from Claude, Cursor, or any MCP client

### Who is this for?

- **Logistics Managers** — quickly check route statuses and verify order metadata via simple AI commands.
- **Dispatchers** — create new orders and coordinate driver lists directly from the workspace.
- **Operations Teams** — monitor fleet availability and track delivery progress in real-time via the AI assistant.


## Available Tools
- **create_order**: Requires order number and client name.

Create a new delivery order
- **get_order_by_number**: Get details for a specific order
- **list_drivers**: List all drivers
- **list_orders**: List all Track-POD orders
- **list_routes**: List delivery routes
- **list_vehicles**: List all vehicles
- **test_api_connection**: Test API key and connection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Track-POD** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active delivery routes in my account."

**🤖 AI Agent:**
> I've retrieved your routes. You have 3 active delivery paths: 'Downtown Morning', 'North Sector Express', and 'Warehouse Transfer'. Which one would you like to monitor?

---

**👤 You:**
> "Show me the details for order #ORD-8823."

**🤖 AI Agent:**
> I've fetched the metadata for order #ORD-8823. The status is 'In Transit', assigned to driver 'Mike Miller' on the 'Downtown Morning' route. The expected delivery time is 11:30 AM.

---

**👤 You:**
> "Create a new order #ORD-9902 for 'Tech Solutions' at '123 Main St'."

**🤖 AI Agent:**
> Success! Order #ORD-9902 has been created for 'Tech Solutions' at the provided address. It is currently unscheduled. Would you like me to check the driver availability for dispatching?


## ❓ FAQ

**Q: Can I see all the orders for a specific client?**
Yes! Use the `list_orders` tool. While it returns the full list, you can ask the AI agent to filter or identify all records matching a specific client name.

**Q: How do I create a new delivery order via AI?**
Use the `create_order` tool. You'll need to provide an Order Number, the Client Name, and an optional delivery address to register the new task in Track-POD.

**Q: Is it possible to list all the drivers currently available in the fleet?**
Absolutely. Use the `list_drivers` query. The agent will retrieve the complete directory of delivery drivers associated with your account, helping you coordinate assignments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/track-pod](https://vinkius.com/mcp/track-pod)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Track-POD** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `track-pod` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Track-POD** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "track-pod": {
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
