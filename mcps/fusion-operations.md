# Fusion Operations MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fusion-operations)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fusion-operations-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fusion-operations-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Optimize factory floor operations with real-time production tracking, worker scheduling, and quality control automation.

## Description
Connect your **Autodesk Fusion Operations** (formerly Prodsmart) account to any AI agent and take full control of your manufacturing execution and shop floor workflows through natural conversation.

### What you can do

- **Production Orchestration** — List and manage all manufacturing orders and retrieve detailed status and technical metadata programmatically
- **Shop Floor Visibility** — Monitor workers, production records, and machine operations in real-time to maintain a high-fidelity oversight of your factory
- **Inventory & Logistics** — Oversight stock levels across different storage locations and warehouses to ensure precise material management
- **Product Catalog** — Access complete metadata and technical details for all items in your manufacturing database directly through your agent
- **Operational Monitoring** — Check site/company information and retrieve historical production logs for instant reporting and process analysis

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Secret** from Fusion Operations (Profile > Request an API key)
3. Start managing your factory operations from Claude, Cursor, or any MCP client

No more manual status checking or digging through manufacturing tables. Your AI acts as your dedicated production and operations coordinator.

### Who is this for?

- **Production Managers** — instantly retrieve order statuses and monitor site-wide output using natural language commands
- **Operations Leads** — track real-time inventory levels and machine performance without leaving your workspace
- **Manufacturing Engineers** — automate the extraction of production records and technical specifications for analysis


## Available Tools
- **create_production_order**: Requires product and quantity.

Create a new production order
- **get_product_details**: Get details for a specific product
- **get_production_order_details**: Get details for a specific production order
- **get_manufacturing_site_info**: Get current site/company details
- **list_inventory_stocks**: List current inventory levels
- **list_floor_machines**: List production machines
- **list_manufacturing_operations**: List manufacturing operations
- **list_production_orders**: List all production orders
- **list_manufacturing_products**: List all products/items
- **list_production_records**: List history of production records
- **list_storage_locations**: List storage locations
- **list_floor_workers**: List shop floor workers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fusion Operations** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active production orders in Fusion Operations."

**🤖 AI Agent:**
> I've retrieved your active production orders. You have 3 jobs in progress, including 'PO-1001' (Gear Shafts) and 'PO-1002' (Pump Units). Which one would you like to check for completion status?

---

**👤 You:**
> "What is the current stock level for 'Gasket Kit'?"

**🤖 AI Agent:**
> Checking inventory... For 'Gasket Kit' (ID: prod_789), you currently have 150 units in the 'Main Warehouse' and 50 units in the 'Assembly Area'. Total availability is 200 units.

---

**👤 You:**
> "Show me the production records from today."

**🤖 AI Agent:**
> Scanning production logs... Today, 5 records have been completed so far. Total output includes 500 Gear Shafts and 25 Pump Units. All operations are running within the scheduled timeframe.


## Installation & Usage

To install and use the **Fusion Operations** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fusion-operations](https://vinkius.com/mcp/fusion-operations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
