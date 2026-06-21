# Unleashed MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unleashed)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate inventory, assemblies, and customer management via Unleashed — query BOMs, list invoices, and manage customers directly from any AI agent.

## Description
Connect your **Unleashed Software** account to any AI agent and take full control of your inventory, production, and sales workflows through natural conversation.

### What you can do

- **Production & Assemblies** — List, inspect, and create assemblies, or query Bills of Materials (BOM) to streamline your manufacturing processes.
- **Customer Management** — Retrieve customer lists, inspect deep profile details, and create new customer accounts on the fly.
- **Sales & Invoicing** — Monitor sales invoices, list credit notes, and keep track of financial accounts and currencies.
- **Company Overview** — Instantly fetch core company information and configured attribute sets to maintain data consistency.

### How it works

1. Subscribe to this server
2. Enter your Unleashed API ID and API Key
3. Start managing your inventory and production workflows from Claude, Cursor, or any MCP-compatible client

No more jumping between tabs to check stock levels, assembly statuses, or customer details. Your AI acts as a dedicated operations assistant.


## Available Tools
- **list_accounts**: List financial accounts
- **list_assemblies**: List assemblies
- **list_attribute_sets**: List attribute sets
- **list_boms**: List Bill of Materials
- **get_company**: Get company information
- **create_assembly**: Create a new assembly
- **create_customer**: Create a new customer
- **create_product**: Create a new product
- **create_purchase_order**: Create a new purchase order
- **create_sales_order**: Create a new sales order
- **list_credit_notes**: List credit notes
- **list_currencies**: List currencies
- **list_customer_delivery_addresses**: List customer delivery addresses
- **list_customers**: List customers
- **get_assembly**: Get a specific assembly
- **get_bom**: Get a specific Bill of Materials
- **get_customer**: Get a specific customer
- **get_invoice**: Get a specific sales invoice
- **get_product**: Get a specific product
- **get_purchase_order**: Get a specific purchase order
- **get_sales_order**: Get a specific sales order
- **get_stock_on_hand**: Get stock on hand for a specific product
- **get_supplier**: Get a specific supplier
- **list_invoices**: List sales invoices
- **list_product_brands**: List product brands
- **list_product_groups**: List product groups
- **list_product_prices**: List product prices
- **list_products**: List products
- **list_purchase_orders**: List purchase orders
- **list_recost_adjustments**: List recost adjustments
- **list_sales_orders**: List sales orders
- **list_sales_quotes**: List sales quotes
- **list_sales_shipments**: List sales shipments
- **list_salespersons**: List salespersons
- **list_sell_price_tiers**: List sell price tiers
- **list_stock_adjustments**: List stock adjustments
- **list_stock_counts**: List stock counts
- **list_stock_on_hand**: List stock on hand
- **list_supplier_returns**: List supplier returns
- **list_suppliers**: List suppliers
- **list_unit_of_measures**: List unit of measures
- **list_warehouse_stock_transfers**: List warehouse stock transfers
- **list_warehouses**: List warehouses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unleashed** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first page of our customers in Unleashed."

**🤖 AI Agent:**
> I've retrieved your customers. Currently, you have active accounts including 'Global Trade Ltd' (GUID: 8a7b6c) and 'Apex Retail' (GUID: 5f4e3d). Would you like to inspect any of these specifically?

---

**👤 You:**
> "Create a new customer with code 'CUST-999' and name 'Delta Industries'."

**🤖 AI Agent:**
> I have successfully created the customer 'Delta Industries' with code 'CUST-999'. The newly generated GUID is '9a8b7c6d-5e4f-3a2b-1c0d'. Let me know if you need to add delivery addresses or other details.

---

**👤 You:**
> "Get the details for assembly GUID 12345-abcde-67890."

**🤖 AI Agent:**
> Retrieving assembly details... Assembly '12345-abcde-67890' is currently 'In Progress'. It is assembling 50 units of 'Premium Widget' using BOM 'BOM-004'. No quality issues have been flagged.


## ❓ FAQ

**Q: How do I fetch the details of a specific Bill of Materials (BOM)?**
You can use the `get_bom` tool by providing the unique GUID of the Bill of Materials. The agent will return the complete component list and configuration details.

**Q: Can I create a new customer directly through my AI agent?**
Yes! Use the `create_customer` tool. You will need to provide a unique `CustomerCode` and a `CustomerName`, along with any optional fields you wish to populate.

**Q: How can I monitor active assembly processes?**
You can list all assemblies using `list_assemblies` (supporting pagination) or fetch a specific one using `get_assembly` with its GUID to check its status and progress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unleashed](https://vinkius.com/mcp/unleashed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unleashed** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `unleashed` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unleashed** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unleashed": {
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
