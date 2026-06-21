# ApparelMagic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apparelmagic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

ERP, PLM, and CRM for the apparel industry — manage styles, orders, inventory, and shipments via AI.

## Description
The **ApparelMagic MCP Server** provides powerful integration with your ApparelMagic Cloud ERP. Connect your account to your AI agent to streamline apparel manufacturing and distribution. Manage your entire product lifecycle, from initial styles to final shipments, using natural language.

### What you can do

- **Order Management** — List sales orders and retrieve detailed information including quantities and SKUs.
- **Inventory Visibility** — Check real-time stock levels for any product or style in your collection.
- **Customer Insights** — Access customer profiles and history to improve sales and support interactions.
- **Shipping & Fulfillment** — Track shipments and monitor fulfillment status directly from your chat.
- **Product Lifecycle** — Browse styles and products to manage your apparel collection efficiently.

### How it works

1. Subscribe to this server
2. Provide your ApparelMagic API Token and Account Subdomain
3. Start managing your apparel operations through your AI chat interface.

### Who is this for?

- **Fashion Brand Owners** — Monitor production and sales performance on the go.
- **Operations Managers** — Coordinate inventory and shipping tasks without manual report generation.
- **Sales & Support Teams** — Quickly look up customer and order details during client interactions.


## Available Tools
- **get_customer**: Get details for a specific customer
- **get_order**: Get details for a specific sales order
- **get_product**: Get details for a specific product
- **get_shipment**: Get details for a specific shipment
- **list_customers**: List customers from ApparelMagic
- **list_inventory**: List inventory levels from ApparelMagic
- **list_orders**: List sales orders from ApparelMagic
- **list_products**: List products/styles from ApparelMagic
- **list_shipments**: List shipments from ApparelMagic
- **list_styles**: List styles from ApparelMagic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ApparelMagic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 sales orders in ApparelMagic."

**🤖 AI Agent:**
> I've retrieved the latest 5 orders. Order #1001 for 'Global Retail' is currently 'Processing', while #1002 for 'Local Boutique' has been 'Shipped'.

---

**👤 You:**
> "What is the inventory level for SKU 'TSHIRT-BLUE-L'?"

**🤖 AI Agent:**
> I checked the inventory for 'TSHIRT-BLUE-L'. There are 150 units on hand, with 120 available for new orders (30 units are already allocated).

---

**👤 You:**
> "Show the details for customer 'CUST-889'."

**🤖 AI Agent:**
> Customer 'CUST-889' is 'Fashion Forward Inc'. They have a credit limit of $10,000 and their primary contact is Sarah Miller at sarah@fashionforward.com.


## ❓ FAQ

**Q: How do I get my ApparelMagic API Token?**
Log in to your ApparelMagic Cloud account, navigate to **Settings > API > Tokens**, and generate a new token. You will also need your account subdomain (e.g., 'yourbrand' in `yourbrand.app.apparelmagic.com`).

**Q: Does the API support real-time inventory updates?**
Yes, the `list_inventory` tool queries ApparelMagic's current stock records, allowing your AI agent to provide accurate availability information based on latest transactions.

**Q: Can I filter orders by their modification date?**
While the current MCP tools provide basic listing, you can ask your AI agent to 'find recent orders' and it will parse the results from ApparelMagic to identify newly created or updated records.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apparelmagic](https://vinkius.com/mcp/apparelmagic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ApparelMagic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `apparelmagic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ApparelMagic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apparelmagic": {
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
