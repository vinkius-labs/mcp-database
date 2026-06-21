# Envi Healthcare Supply Chain MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/envi-healthcare-supply-chain)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/envi-healthcare-supply-chain-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/envi-healthcare-supply-chain-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Equip your AI agent to manage healthcare purchase orders, track medical inventory, and monitor vendors via the Envi API.

## Description
Integrate **Envi**, the leading supply chain and inventory management platform for healthcare, directly into your AI workflow. Manage your healthcare purchase orders across facilities, track real-time medical supply inventory and stock levels, monitor authorized vendors and suppliers, and oversee your clinical procurement using natural language.

### What you can do

- **PO Oversight** — List and retrieve detailed information, line items, and approval status for all your healthcare purchase orders.
- **Inventory Intelligence** — Monitor real-time medical supply stock across facilities and departments, resolving clinical SKUs and quantities.
- **Vendor Management** — Access and monitor authorized medical vendors and suppliers, identifying contract details and sourcing origins.
- **Supply Auditing** — Retrieve high-level summaries of PO volume, critical stock alerts, and organizational facility health instantly.

### How it works

1. Connect the Envi integration to your AI assistant.
2. Authorize using your Envi REST API Key (found in your organization settings).
3. Orchestrate your healthcare procurement and supply chain strategy through intuitive conversation.

### Who is this for?

- **Healthcare Supply Chain Managers** — Quickly check PO statuses and supply availability on the go.
- **Clinical Operations Teams** — Research critical stock alerts and department inventory via chat.
- **Procurement Specialists** — Monitor vendor performance and organizational supply metadata instantly.


## Available Tools
- **get_envi_account_metadata**: Retrieve metadata and limits for your Envi account
- **get_supply_stock_level**: Get real-time stock levels for a specific medical item
- **get_po_technical_details**: Get detailed settings and line items for a specific purchase order
- **quick_healthcare_supply_audit**: Retrieve a high-level summary of POs, inventory, and requisitions
- **list_healthcare_facilities**: List all facilities and clinics configured in your organization
- **list_medical_inventory_levels**: List inventory levels across all facilities and locations
- **list_critical_stock_alerts**: Identify medical supplies that are currently below safety thresholds (mock logic)
- **list_healthcare_pos**: List all purchase orders in your Envi account
- **list_latest_supply_requisitions**: Identify the most recently created or updated supply requisitions
- **list_medical_vendors**: List all authorized vendors and suppliers in your network


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Envi Healthcare Supply Chain** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending healthcare purchase orders."

**🤖 AI Agent:**
> I've found 8 pending purchase orders, including 'PO-2024-001' ($4,500 for Surgical Supplies) and 'PO-2024-005' ($1,200 for Lab Reagents). 5 are awaiting manager approval. Would you like the details for PO-2024-001?

---

**👤 You:**
> "What is the stock level for 'Sterile Gauze' at Main Hospital?"

**🤖 AI Agent:**
> At Main Hospital, 'Sterile Gauze' (SKU: GZ-100) has 250 boxes in stock. 50 boxes are currently allocated to the ER. Should I check for low stock on other wound care items?

---

**👤 You:**
> "Show me our authorized medical vendors."

**🤖 AI Agent:**
> I've retrieved 12 authorized vendors, including 'Medline Industries', 'Cardinal Health', and 'Owens & Minor'. All have active contracts. Would you like to see the contact details for Medline?


## Installation & Usage

To install and use the **Envi Healthcare Supply Chain** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/envi-healthcare-supply-chain](https://vinkius.com/mcp/envi-healthcare-supply-chain)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
