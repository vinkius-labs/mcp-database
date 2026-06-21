# Fixably MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fixably)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage repair orders, track inventory, and handle customer data via AI agents with Fixably.

## Description
Connect your **Fixably** instance to any AI agent and automate your repair management workflows through the Model Context Protocol (MCP). Fixably provides a comprehensive platform for handling the entire repair lifecycle, from initial order creation to final dispatch. Now, you can manage your service center operations directly through natural conversation.

### What you can do

- **Order Management** — List all repair orders, fetch detailed order metadata, and create or update orders instantly.
- **Customer Oversight** — Access your customer database, retrieve specific profiles, and search for accounts by name or email.
- **Inventory Tracking** — List all stock locations and monitor product availability at specific inventory sites.
- **Operational Updates** — Post internal notes to orders and update the internal location of devices (e.g., from SERVICE to STORE).
- **Document Access** — List all files and attachments associated with a repair order for quick reference.
- **Real-time Monitoring** — Fetch specific order statuses or device locations to keep your service team and customers informed.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fixably Subdomain and API Token (found in User Settings > Integrations)
3. Start managing your repair operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Service Technicians** — quickly check order details or add repair notes without leaving your primary workspace.
- **Store Managers** — get a real-time overview of inventory across locations and update order statuses via simple AI commands.
- **Customer Support** — automate the retrieval of order updates and customer history to provide faster resolutions.


## Available Tools
- **add_order_note**: Add note to order
- **change_internal_location**: g. SERVICE, STORE).

Change device location
- **create_order**: Create a new order
- **get_customer**: Get customer details
- **get_order**: Get order details
- **get_stock**: Get stock details
- **list_customers**: List customers
- **list_order_files**: List files for order
- **list_orders**: List repair orders
- **list_stock_products**: List products in stock
- **list_stocks**: List inventory locations
- **update_order**: Update an order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fixably** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active repair orders in Fixably."

**🤖 AI Agent:**
> Fetching orders... I found 5 active repair orders, including 'Order #123' for an iPhone 13 and 'Order #456' for a MacBook Pro. Would you like the details for any of these?

---

**👤 You:**
> "Add a note to order '123': 'Diagnostic complete, waiting for replacement screen'."

**🤖 AI Agent:**
> Note added! Your update has been successfully posted to order '123'. Technicians and support staff will see this diagnostics update immediately.

---

**👤 You:**
> "Check the available stock at inventory location 'stock_abc'."

**🤖 AI Agent:**
> Checking inventory... At location 'stock_abc', you have several parts in stock, including 10 'LCD Assemblies' and 5 'Battery Modules'. Would you like the full product list?


## ❓ FAQ

**Q: How do I change the internal location of a device using the agent?**
You can use the 'change_internal_location' tool. Simply provide the Order ID and the new location string (e.g., 'SERVICE', 'STORE', or 'CUSTOMER'). The agent will update the record in Fixably immediately.

**Q: Can I see which products are available at a specific stock location?**
Yes! Use the 'list_stock_products' tool and provide the Stock ID. The agent will return a list of all products currently held at that specific inventory location.

**Q: How do I add an internal update to a repair order?**
Use the 'add_order_note' tool. You'll need the Order ID and the text of your note. This allows you to document repair progress or internal findings directly from your chat interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fixably](https://vinkius.com/mcp/fixably)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fixably** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fixably` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fixably** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fixably": {
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
