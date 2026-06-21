# Loyverse MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loyverse)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/loyverse-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/loyverse-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Free POS and inventory management system.

## Description
The Loyverse MCP Server allows you to seamlessly integrate your point-of-sale system with any AI agent. Manage your inventory, track sales data, and create customer profiles programmatically through natural language.

### What you can do

- **Track Sales** — Retrieve aggregated sales metrics, receipts, and performance data dynamically
- **Inventory Management** — Check stock levels and list items across multiple locations
- **Customer Data** — Search and list your registered customers in the system
- **Locations** — Retrieve store location details and coordinate operations across branches

### How it works

1. Subscribe to this server
2. Open your Loyverse Back Office and generate an Access Token
3. Start managing your store operations from any MCP-compatible client or AI agent

### Who is this for?

- **Store Managers** — quickly check inventory levels without opening the dashboard
- **Retail Owners** — pull daily sales numbers via chat
- **Customer Service** — look up customer history automatically


## Available Tools
- **l_list_customers**: List your registered store customers from Loyverse POS
- **l_list_items**: List inventory items in your Loyverse account with optional pagination parameters
- **l_list_locations**: List all store locations in your Loyverse account
- **l_list_receipts**: Can filter by creation date min and max parameters.

List generated receipts from your Loyverse POS system. Can be filtered by date range and pagination limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loyverse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the total sales numbers for all locations yesterday."

**🤖 AI Agent:**
> Retrieved yesterday's sales figures: A total of $4,532.10 across 3 stores with 120 individual receipts.

---

**👤 You:**
> "Check the current inventory level for the item 'Honduras Dark Roast Coffee' at the Main Street location."

**🤖 AI Agent:**
> The item 'Honduras Dark Roast Coffee' has 45 units in stock at the Main Street location. The low stock alert threshold is 10 units.

---

**👤 You:**
> "Create a new customer profile for John Doe with the email john@example.com."

**🤖 AI Agent:**
> Customer profile for 'John Doe' (john@example.com) has been successfully created and linked to your customer database.


## Installation & Usage

To install and use the **Loyverse** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loyverse](https://vinkius.com/mcp/loyverse)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
