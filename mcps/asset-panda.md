# Asset Panda MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/asset-panda)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/asset-panda-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/asset-panda-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Asset Panda** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/asset-panda](https://vinkius.com/mcp/asset-panda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
