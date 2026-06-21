# EZO Asset Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ezo-asset-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Equip your AI agent to manage fixed assets, track inventory, and monitor checkouts via the EZO.io (EZOfficeInventory) API.

## Description
Integrate **EZO.io** (formerly EZOfficeInventory), the world's most popular asset management platform, directly into your AI workflow. Manage your fixed asset database and physical locations, track consumable inventory and real-time stock levels, monitor active checkouts and reservations, and oversee your entire asset lifecycle using natural language.

### What you can do

- **Asset Oversight** — List and retrieve detailed information, identifiers, and maintenance history for all your managed assets.
- **Inventory Intelligence** — Monitor consumable inventory items, resolving available quantities and stock thresholds across your organization.
- **Checkout Management** — Access and monitor currently checked out assets, identifying assigned members and expected return dates.
- **Asset Auditing** — Retrieve high-level summaries of asset volume, location distribution, and organizational resource health instantly.

### How it works

1. Connect the EZO integration to your AI assistant.
2. Authorize using your EZO Subdomain and REST API Key (found in your account settings).
3. Orchestrate your asset intelligence and resource management through intuitive conversation.

### Who is this for?

- **IT & Facility Managers** — Quickly check asset statuses and physical locations on the go.
- **Operations Teams** — Research inventory levels and active checkouts via chat during workflows.
- **Finance & Admin Teams** — Monitor asset volumes and organizational resource metadata instantly.


## Available Tools (10)
- **get_ezo_account_metadata**: Retrieve metadata and limits for your EZO account
- **get_asset_detailed_data**: Get detailed settings and information for a specific asset
- **quick_asset_volume_audit**: Retrieve a high-level summary of assets, inventory, and members
- **list_currently_checked_out_assets**: Identify all assets that are currently checked out to members
- **list_managed_assets**: g. available, checked out) from the EZO API.

List all fixed assets managed in your EZO account
- **list_available_assets**: Identify assets that are currently available for checkout
- **list_consumable_inventory**: List all consumable inventory items and their stock levels
- **list_asset_locations**: List all physical locations and sub-locations configured in your account
- **list_account_members**: List all members and users registered in your organization
- **list_overdue_checkouts**: Identify assets that are past their expected return date (mock logic)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EZO Asset Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all assets currently checked out."

**🤖 AI Agent:**
> I've found 12 assets currently checked out, including 'MacBook Pro - IT-001' (assigned to John Miller) and 'Projector - CONF-A' (assigned to Alice Connor). Would you like to see the due dates for these items?

---

**👤 You:**
> "Show me our inventory levels for 'Ethernet Cables'."

**🤖 AI Agent:**
> For 'Ethernet Cables' (Cat6), you currently have 85 units in stock across all locations. Your low stock threshold is set to 20 units. Should I pull the list of other consumable items near their limit?

---

**👤 You:**
> "Check for overdue asset returns."

**🤖 AI Agent:**
> There are 3 overdue assets: 'Test Kit #5' (due March 10th), 'DSLR Camera' (due March 12th), and 'Tablet - OPS-02'. Would you like the contact information for the members who have these assets?


## ❓ FAQ

**Q: How do I get an EZO API Key?**
Log in to your EZO.io account, navigate to **Settings > API Integration**, and you can enable the API and retrieve your unique **Secret API Key**. You also need your **Subdomain** (the prefix in your account URL).

**Q: Does the integration support multiple locations?**
Yes, you can use the list_asset_locations tool to see all physical sites and sub-locations configured in your EZO account, and filter assets by location.

**Q: Can the agent perform asset checkouts?**
This integration currently focuses on listing and auditing assets, inventory, and members. Performing live checkouts or scanning barcodes should be managed via the EZO.io mobile app or web interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ezo-asset-intelligence](https://vinkius.com/mcp/ezo-asset-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EZO Asset Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ezo-asset-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EZO Asset Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ezo-asset-intelligence": {
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
