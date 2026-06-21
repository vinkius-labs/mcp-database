# ShippingBo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shippingbo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate your e-commerce logistics with order management, warehouse operations, and carrier integration for French retailers.

## Description
Connect your **ShippingBo** account to any AI agent and take full control of your e-commerce logistics and fulfillment orchestration through natural conversation. ShippingBo provides a comprehensive platform for centralizing orders, managing multi-warehouse stocks, and orchestrating shipments directly from your chat interface.

### What you can do

- **Order & Fulfillment Orchestration** — List and retrieve detailed metadata for your sales orders to keep your fulfillment pipeline synchronized programmatically.
- **Product & Stock Management** — Access and monitor your product catalog and update stock counts for specific items directly from the AI interface.
- **Shipment Lifecycle Control** — List and monitor shipments and track delivery progress via natural language to ensure customer satisfaction.
- **Warehouse Slot Intelligence** — Access and monitor warehouse slots to maintain a clear overview of your physical storage organization.
- **Operational Monitoring** — Track system activity and monitor packs to ensure your logistics setup is always optimized using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your ShippingBo API User, Token, and Version from your dashboard
3. Start managing your e-commerce logistics from Claude, Cursor, or any MCP-compatible client

No more manual stock checks or order hunting. Your AI acts as a dedicated logistics manager or fulfillment coordinator.

### Who is this for?

- **E-commerce Logistics Managers** — quickly retrieve order details and monitor multi-warehouse stocks without switching apps.
- **Warehouse Operations Teams** — automate the update of stock counts and monitor shipment progress via natural conversation.
- **Customer Success Teams** — streamline the retrieval of shipment metadata and coordinate order fulfillments directly within the chat.


## Available Tools (8)
- **get_order**: Get order details
- **get_product**: Get product details
- **list_orders**: List all orders
- **list_packs**: List packaging options
- **list_products**: List all products
- **list_shipments**: List all shipments
- **list_warehouse_slots**: List warehouse storage slots
- **update_stock**: Update product stock level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShippingBo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my ShippingBo catalog."

**🤖 AI Agent:**
> I've retrieved your product catalog. You have 125 active SKUs including 'Summer T-Shirt (Blue)', 'Wireless Headphones', and 'Eco Water Bottle'. Which one would you like to check stock for?

---

**👤 You:**
> "Update stock for product ID 54321 to 150 units."

**🤖 AI Agent:**
> Stock update processed! Product 54321 now has 150 units in your main warehouse. Should I verify if any pending orders can now be fulfilled?

---

**👤 You:**
> "List the last 5 shipments in ShippingBo."

**🤖 AI Agent:**
> Retrieving shipments... Your last 5 shipments include 'SH-9901' (Delivered), 'SH-9902' (In Transit), and three others. Would you like to see the tracking progress for the one in transit?


## ❓ FAQ

**Q: Can my AI automatically update the stock count for a specific product just by providing its ID?**
Yes! Use the `update_stock` tool. Provide the Product ID and the new stock count, and your agent will synchronize it across your ShippingBo warehouses instantly.

**Q: How do I monitor the status of warehouse slots to see how my inventory is organized?**
Simply ask the agent to run the `list_warehouse_slots` action. It will retrieve the full list of storage slots configured in your ShippingBo account.

**Q: How do I find my ShippingBo API credentials?**
Log in to your ShippingBo account, navigate to **Settings** > **API**, and you will find your unique **API User** (X-API-USER) and **Token** (X-API-TOKEN) there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shippingbo](https://vinkius.com/mcp/shippingbo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ShippingBo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shippingbo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ShippingBo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shippingbo": {
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
