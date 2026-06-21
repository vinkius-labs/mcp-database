# Dutchie Plus MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dutchie-plus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dutchie-plus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dutchie-plus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage enterprise dispensary locations, track online menus, and monitor orders via the Dutchie Plus API.

## Description
Integrate **Dutchie Plus**, the enterprise-grade e-commerce platform for cannabis retailers, directly into your AI workflow. Manage your multi-location dispensary operations, track online menus and product categories, monitor enterprise-wide online orders and fulfillment, and oversee synchronized brands using natural language.

### What you can do

- **Location Oversight** — List and retrieve detailed configuration and real-time status for all your dispensary locations.
- **Menu Intelligence** — Access and monitor online menus, categories, and preview URLs for every location in your enterprise.
- **Order Management** — Track online orders, payment statuses, and fulfillment history for specific locations or across the entire organization.
- **Brand Synchronization** — List and retrieve all product brands synchronized in your enterprise account, including associated product counts.

### How it works

1. Connect the Dutchie Plus integration to your AI assistant.
2. Authorize using your Dutchie Plus API Key (found in your enterprise settings).
3. Orchestrate your enterprise dispensary management and online retail operations through intuitive conversation.

### Who is this for?

- **Enterprise Managers** — Quickly check order volumes and location activity across the entire fleet on the go.
- **Digital Operations** — Monitor online menu availability and category mapping via chat.
- **Inventory & Brand Leads** — Audit synchronized brands and location-specific orders instantly.


## Available Tools
- **get_dutchie_plus_metadata**: Retrieve metadata and limits for your Dutchie Plus account
- **get_location_details**: Get detailed settings and information for a specific dispensary location
- **get_order_details**: Get detailed information for a specific online order
- **quick_enterprise_volume_audit**: Retrieve a high-level summary of order activity across multiple locations (mock logic)
- **list_pending_fulfillment_orders**: Identify online orders that are currently awaiting fulfillment or ready for pickup
- **list_synced_brands**: List all product brands synchronized in your enterprise account
- **list_dispensary_locations**: List all dispensary locations managed in your Dutchie Plus account
- **list_online_menus**: List all online menus configured for a specific location
- **list_enterprise_orders**: List all recent online orders for a specific dispensary location
- **search_dispensaries_by_city**: Search for dispensary locations using a city or name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dutchie Plus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our dispensary locations."

**🤖 AI Agent:**
> I've found 8 locations in your network, including 'Downtown Dispensary' (San Francisco) and 'Airport Plaza' (Los Angeles). Would you like to see the current online menu URL for Downtown?

---

**👤 You:**
> "Show me the pending online orders for location 'LOC-12345'."

**🤖 AI Agent:**
> For 'Downtown Dispensary' (LOC-12345), there are 5 pending online orders, including 'WEB-99' (Ready for Pickup) and 'WEB-101' (Awaiting Fulfillment). Should I pull the items list for WEB-99?

---

**👤 You:**
> "List all synchronized brands in our account."

**🤖 AI Agent:**
> I've retrieved 12 synchronized brands, including 'Nature's Own', 'Indica Gold', and 'Pure CBD'. 'Nature's Own' has 45 associated products in your catalog. Would you like to see the brand details for Indica Gold?


## Installation & Usage

To install and use the **Dutchie Plus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dutchie-plus](https://vinkius.com/mcp/dutchie-plus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
