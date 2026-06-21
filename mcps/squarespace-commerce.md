# Squarespace Commerce MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/squarespace-commerce)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/squarespace-commerce-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/squarespace-commerce-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Bring your Squarespace Commerce backend into your AI. Manipulate inventory, track orders, and fulfill shipments programmatically.

## Description
Connect your **Squarespace Commerce** backend operations exclusively to your localized artificial intelligence companion. Sever the need to log into visual CMS dashboards repetitively just to verify if an order processed successfully or if a variant sold out. Unveil inventory metrics, customer logs, and complex catalog hierarchies natively, commanding AI responses to adjust stock instantly via natural language.

### What you can do

- **Order Logistics** — Read pending commercial shipments scanning `list_orders`, pinpoint specific buyer details using `get_order_details` and finalize dispatch procedures securely invoking `fulfill_order`
- **Inventory Scaling** — Audit remaining physical store stock actively running `list_inventory`, and inject stock resupplies or debits commanding `adjust_inventory` instantly
- **Product Catalog** — Pull deep merchandising arrays gathering everything your shop sells utilizing `list_products` and breaking down SKU variants natively requesting `get_product_details`
- **CRM & Books** — Download shopper histories calling `list_customer_profiles` while tracking absolute bank flow via pure data streams with `list_transactions`

### How it works

1. Enable the MCP bridge natively on your computing environment
2. Provide your overarching Squarespace Developer API Key securely
3. Engage your language model internally telling it to flag all unfulfilled orders older than 48 hours automatically

### Who is this for?

- **E-Commerce Operations** — automate repetitive dispatch approvals by commanding LLMs to process `fulfill_order` based on simple logic parameters over chat
- **Back-End Developers** — build specialized headless checkout flows investigating exact endpoint limits or structures blindly without consulting postman 
- **Shop Managers & Owners** — pull markdown tables highlighting "Low Stock Items" instantly right inside Cursor to orchestrate purchasing cycles quickly


## Available Tools
- **adjust_inventory**: Provide a variant_id and a quantity delta (e.g. 5 to add, -2 to subtract).

Adjusts the inventory quantity for a product variant
- **fulfill_order**: Requires order_id, tracking_number, and carrier name.

Marks an order as fulfilled and adds tracking information
- **get_order_details**: Retrieves details for a specific order
- **get_product_details**: Retrieves details for a specific product
- **list_inventory**: Lists inventory levels for product variants
- **list_orders**: Supports pagination via cursor.

Lists Squarespace Commerce orders
- **list_products**: Returns product names and IDs. Use the cursor from the previous response for pagination.

Lists Squarespace Commerce products
- **list_customer_profiles**: Lists Squarespace customer profiles
- **list_transactions**: Lists financial transactions
- **list_webhooks**: Lists configured webhook subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Squarespace Commerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan the current order list and figure out exactly which items are marked as pending fulfillment."

**🤖 AI Agent:**
> Cycling via `list_orders` returning unresolved tickets:

1. 📦 **Order #62Bf (Pending/Open)** - Customer: Alice Lee - Value: $140.00
2. 📦 **Order #12Zx (Pending/Open)** - Customer: John M. - Value: $40.50

The rest of the transactions present in this pagination phase are cleanly fulfilled. Tell me the ID string if you want to apply a Courier track to any.

---

**👤 You:**
> "Tell me the inner variant IDs attached to my product item tagged 'Winter Coat X5'. Our main store sells roughly 5 jackets."

**🤖 AI Agent:**
> Invoked iterative search through `list_products` extracting 'Winter Coat X5' locating Primary ID object ~ `12abcd56`. Next requested Deep Metadata firing `get_product_details` to return your variables.

Here are the variants bound inside your Coat Parent Wrapper:
- **Variant A**: 'Black / Large' -> Variant ID: `vxA001` (Stock: 5)
- **Variant B**: 'Grey / Medium' -> Variant ID: `vxB004` (Stock: 2)

You can explicitly demand an inventory adjustment on these ID signatures via this interface freely.

---

**👤 You:**
> "We just sold a 'Grey / Medium' offline to a friend. Adjust its variant inventory quantity ID vxB004 by -1 unit securely."

**🤖 AI Agent:**
> Initializing an update request securely wrapping bounds connecting onto backend. Target Node `adjust_inventory` applied. 

**STATUS: ADJUSTMENT FINALIZED ✅**
Associated Variant: `vxB004`
Adjustment Processed: `-1 Unit Subtract`

The Squarespace backend accepted structural changes. Your active live stock now officially reflects 1 physical good available seamlessly avoiding overselling.


## Installation & Usage

To install and use the **Squarespace Commerce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/squarespace-commerce](https://vinkius.com/mcp/squarespace-commerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
