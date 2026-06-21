# CloudCart MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudcart)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage e-commerce and store operations via CloudCart — track products, monitor orders, and manage customers directly from any AI agent.

## Description
Connect your **CloudCart** account to any AI agent and take full control of your e-commerce operations through natural conversation. Streamline how you manage your product catalog and customer orders natively.

### What you can do

- **Product Oversight** — List and retrieve details for all products in your catalog including SKUs and prices natively
- **Order Intelligence** — Access and monitor customer orders, including fulfillment statuses flawlessly
- **Category Logistics** — List and manage store categories to keep your catalog organized securely
- **Customer Tracking** — Access registered customer profiles and their interaction history flawlessly
- **Abandoned Cart Auditing** — Retrieve a list of abandoned shopping carts to identify recovery opportunities flawlessly
- **Brand Visibility** — List all product brands configured in your store directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your CloudCart Client ID, Client Secret, and Store Domain
3. Start managing your store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor stock levels and order fulfillment using natural language
- **Store Owners** — audit abandoned carts and customer trends without opening the dashboard
- **Support Teams** — quickly look up order details and customer profiles straight from their chat interface
- **Marketing Teams** — verify product metadata and brand associations across the catalog


## Available Tools (8)
- **get_abandoned_carts**: Retrieve a list of abandoned shopping carts
- **get_order_store_details**: Get detailed information for a specific order
- **get_product_store_details**: Get detailed information for a specific product
- **list_store_brands**: List all product brands configured in the store
- **list_store_categories**: List all product categories in the store
- **list_store_customers**: List all registered customers in the store
- **list_store_orders**: List all customer orders in the store
- **list_store_products**: List all products in the store catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CloudCart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my CloudCart store."

**🤖 AI Agent:**
> Retrieving your product catalog... I found 5 items: 'Smartphone X' (SKU: SPX-01), 'Laptop Pro' (SKU: LP-2026), and 3 others. Would you like to see the inventory for any of these?

---

**👤 You:**
> "Show me the last 5 orders."

**🤖 AI Agent:**
> Checking recent orders... You have 5 new orders today. #1001 (Processing), #1002 (Shipped), #1003 (Paid), and 2 others. Total revenue from these is $850.00.

---

**👤 You:**
> "What is the status of order ID 'order_98765'?"

**🤖 AI Agent:**
> Retrieving details for order 98765... The order is currently 'Shipped' and was picked up by the courier yesterday. The customer has been notified.


## ❓ FAQ

**Q: Can I see a list of abandoned carts through the agent?**
Yes! Use the `get_abandoned_carts` tool. The agent will return all recent shopping sessions that were not completed, allowing you to plan recovery campaigns.

**Q: How do I check the stock status or SKU for a product?**
Use the `list_store_products` tool to see a summary, or `get_product_store_details` with the product ID for detailed inventory information.

**Q: Where do I find my CloudCart API credentials?**
Log in to your CloudCart admin panel, navigate to **Settings**, and select **API Keys**. You can generate a new Client ID and Client Secret there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudcart](https://vinkius.com/mcp/cloudcart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CloudCart** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudcart` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CloudCart** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudcart": {
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
