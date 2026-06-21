# NCR Voyix MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ncr-voyix)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage commerce and retail operations via NCR Voyix — track orders, sites, products, and inventory directly from your AI agent.

## Description
Connect your **NCR Voyix** (formerly NCR) commerce account to your AI agent and streamline your retail operations and catalog management through natural conversation.

### What you can do

- **Site Management** — List all physical and digital commerce sites and get detailed configuration info.
- **Order Tracking** — Access customer orders across all sites and retrieve complete metadata and line items.
- **Catalog & Product Oversight** — View all products, descriptions, and pricing in your global catalog.
- **Inventory Control** — Check real-time stock levels for any product at specific physical sites.
- **Customer & Loyalty** — List registered customers and monitor active loyalty and reward programs.
- **Catalog Discovery** — Browse all available product catalogs defined in your commerce system.

### How it works

1. Subscribe to this server
2. Enter your NCR API Key, Shared Secret, and Organization Number
3. Start managing your commerce data from Claude, Cursor, or any MCP client

### Who is this for?

- **Retail Managers** — quickly check inventory levels or site statuses without opening the NCR portal.
- **Operations Teams** — automate the retrieval of order data and customer info for daily reporting.
- **Catalog Managers** — verify product details and catalog structures through natural language commands.


## Available Tools
- **get_loyalty_programs**: List loyalty programs
- **get_order**: Get specific order info
- **get_product**: Get specific product details
- **get_site**: Get specific site details
- **list_catalogs**: List available catalogs
- **list_customers**: List commerce customers
- **list_inventory**: List site inventory levels
- **list_orders**: List commerce orders
- **list_products**: List catalog items (products)
- **list_sites**: List NCR commerce sites


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NCR Voyix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active commerce sites."

**🤖 AI Agent:**
> I've retrieved your sites. You have 5 active locations: 'Main Street flagship', 'Westside Mall', 'E-commerce Portal', and 2 others. Would you like the detailed configuration for the Westside Mall site?

---

**👤 You:**
> "Check the status of order ID ORD-98765."

**🤖 AI Agent:**
> Inspecting order ORD-98765... The current status is 'READY_FOR_PICKUP'. It was placed at the 'Westside Mall' site and contains 3 items totaling $45.50. Shall I list the specific items in this order?

---

**👤 You:**
> "What is the inventory level at site 'flagship-01'?"

**🤖 AI Agent:**
> Fetching inventory for 'flagship-01'... I found stock levels for 150 items. Notable counts include 'Summer T-Shirt' (45 units), 'Blue Jeans' (12 units - Low Stock), and 'White Sneakers' (88 units). Would you like to see all items currently in low stock?


## ❓ FAQ

**Q: How do I find my NCR Organization Number?**
Your Organization Number (nep-organization) is provided by NCR during your account onboarding. You can also find it in your NCR Cloud Developer Portal profile settings.

**Q: Can I check stock for a specific store?**
Yes! Use the `list_inventory` tool and provide the specific Site ID to see all current stock levels at that physical location.

**Q: What is the global catalog?**
The global catalog contains all the items and products your business offers across all sites. You can browse this master list using the `list_products` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ncr-voyix](https://vinkius.com/mcp/ncr-voyix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NCR Voyix** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ncr-voyix` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NCR Voyix** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ncr-voyix": {
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
