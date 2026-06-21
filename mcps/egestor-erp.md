# eGestor ERP MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/egestor-erp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/egestor-erp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/egestor-erp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your Brazilian small business with financial controls, inventory tracking, and fiscal compliance built for local regulations.

## Description
Connect your **eGestor** ERP account to any AI agent and manage your Brazilian small business operations through natural conversation.

### What you can do

- **Contact Management** — List all clients and suppliers, and retrieve individual contact profiles with full commercial data
- **Product Catalog** — Browse your product inventory with prices, stock quantities, and categories
- **Service Catalog** — Manage service offerings with pricing and descriptions
- **Sales Records** — List all sales orders and inspect individual transactions with line items, totals, and payment status
- **Purchase Records** — Track purchase orders from suppliers with costs, quantities, and receiving status

### How it works

1. Subscribe to this server
2. Enter your eGestor Personal Token from Configurações > API
3. Start managing your business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — query sales reports, check product stock, and review purchase history without opening the dashboard
- **Accountants** — pull sales and purchase records for reconciliation and fiscal reporting
- **Operations Managers** — monitor inventory levels and supplier orders through conversational AI


## Available Tools
- **get_contact**: Get a specific contact
- **get_product**: Get a specific product
- **get_purchase**: Get a specific purchase
- **get_sale**: Get a specific sale
- **get_service**: Get a specific service
- **list_contacts**: List all eGestor contacts
- **list_products**: List all products
- **list_purchases**: List all purchases
- **list_sales**: List all sales
- **list_services**: List all services


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eGestor ERP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all products with low stock (less than 10 units)."

**🤖 AI Agent:**
> Retrieved 47 products from your catalog. 6 have stock below 10 units: 1) 'Camiseta Polo M' (SKU: CP-M, stock: 3, sale price: R$ 89,90). 2) 'Caneta Esferográfica' (SKU: CE-01, stock: 7, R$ 2,50). 3) 'Mouse Wireless' (SKU: MW-100, stock: 2, R$ 45,00). 4) 'Caderno A4' (SKU: CA4-01, stock: 5, R$ 18,90). 5) 'Fone Bluetooth' (SKU: FB-200, stock: 1, R$ 129,00). 6) 'Carregador USB-C' (SKU: CU-50, stock: 8, R$ 39,90). Would you like to create a purchase order for restocking?

---

**👤 You:**
> "List all sales from this month and show me the total revenue."

**🤖 AI Agent:**
> This month you have 34 sales orders. Total revenue: R$ 12,456.80. Top 5 by value: 1) Sale #2891 — R$ 2,340.00 (client: Tech Solutions Ltda, 12 items). 2) Sale #2878 — R$ 1,890.50 (client: Maria Comercial). 3) Sale #2902 — R$ 1,250.00 (client: João Pereira ME). Payment methods: PIX (45%), boleto (30%), credit card (25%). Would you like details on any specific sale?

---

**👤 You:**
> "Show all clients who have purchased this quarter and their total spend."

**🤖 AI Agent:**
> Found 28 active clients this quarter. Top 5 by total spend: 1) 'Tech Solutions Ltda' (contact_201) — R$ 8,450.00 across 6 orders. 2) 'Maria Comercial' (contact_145) — R$ 5,120.50 across 4 orders. 3) 'João Pereira ME' (contact_089) — R$ 3,890.00 across 3 orders. 4) 'Distribuidora Norte' (contact_312) — R$ 2,780.00 across 2 orders. 5) 'Carlos Eletrônicos' (contact_178) — R$ 1,950.00 across 5 orders. Total quarterly revenue from these clients: R$ 34,290.50. Would you like to check purchase orders from suppliers?


## Installation & Usage

To install and use the **eGestor ERP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/egestor-erp](https://vinkius.com/mcp/egestor-erp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
