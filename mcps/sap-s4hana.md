# SAP S/4HANA MCP Server

Manage purchase orders, business partners, inventory, and financial postings on SAP S/4HANA — the intelligent ERP.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sap-s4hana)

## Overview
**Category:** industry-titans
**Tools Count:** 9

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


## Installation & Usage

To install and use the **SAP S/4HANA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sap-s4hana](https://vinkius.com/mcp/sap-s4hana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
