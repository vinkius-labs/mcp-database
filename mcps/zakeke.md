# Zakeke MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zakeke)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage customized product designs, 3D configurations, and orders via Zakeke.

## Description
Connect your **Zakeke** account to any AI agent to streamline your visual product customization and 3D configuration workflows. This MCP server enables your agent to interact with customer designs, 3D compositions, and specialized e-commerce orders directly.

### What you can do

- **Design Oversight** — List and retrieve detailed configurations for visual product designs created by your customers
- **3D Configuration Management** — Access pricing and attribute data for complex 3D product compositions
- **Order Synchronization** — Query and monitor orders containing customized products to ensure smooth fulfillment
- **Print-Ready Access** — Retrieve ZIP files of all output files for production-ready designs instantly
- **Cart Integration** — Get necessary technical data to add 3D configured products to any shopping cart

### How it works

1. Subscribe to this server
2. Enter your Zakeke API Key and API Secret
3. Start managing your customized product business from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Owners** — Monitor custom design trends and order statuses without logging into the dashboard
- **Production Managers** — Quickly retrieve print-ready files for fulfillment via natural language
- **Developers** — Integrate visual customization data and 3D configuration logic into custom applications effortlessly


## Available Tools (9)
- **get_cart_info**: Get cart information for a 3D configuration
- **list_compositions**: List all 3D product configurations
- **get_design_print_files**: Get ZIP file of print-ready outputs for a design
- **list_designs**: List all customer-created designs
- **get_composition_details**: Get details for a specific 3D configuration
- **get_design_details**: Get details for a specific design
- **get_order_details**: Get details for a specific order
- **list_orders**: List all customized product orders
- **list_products**: List all products available for customization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zakeke** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all visual designs created by customers today in Zakeke."

**🤖 AI Agent:**
> I've retrieved the latest designs. You have 12 new designs today, including a 'Custom Coffee Mug' and a 'Photo T-Shirt'. Would you like to see the details for any of them?

---

**👤 You:**
> "List my customized product orders from Zakeke."

**🤖 AI Agent:**
> I found 8 orders with customized items. Notable ones include Order #ZK-1001 and #ZK-1002. All are currently 'In Production'.

---

**👤 You:**
> "Get the print-ready ZIP for design ID 'DESIGN_12345'."

**🤖 AI Agent:**
> I've retrieved the production files for design 'DESIGN_12345'. You can download the ZIP archive containing high-resolution PDFs and vectors here.


## ❓ FAQ

**Q: How do I get the print-ready files for a customer design?**
Use the `get_design_print_files` tool with the design ID to retrieve the production-ready ZIP file metadata and URL.

**Q: Can I check the price of a 3D configuration for a specific quantity?**
Yes, the `get_composition_details` and `get_design_details` tools accept an optional `quantity` parameter to calculate updated pricing.

**Q: Is it possible to see all products available for customization?**
Absolutely. Use the `list_products` tool to retrieve the full catalog of items currently configured for customization in your Zakeke account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zakeke](https://vinkius.com/mcp/zakeke)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zakeke** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zakeke` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zakeke** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zakeke": {
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
