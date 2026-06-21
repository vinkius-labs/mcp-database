# Bsale MCP Server

Automate cloud POS operations via Bsale — issue electronic invoices, manage inventory, track stock levels, and register clients from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bsale)

## Overview
**Category:** money-moves
**Tools Count:** 15

## Description
Connect your **Bsale** cloud POS account to any AI agent and take full control of your Chilean retail and invoicing operations through natural conversation.

### What you can do

- **Electronic Document Emission** — Issue SII-compliant boletas, facturas electrónicas, credit notes, and dispatch guides directly through your AI agent
- **Product Catalog Management** — Browse, search, and create products with full variant (SKU) support, pricing tiers, and web descriptions
- **Inventory & Stock Control** — Check real-time stock levels across all office branches and track variant-level availability
- **Client Registry** — Search, inspect, and register customers with RUT, business activity (giro), and contact details for tax compliance
- **Configuration Intelligence** — Query your document types, payment methods, price lists, and office configurations instantly

### How it works

1. Subscribe to this server
2. Enter your Bsale Access Token
3. Start managing your POS from Claude, Cursor, or any MCP-compatible client

Your AI becomes a dedicated retail operations assistant — no more navigating multiple POS screens to issue a simple boleta.

### Who is this for?

- **Retail Store Managers** — issue invoices and check stock without switching between terminals and browsers
- **Accountants** — query document registries and client information for month-end reconciliation
- **E-commerce Operators** — sync product catalogs and manage variant pricing across sales channels


## Available Tools
- **create_client**: The client can then be associated with future invoices and sales documents. For Chilean tax compliance, include the RUT and business activity (giro) when available.

Register a new client in the system
- **create_document**: Requires the document type ID and at minimum one line item with product details. The document is automatically sent to the Chilean SII (Servicio de Impuestos Internos) for validation.

Issue a new electronic tax document
- **create_product**: The product will be available for inclusion in future documents and can be associated with variants (SKUs), price lists, and stock management across multiple offices.

Create a new product in the catalog
- **get_client**: Get full details of a specific client
- **get_document**: Get full details of a specific tax document
- **get_product**: Get full details of a specific product
- **list_clients**: Use limit and offset for pagination.

List all registered clients
- **list_document_types**: List available SII document types
- **list_documents**: Documents are returned with their SII-compliant folio numbers, emission dates, and net/tax/total breakdowns. Use optional limit and offset parameters for pagination.

List tax documents (invoices, boletas, credit notes)
- **list_offices**: List all office branches and locations
- **list_payment_types**: List accepted payment methods
- **list_price_lists**: g., retail, wholesale, distributor). Each price list can have different pricing for the same product variants.

List all configured price lists
- **list_products**: Use limit and offset for paginated browsing of large catalogs.

List all products and services in your catalog
- **list_stocks**: Returns available quantities per location.

Check stock levels across offices
- **list_variants**: Each variant has its own barcode, cost, and pricing configuration across different price lists.

List all SKU variants for a product


## Installation & Usage

To install and use the **Bsale** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bsale](https://vinkius.com/mcp/bsale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
