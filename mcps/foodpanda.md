# Foodpanda MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/foodpanda)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate food delivery operations via Foodpanda — manage vendor catalogs, track orders, and control restaurant status directly from any AI agent.

## Description
Connect your **Foodpanda Partner** account to any AI agent and take full control of your food delivery operations through natural conversation.

### What you can do

- **Vendor Catalog Management** — Fetch, update, and export complete product catalogs for any restaurant in your chain
- **Category Organization** — List and manage vendor categories to organize menu items efficiently
- **Order Tracking** — Retrieve order details and full order history with date range filtering
- **Order Management** — Update order status and details in real-time
- **Promotion Control** — Create, update, and monitor promotional campaigns across your chain
- **Vendor Status** — Check and update operational status (open, closed, busy) for any vendor
- **Catalog Jobs** — Monitor async catalog update and product addition jobs

### How it works

1. Subscribe to this server
2. Enter your Foodpanda Partner API OAuth 2.0 Bearer token
3. Start managing your delivery operations from Claude, Cursor, or any MCP-compatible client

No more logging into multiple vendor portals or manually updating menus. Your AI acts as a dedicated operations manager.

### Who is this for?

- **Restaurant Chains** — instantly update menus, check order volumes, and manage vendor status across multiple locations
- **Operations Managers** — monitor promotions, track orders, and handle vendor status changes without switching platforms
- **Delivery Coordinators** — fetch order details and history directly from your workflow to optimize dispatching


## Available Tools (13)
- **update_vendor_status**: g., open, closed, busy).

Update vendor status on Foodpanda
- **add_catalog_products**: Add products to chain catalog on Foodpanda
- **get_catalog_job**: Get catalog job status on Foodpanda
- **export_catalog**: Export vendor catalog on Foodpanda
- **get_order_details**: Get order details from Foodpanda
- **get_order_history**: Get order history for a vendor on Foodpanda
- **get_promotion_job**: Get promotion job status on Foodpanda
- **update_vendor_catalog**: Update vendor catalog on Foodpanda
- **update_order**: Update an order on Foodpanda
- **upsert_promotion**: Create or update a promotion on Foodpanda
- **get_vendor_catalog**: Get vendor catalog from Foodpanda
- **get_vendor_categories**: Get vendor categories from Foodpanda
- **get_vendor_status**: Get vendor status from Foodpanda


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Foodpanda** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the complete catalog for vendor 12345 in chain 67890."

**🤖 AI Agent:**
> I've fetched the vendor catalog. This restaurant has 45 active products across 8 categories, including burgers, sides, and beverages. The most popular item is the Classic Burger combo.

---

**👤 You:**
> "What's the status of order ORD-98765?"

**🤖 AI Agent:**
> Order ORD-98765 is currently being prepared. It was placed at 14:32 with 3 items: 2x Classic Burger, 1x Fries Large. Estimated delivery time is 25 minutes.

---

**👤 You:**
> "Set vendor 12345 to busy status due to high order volume."

**🤖 AI Agent:**
> Done! Vendor 12345 is now set to 'busy' status. Customers will see an extended delivery time estimate. The reason 'high order volume' has been recorded.


## ❓ FAQ

**Q: How do I get my Foodpanda Partner API access token?**
After being approved on the Foodpanda Partner Portal, you'll receive OAuth 2.0 Client Credentials. Use the `getAuthToken` flow with your client_id and client_secret to obtain a JWT Bearer token. This token is what you paste into the credential field.

**Q: Can I update my restaurant menu directly through this integration?**
Yes! Use the `update_vendor_catalog` tool with the chain_id, vendor_id, and a JSON array of products. You can also use `add_catalog_products` to add specific items to your chain catalog.

**Q: What is the API rate limit for Foodpanda Partner API?**
The Foodpanda Partner API has a rate limit of 50 requests per minute. The integration handles this automatically, but if you're doing bulk operations, be mindful of this constraint.

**Q: Can I temporarily close a restaurant via the API?**
Yes, you can update the operational status using `update_vendor_status` to close or set the restaurant as busy to prevent new orders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/foodpanda](https://vinkius.com/mcp/foodpanda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Foodpanda** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `foodpanda` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Foodpanda** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foodpanda": {
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
