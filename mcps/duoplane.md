# Duoplane MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/duoplane)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage multi-vendor orders, track purchase orders, and monitor vendor inventory via the Duoplane API.

## Description
Integrate **Duoplane**, the leading multi-vendor e-commerce automation platform, directly into your AI workflow. Manage your customer orders across multiple storefronts, track purchase orders sent to vendors, monitor vendor profiles and connection statuses, and oversee your synchronized product catalog using natural language.

### What you can do

- **Order Oversight** — List and retrieve detailed information and status for all your customer orders and their associated fulfillment stages.
- **Purchase Order Intelligence** — Monitor purchase orders sent to vendors, including tracking numbers and real-time fulfillment history.
- **Vendor Management** — Access and monitor all drop-ship and wholesale vendors, resolving connection statuses and order routing settings.
- **Inventory Auditing** — Retrieve high-level summaries of synchronized products, vendor activity, and inventory counts across your organization.

### How it works

1. Connect the Duoplane integration to your AI assistant.
2. Authorize using your Duoplane API Key, API Password (typically 'X'), and subdomain.
3. Orchestrate your multi-vendor fulfillment and e-commerce automation through intuitive conversation.

### Who is this for?

- **E-commerce Managers** — Quickly check order fulfillment statuses and vendor responsiveness on the go.
- **Supply Chain Leads** — Monitor purchase order volumes and vendor inventory counts via chat.
- **Operations Teams** — Research specific order details and organizational fulfillment metadata instantly.


## Available Tools
- **get_duoplane_account_metadata**: Retrieve metadata for the current Duoplane subdomain
- **get_order_details**: Get detailed information and status for a specific customer order
- **get_purchase_order_details**: Get detailed information for a specific purchase order
- **quick_vendor_inventory_audit**: Retrieve a high-level summary of vendor activity and product counts
- **get_vendor_profile**: Get detailed profile and configuration for a specific vendor
- **list_ecommerce_orders**: List all customer orders in your Duoplane account
- **list_purchase_orders**: List all purchase orders (POs) sent to vendors
- **list_unfulfilled_purchase_orders**: Identify purchase orders that are currently awaiting fulfillment by vendors
- **list_synced_products**: List all products synchronized across your vendors and storefronts
- **list_active_vendors**: List all drop-ship and wholesale vendors registered in your Duoplane account
- **search_orders_by_reference**: Search for orders using a keyword or reference identifier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Duoplane** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all unfulfilled purchase orders."

**🤖 AI Agent:**
> I've found 5 unfulfilled purchase orders, including PO-9988 sent to 'Vendor A' and PO-7766 sent to 'Vendor B'. Would you like to see the items for PO-9988?

---

**👤 You:**
> "Show me the details for customer order '12345'."

**🤖 AI Agent:**
> Order '12345' (External ID: WEB-101) is currently 'Partially Shipped'. It contains 3 items across 2 different vendors. Should I pull the tracking numbers for the shipped portion?

---

**👤 You:**
> "List all active vendors and their status."

**🤖 AI Agent:**
> You have 8 active vendors, including 'DropShip Plus' (Connected) and 'Wholesale Direct' (Connected). 1 vendor is currently 'Disconnected'. Would you like to see the profile for the disconnected vendor?


## ❓ FAQ

**Q: How do I get Duoplane API credentials?**
Log in to your Duoplane dashboard, navigate to **Settings > API**, and you can generate or retrieve your unique API Key. For the API Password, Duoplane typically uses 'X'. You will also need your account subdomain.

**Q: Can the agent update inventory levels?**
This integration currently focuses on listing and auditing orders, POs, vendors, and products. Updating inventory levels or product details should be managed via the Duoplane portal or your e-commerce platform.

**Q: Does the integration show vendor tracking info?**
Yes, you can use the get_purchase_order_details tool to retrieve tracking numbers and fulfillment status for orders handled by your vendors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/duoplane](https://vinkius.com/mcp/duoplane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Duoplane** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `duoplane` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Duoplane** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "duoplane": {
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
