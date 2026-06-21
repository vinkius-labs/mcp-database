# Odoo Purchase MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-purchase)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/odoo-purchase-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/odoo-purchase-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Create purchase orders, manage RFQs, search vendors, and track procurement — Odoo Purchasing through natural conversation.

## Description
Connect **Odoo ERP** to any AI agent — manage your entire business without switching tabs.

### What you can do
- **CRM** — Search and create leads, track opportunities through your pipeline
- **Contacts** — Find individual contacts and companies, create new partners
- **Sales** — List and manage sales orders with full order details
- **Notes** — Add comments and notes to any record in your Odoo instance

### Who is this for?
- **Sales Teams** — CRM pipeline at your fingertips through AI
- **Account Managers** — Quick access to contact and company information
- **Operations** — Monitor sales orders without switching screens
- **Odoo Administrators** — Query any module through natural conversation


## Available Tools
- **odoo_confirm_purchase_order**: order, transitioning from "draft" to "purchase" state. This locks the order, notifies the vendor, and creates an incoming receipt (stock.picking) for warehouse processing. Use when the user approves a vendor quote or wants to place the order.

Confirm a draft RFQ, converting it into a confirmed purchase order and triggering receipt creation
- **odoo_create_purchase_order**: order in "draft" state (an RFQ). The partnerId must be an existing vendor (res.partner with supplier_rank > 0) — use odoo_search_vendors to find vendor IDs. Lines must be a JSON array: [{"product_id": <id>, "product_qty": <qty>, "price_unit": <cost>}]. Each line also gets an auto-generated description.

Create a new purchase order (as a draft RFQ) for a vendor with product lines, quantities, and prices
- **odoo_get_po_lines**: order.line records for the given PO. Returns each line with product name, ordered quantity, unit cost, subtotal, and planned delivery date. Use to inspect what is being purchased, verify pricing, or check delivery schedules per line item.

Get the individual line items of a purchase order showing products, quantities, costs, and expected delivery dates
- **odoo_get_purchase_order**: order with all key fields. Use after listing POs to drill into a specific order for vendor details, amounts, and expected receipt dates.

Get the complete details of a specific purchase order by its numeric ID
- **odoo_list_purchase_orders**: order records ordered by creation date. Returns PO number, vendor name, state (draft/sent/purchase/done/cancel), total and untaxed amounts, responsible buyer, expected receipt date, and order date. Filter by state to see only draft RFQs, confirmed POs, or completed orders. Use when the user asks about procurement activity, pending orders, or vendor purchases.

List purchase orders in Odoo with vendor, amounts, buyer, and current processing status
- **odoo_list_rfqs**: order records in "draft" state only. These are RFQs that need vendor pricing, negotiation, or approval before being confirmed. Use when the user asks specifically about pending RFQs, quotes from vendors, or procurement requests awaiting approval.

List all Requests for Quotation (draft purchase orders) that have not yet been confirmed to vendors
- **odoo_search_vendors**: partner records where supplier_rank > 0 — these are partners flagged as vendors/suppliers. Returns vendor name, email, phone, city, and country. Use to find vendor IDs before creating purchase orders, or when the user asks about supplier information.

Search for vendors and suppliers in Odoo by name, returning contact details and location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Odoo Purchase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from the website"

**🤖 AI Agent:**
> 👥 **CRM Leads — Website**
| Name | Email | Stage | Revenue |
|---|---|---|---|
| Acme Corp | info@acme.com | Qualification | $15,000 |
| Beta Inc | hello@beta.io | Proposition | $8,500 |

---

**👤 You:**
> "Show recent sales orders"

**🤖 AI Agent:**
> 📋 **Sales Orders**
| SO# | Customer | Amount | Status |
|---|---|---|---|
| S00042 | Acme Corp | $12,500 | Confirmed |
| S00041 | Beta Inc | $3,200 | Draft |


## Installation & Usage

To install and use the **Odoo Purchase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-purchase](https://vinkius.com/mcp/odoo-purchase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
