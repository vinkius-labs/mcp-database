# Holded MCP Server

Automate business management via Holded — manage invoices, contacts, and projects directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/holded)

## Overview
**Category:** erp-operations
**Tools Count:** 11

## Description
Connect your **Holded** ERP platform to any AI agent and take full control of your invoicing, CRM, and project management through natural conversation.

### What you can do

- **Invoicing Oversight** — List all documents, retrieve detailed invoice data, and monitor payment statuses efficiently.
- **CRM & Contact Management** — Access lists of clients, suppliers, and leads, and retrieve full profile information for better relationship management.
- **Project & Task Tracking** — List active projects and monitor tasks across your entire portfolio to ensure deadlines are met.
- **Inventory & Products** — Access your product catalog and update stock levels directly from the chat interface.
- **Business Intelligence** — Retrieve account and organization metadata to maintain a high-level overview of your business operations.
- **Unified ERP** — Bridge the gap between your accounting and operations using the comprehensive Holded API.

### How it works

1. Subscribe to this server
2. Enter your Holded API Key (found in Settings > Developers)
3. Start managing your business from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex ERP modules for simple data lookups. Your AI assistant acts as a dedicated Business Operations Manager or Project Coordinator.

### Who is this for?

- **Business Owners** — instantly retrieve invoice statuses and company performance data.
- **Project Managers** — automate the oversight of tasks and project lifecycles across multiple teams.
- **Operations Leads** — maintain a real-time overview of inventory levels and customer contact data.


## Available Tools
- **get_contact_details**: Get detailed profile information for a specific contact
- **get_invoice_details**: Get detailed information about a specific invoice
- **get_api_profile**: Retrieve information about the authenticated account
- **get_product_details**: Get detailed information for a specific product
- **get_project_details**: Get detailed configuration and status for a project
- **list_contacts**: Useful for finding the contact ID required for documents.

List all contacts (clients, suppliers, leads) in Holded
- **list_invoices**: Use this to monitor billing and find IDs for specific document actions.

List all invoices in your Holded account
- **list_products**: List all products and services in your Holded inventory
- **list_projects**: List all active and past projects
- **list_all_tasks**: List tasks across all projects
- **update_product_stock**: Pass details as a JSON string in "body_json" (requires warehouseId and new quantity).

Update the stock level for a specific product


## Installation & Usage

To install and use the **Holded** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/holded](https://vinkius.com/mcp/holded)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
