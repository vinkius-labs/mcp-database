# Channable MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/channable)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage marketplace orders and stock via Channable — track sales, update shipments, and monitor returns directly from any AI agent.

## Description
Connect your **Channable** account to any AI agent and orchestrate your marketplace order management and stock synchronization through natural conversation. Streamline how you sell across Amazon, eBay, bol.com, and more.

### What you can do

- **Order Fulfillment** — List and retrieve details for orders from all connected marketplaces natively
- **Stock Synchronization** — Update product stock levels across all channels to prevent overselling flawlessly
- **Shipment Tracking** — Update order statuses and send tracking information back to marketplaces securely
- **Returns Oversight** — List and manage customer returns directly from your chat interface flawlessly
- **Project Visibility** — Access and monitor multiple projects and connected channels in real-time
- **Commerce Intelligence** — Retrieve detailed order metadata and project summaries directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Channable API Token and Company ID
3. Start managing your marketplace sales from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor sales performance across multiple channels using natural language
- **Operations Teams** — update stock and shipments without opening the Channable dashboard
- **Customer Support** — quickly look up order details and return statuses straight from their chat interface
- **Logistics Coordinators** — verify shipment information and tracking numbers for marketplace orders


## Available Tools (8)
- **get_order_details**: Get detailed information for a specific order
- **get_project_summary**: Get summary details for a specific project
- **list_connected_channels**: List connected marketplace channels for a project
- **list_marketplace_orders**: List orders from connected marketplaces for a project
- **list_channable_projects**: List all projects for the company
- **list_customer_returns**: List customer returns for a specific project
- **list_order_shipments**: List shipments and tracking info for a project
- **update_product_stock**: Update stock levels for products in a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Channable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 10 orders from all marketplaces."

**🤖 AI Agent:**
> Retrieving recent orders... I found 10 items including Order #ABC (Amazon), #DEF (bol.com), and #GHI (eBay). Which one would you like to see details for?

---

**👤 You:**
> "Update stock for SKU 'TSHIRT-L-RED' to 25 units in project 123."

**🤖 AI Agent:**
> Updating stock for 'TSHIRT-L-RED'... The stock has been successfully updated to 25 units in project 123 and will be synced to all connected channels.

---

**👤 You:**
> "List all active channels for project 456."

**🤖 AI Agent:**
> Checking channels for project 456... You have 4 active channels: Amazon US, eBay UK, Zalando DE, and Google Shopping. All are currently 'Healthy'.


## ❓ FAQ

**Q: Can I update stock for multiple products at once?**
Yes! Use the `update_product_stock` tool. You can provide an array of SKU IDs and their new stock levels, and the agent will sync them across Channable.

**Q: How do I see orders from a specific marketplace like Amazon?**
Use the `list_marketplace_orders` tool with your project ID. The agent will return all recent orders, and you can see the originating channel (e.g., Amazon, eBay) for each.

**Q: Where do I find my Channable API Token?**
Log in to Channable, go to 'Company Settings' in the sidebar, and then select 'Channable API'. You can generate and copy your token from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/channable](https://vinkius.com/mcp/channable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Channable** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `channable` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Channable** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "channable": {
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
