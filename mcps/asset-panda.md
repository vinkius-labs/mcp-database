# Asset Panda MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/asset-panda)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Track and manage fixed assets with Asset Panda — audit groups, objects, and locations via AI.

## Description
The **Asset Panda MCP Server** provides a flexible natural language interface to your asset tracking and management platform. Empower your AI agent to manage your entire inventory, from high-level entity groups to individual asset details and location tracking.

### Key Features

- **Group Management** — List all organizational entities (Groups) to understand how your data is structured.
- **Asset Tracking** — Retrieve detailed information for individual objects (assets), including custom field values.
- **Inventory Oversight** — List and search for assets within specific groups to maintain an accurate inventory.
- **Asset Lifecycle** — Create and update asset records directly from your chat interface to reflect real-world changes instantly.
- **Location Management** — Track where your assets are across different sites and departments.
- **Secure OAuth 2.0** — Uses secure Client Credentials flow to ensure safe access to your organization's inventory data.

### Who is this for?

- **IT Asset Managers** — Quickly audit hardware inventory and update asset assignments using natural language.
- **Operations Leads** — Track equipment locations and statuses across multiple facilities.
- **Finance Teams** — Retrieve asset data for depreciation reporting and audit compliance without manual exports.


## Available Tools (8)
- **create_object**: Create a new object (asset) in a group
- **get_account_check**: Verify Asset Panda account connection
- **get_group**: Get metadata for a specific asset group
- **get_object**: Get details for a specific object (asset)
- **list_groups**: List all asset groups (entities) in Asset Panda
- **list_locations**: List all locations (alias for list_groups)
- **list_objects**: List all objects (assets) within a specific group
- **update_object**: Update an existing object (asset)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Asset Panda** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all asset groups in my account."

**🤖 AI Agent:**
> I've retrieved your groups. You have several entities defined, including 'Assets', 'Employees', 'Locations', and 'Software Licenses'.

---

**👤 You:**
> "Show me the assets in the 'Laptops' group (ID: 12345)."

**🤖 AI Agent:**
> I've found 15 objects in the 'Laptops' group, including 'MacBook Pro #45' and 'Dell XPS #12'.

---

**👤 You:**
> "Update the status of asset 'obj_9988' in group '123' to 'In Repair'."

**🤖 AI Agent:**
> Asset 'obj_9988' has been successfully updated with the new status. The changes are now reflected in your Asset Panda account.


## ❓ FAQ

**Q: How do I find my Asset Panda Client ID and Secret?**
Log in to Asset Panda, go to **Settings (cog icon) > API Configuration**. Your Client ID and Client Secret will be displayed at the bottom of the page.

**Q: What is a 'Group ID' in Asset Panda?**
Groups (or Entities) are the categories for your records (e.g., Assets, Employees). You can find a group's ID in its URL when editing it in **Settings > Group Settings**.

**Q: How do I provide data for creating or updating assets?**
Use the `jsonData` parameter with a valid JSON string where keys are field IDs (e.g., `{"field_123": "New Value"}`). You can find field IDs by using the `get_group` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/asset-panda](https://vinkius.com/mcp/asset-panda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Asset Panda** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `asset-panda` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Asset Panda** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "asset-panda": {
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
