# Cart.com (AmeriCommerce) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cartcom-americommerce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

E-commerce store orchestration via Cart.com — manage products, orders, and customers via AI.

## Description
Connect your **AmeriCommerce (Cart.com)** store to your AI agent to unlock professional e-commerce orchestration. From managing product catalogs and tracking inventory to auditing orders and retrieving customer profiles, your agent handles your storefront operations through natural conversation.

### What you can do

- **Product Management** — List, search, and update products in your catalog to ensure your storefront is always current
- **Order Orchestration** — Retrieve incoming orders and update fulfillment statuses seamlessly
- **Customer Intelligence** — List and audit customer profiles to track purchase history and engagement
- **Category Oversight** — Manage product categories to keep your online store perfectly organized
- **E-commerce Insights** — Quickly identify pending orders or low-stock products directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Store Domain and Access Token (Single Token Flow)
3. Start managing your storefront and monitoring sales through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store Owners** — automate order audits and monitor inventory levels effortlessly
- **E-commerce Managers** — update product details and manage categories on the fly
- **Customer Support Teams** — quickly look up order statuses and customer history to resolve inquiries
- **Operations Specialists** — retrieve daily sales reports and synchronize data with external tools


## Available Tools (10)
- **list_products**: Supports pagination.

List store products
- **get_product_details**: Get product metadata
- **create_product**: Add a new product
- **list_orders**: List store orders
- **get_order_details**: Get order metadata
- **list_customers**: List customers
- **get_customer_details**: Get customer metadata
- **create_customer**: Add a new customer
- **list_categories**: List product categories
- **get_category_details**: Get category metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cart.com (AmeriCommerce)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending orders in my store."

**🤖 AI Agent:**
> I've retrieved your orders. You currently have 5 pending orders waiting for fulfillment. Would you like me to retrieve the order items for the most recent one?

---

**👤 You:**
> "Show the details for product ID '1001'."

**🤖 AI Agent:**
> I've retrieved the details for product 1001. It is the 'Premium Coffee Blend'. The current price is $24.99 and you have 150 units in stock. The status is set to active.

---

**👤 You:**
> "Search for a customer with email 'jane.smith@example.com'."

**🤖 AI Agent:**
> I've found the profile for Jane Smith (ID: 555). She has placed 3 orders in the past 6 months and is a member of the 'VIP Customers' group. Would you like to see her recent order history?


## ❓ FAQ

**Q: How do I find my AmeriCommerce API Token?**
Log in to your AmeriCommerce admin panel, navigate to **Tools** > **Apps & Addons**, and create a new application using the **Single Token Flow**. You will generate a non-expiring Access Token to use here.

**Q: Can I manage product categories via the agent?**
Yes! Use the `list_categories` tool to see your existing structure and `get_category_details` to retrieve metadata for a specific category.

**Q: Can I filter orders by status?**
Yes! Use the `list_orders` tool and provide the appropriate `order_status_id` parameter to filter for pending, shipped, or cancelled orders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cartcom-americommerce](https://vinkius.com/mcp/cartcom-americommerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cart.com (AmeriCommerce)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cartcom-americommerce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cart.com (AmeriCommerce)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cartcom-americommerce": {
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
