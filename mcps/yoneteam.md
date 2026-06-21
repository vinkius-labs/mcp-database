# YoneTeam MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yoneteam)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yoneteam-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yoneteam-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your Turkish business operations with project tracking, task management, and team collaboration designed for local teams.

## Description
Connect your **YoneTeam (Satin Alma)** account to any AI agent and streamline your entire procurement and supply chain process through natural conversation.

### What you can do

- **Demand Management** — List and create internal purchasing demands to initiate the procurement cycle.
- **Offer Comparison** — Query and inspect supplier offers and quotes to make informed buying decisions.
- **Order Tracking** — Manage the lifecycle of purchase orders from issuance to final delivery.
- **Supplier Directory** — List approved suppliers and browse your materials catalog to identify sourcing options.
- **Delivery Logistics** — Monitor scheduled deliveries and incoming shipments to keep your operations running smoothly.

### How it works

1. Subscribe to this server
2. Enter your YoneTeam API Key
3. Start managing your procurement from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Procurement Officers** — quickly check the status of pending demands and compare supplier quotes via AI.
- **Supply Chain Managers** — monitor delivery schedules and verify material availability in real-time.
- **Operations Leads** — automate the creation of purchasing requests and track order progress without leaving the workspace.


## Available Tools
- **create_demand**: Create a new purchasing demand
- **get_me**: Get account information
- **get_offer_details**: Get details of a specific offer
- **get_order_details**: Get details of a specific purchase order
- **list_deliveries**: List scheduled deliveries
- **list_demands**: List purchasing demands
- **list_materials_catalog**: List material catalog
- **list_offers**: List supplier offers
- **list_purchase_orders**: List purchase orders
- **list_suppliers**: List approved suppliers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **YoneTeam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all pending purchasing demands from the IT department."

**🤖 AI Agent:**
> I've retrieved the demands. There are 2 pending requests from IT: 'Laptops for New Hires' and 'Server Maintenance Spares'. Would you like to check for supplier offers on these?

---

**👤 You:**
> "Compare the current offers for purchase demand #1029."

**🤖 AI Agent:**
> I've analyzed the offers for Demand #1029. You have 3 quotes: 'Global Systems' ($1,200), 'Office Plus' ($1,150), and 'Tech Source' ($1,300). 'Office Plus' is currently the most cost-effective option.

---

**👤 You:**
> "Create a new demand for '10x Ergonomic Chairs' for the Sales team."

**🤖 AI Agent:**
> Success! A new purchasing demand for '10x Ergonomic Chairs' (Sales Dept) has been created with ID DEM-8823. I'll monitor for incoming supplier offers.


## Installation & Usage

To install and use the **YoneTeam** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yoneteam](https://vinkius.com/mcp/yoneteam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
