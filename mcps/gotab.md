# GoTab MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gotab)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gotab-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gotab-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your restaurant operations — menus, orders, and tabs via AI.

## Description
Connect your **GoTab** POS and commerce account to your AI agent and streamline your hospitality management. Use natural language to update menu items, check the status of active tabs, and monitor real-time orders directly from your workflow.

### What you can do

- **Menu & Item Management** — List all menus, browse categories, and instantly update the availability status of specific items (e.g., mark as 'sold out')
- **Order Tracking** — Retrieve recent orders, view specific order details, and monitor kitchen operations without opening the GoTab manager dashboard
- **Tab Management** — Check active or closed tabs to help resolve customer inquiries quickly
- **Location Insights** — Manage multiple venues by querying specific location data easily

### How it works

1. Subscribe to this server
2. Enter your GoTab API Access ID and Secret
3. Start managing your restaurant operations from Claude, Cursor, or any MCP-compatible client

Your AI acts as your digital front-of-house manager, capable of instantly checking tab balances or updating item availability based on kitchen feedback.

### Who is this for?

- **Restaurant Managers** — quickly mark an item as 86'd (sold out) across all digital menus via a simple voice or text command
- **Customer Support** — look up a specific guest's tab or past order details instantly when handling disputes or inquiries
- **F&B Directors** — monitor order flow and menu availability across multiple locations from a unified chat interface


## Available Tools
- **get_item**: Get details for a specific item
- **get_location**: Get details for a specific location
- **get_menu**: Get details for a specific menu
- **get_order**: Get details for a specific order
- **get_tab**: Get details for a specific tab
- **list_categories**: List categories within a menu
- **list_items**: List catalog items for a location
- **list_locations**: List all accessible locations
- **list_menus**: List menus for a location
- **list_orders**: List recent orders for a location
- **list_tabs**: List active or closed tabs
- **update_item_status**: Update the availability status of an item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoTab** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Mark the 'Truffle Fries' (Item ID 883) at location 12 as sold out."

**🤖 AI Agent:**
> Updating item... Success! I've marked Item ID 883 ('Truffle Fries') as 'sold_out' for location 12. It will no longer be available for order on the digital menu.

---

**👤 You:**
> "Show me the details of Tab ID 93021."

**🤖 AI Agent:**
> Fetching tab details... Tab #93021 is currently 'OPEN' under the name 'Sarah P.'. The current total is $45.50. Recent items ordered include 2x 'House Margarita' and 1x 'Calamari'.

---

**👤 You:**
> "List all incoming orders that are currently queued in the kitchen for Location 1."

**🤖 AI Agent:**
> Checking active ticket flow...
There are presently 3 live orders queued in prep queues globally. Would you like me to expand ticket #A22 specifically?


## Installation & Usage

To install and use the **GoTab** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gotab](https://vinkius.com/mcp/gotab)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
