# SAP S/4HANA MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sap-s4hana)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sap-s4hana-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sap-s4hana-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage purchase orders, business partners, inventory, and financial postings on SAP S/4HANA — the intelligent ERP.

## Description
Connect your **SAP S/4HANA** system to any AI agent and manage core ERP operations through natural conversation.

### What you can do

- **Business Partners** — Create, read, and update business partner master data including customers, suppliers, and contacts
- **Purchase Orders** — Create purchase orders, check approval status, and query PO history with full line-item detail
- **Sales Orders** — Retrieve sales order data, delivery status, and billing documents across your sales organization
- **Inventory Management** — Query material master data, stock levels by plant/storage location, and goods receipt history
- **Financial Postings** — Post journal entries, retrieve G/L account balances, and query cost center reports
- **Production Planning** — Check production order status, planned orders, and material requirements planning (MRP) results
- **Custom OData Queries** — Execute any exposed OData v4 service on your S/4HANA system for tailored data access

### How it works

1. Subscribe to this server
2. Enter your SAP S/4HANA Communication User credentials and instance URL
3. Start managing ERP operations through Claude, Cursor, or any MCP-compatible client

77% of global commercial transactions touch an SAP system. Now your AI agent speaks SAP.

### Who is this for?

- **Procurement Teams** — create purchase orders and manage supplier data through simple chat commands
- **Finance Teams** — post journal entries and query G/L balances without navigating SAP GUI transactions
- **Supply Chain Managers** — check inventory levels and production order status through conversation
- **SAP Consultants** — accelerate data retrieval and configuration audits across client landscapes


## Available Tools
- **list_business_partners**: Use OData $filter syntax for filtering — e.g. BusinessPartnerCategory eq '2' for organizations.

List SAP business partners
- **get_business_partner**: Get a specific business partner by ID
- **create_business_partner**: Provide JSON with BusinessPartnerCategory (1=Person, 2=Organization), FirstName/LastName or OrganizationBPName1.

Create a new business partner
- **list_purchase_orders**: Filter by supplier, purchasing org, or status using OData $filter syntax.

List purchase orders
- **create_purchase_order**: Provide JSON with CompanyCode, PurchaseOrderType, Supplier, PurchasingOrganization, PurchasingGroup, and line items in _PurchaseOrderItem array.

Create a purchase order
- **list_sales_orders**: Filter using OData syntax.

List sales orders
- **get_material_stock**: Returns available quantities across storage locations.

Get material stock levels
- **get_gl_balances**: Get G/L account balances
- **query_odata**: Provide the service path and entity set. Supports $filter, $select, $expand.

Execute a custom OData v4 query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAP S/4HANA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all pending purchase orders for plant 1000 above €50,000."

**🤖 AI Agent:**
> Found 7 pending POs for Plant 1000 above €50K: 1. PO 4500012345 — 'Raw Materials Q2' (€125,000, Supplier: ACME GmbH), 2. PO 4500012350 — 'Server Equipment' (€89,500, Supplier: TechCorp), and 5 more. Total pending value: €487,230. Would you like to approve or view details?

---

**👤 You:**
> "What's the current stock level for material MAT-2024-A across all plants?"

**🤖 AI Agent:**
> Material MAT-2024-A stock levels: Plant 1000 (Berlin) — 2,450 units, Plant 2000 (Shanghai) — 1,800 units, Plant 3000 (São Paulo) — 920 units. Total available: 5,170 units. Safety stock threshold is 1,000/plant — São Paulo is below threshold. Want me to create a purchase requisition?

---

**👤 You:**
> "Create a business partner record for 'NovaTech Solutions' as a supplier."

**🤖 AI Agent:**
> Business Partner BP-0010045678 ('NovaTech Solutions') created successfully as a Supplier. Category: Organization, Role: Vendor. Would you like me to add bank details, purchasing organization assignments, or a contact person?


## Installation & Usage

To install and use the **SAP S/4HANA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sap-s4hana](https://vinkius.com/mcp/sap-s4hana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
