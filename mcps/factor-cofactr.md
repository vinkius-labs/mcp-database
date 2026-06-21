# Factor (Cofactr) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/factor-cofactr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/factor-cofactr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/factor-cofactr-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate supply chain operations via Factor (Cofactr) — manage parts, purchase orders, and inventory directly through your AI agent.

## Description
Connect your **Factor (now Cofactr)** supply chain account to any AI agent and take full control of your electronics procurement and logistics through natural conversation.

### What you can do

- **BOM & Part Management** — List and fetch details for parts and components in your Bill of Materials
- **Purchase Order Tracking** — List, inspect, and create purchase orders (POs) directly from the cloud
- **RFQ Management** — Manage requests for quotes (RFQs) to streamline your sourcing process
- **Inventory Visibility** — Check real-time stock levels across specialized warehouses
- **Supplier CRM** — List and manage your network of pre-vetted suppliers with ease

### How it works

1. Subscribe to this server
2. Enter your Factor/Cofactr API Key and Base URL
3. Start managing your supply chain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Procurement Managers** — monitor PO status and part availability without leaving your communication tools
- **Hardware Engineers** — check kitting status and component stock levels directly from your workflow
- **Operations Teams** — automate follow-ups and supply chain updates through natural language queries


## Available Tools
- **create_purchase_order**: Create a new purchase order
- **get_item**: Get details for a specific part or component
- **get_me**: Get current API user profile
- **get_purchase_order**: Get details for a specific purchase order
- **get_rfq**: Get details for a specific RFQ
- **get_supplier**: Get details for a specific supplier
- **list_inventory**: List current stock levels across warehouses
- **list_items**: List all parts and components in the Factor/Cofactr catalog
- **list_purchase_orders**: List all purchase orders
- **list_rfqs**: List all requests for quotes
- **list_suppliers**: List all suppliers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Factor (Cofactr)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active purchase orders on Factor."

**🤖 AI Agent:**
> I've retrieved your purchase orders. You have PO-102 (Shipped), PO-105 (Pending Approval), and PO-108 (Received) among others. Which one should I inspect further?

---

**👤 You:**
> "Check the kitting status for project ABC."

**🤖 AI Agent:**
> Searching kitting status... Project ABC is 85% complete. 42 out of 50 parts are currently in stock and ready. We are waiting on 8 capacitors from Vendor X.

---

**👤 You:**
> "List all suppliers in my network."

**🤖 AI Agent:**
> Fetching suppliers... I found 15 pre-vetted suppliers including 'Avnet', 'Digi-Key', and 'Mouser'. Would you like to see the performance rating for any of them?


## Installation & Usage

To install and use the **Factor (Cofactr)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/factor-cofactr](https://vinkius.com/mcp/factor-cofactr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
