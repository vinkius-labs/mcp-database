# Grocy (Home ERP) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grocy-home-erp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/grocy-home-erp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/grocy-home-erp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate your household management with Grocy — track inventory, manage shopping lists, and organize chores directly from your AI agent.

## Description
Connect your **Grocy** instance to any AI agent and take full control of your home ERP through natural conversation. Grocy is the self-hosted solution for managing your household.

### What you can do

- **Stock Management** — List all products in stock, add new items, consume supplies, and perform inventory checks to keep your pantry updated.
- **Shopping Lists** — Manage your grocery needs by adding items to your list, clearing purchased items, or viewing what's missing.
- **Recipes & Meal Planning** — Browse your recipe collection and automatically consume ingredients from your stock when you cook.
- **Chore Tracking** — Keep track of household maintenance by listing pending chores and marking them as executed.
- **Battery & Task Management** — Monitor battery charge cycles and manage general household tasks and reminders.

### How it works

1. Subscribe to this server
2. Enter your Grocy API Key and Base URL
3. Start managing your home from Claude, Cursor, or any MCP-compatible client

No more manual entry on a small screen. Your AI acts as your personal home manager, helping you stay organized and efficient.

### Who is this for?

- **Home Organizers** — instantly check if you have enough ingredients for dinner without opening the pantry.
- **Busy Families** — coordinate chores and shopping lists through simple voice or text commands.
- **Self-Hosters** — leverage your existing Grocy data within your favorite AI tools and IDEs.


## Available Tools
- **add_product_stock**: Add a specific amount of a product to stock
- **add_shopping_list_item**: Add an item to the shopping list
- **charge_battery**: Mark a battery as charged
- **clear_shopping_list**: Remove all items from the shopping list
- **consume_product_stock**: Consume a specific amount of a product from stock
- **consume_recipe**: Consume all ingredients for a specific recipe from stock
- **create_task**: Create a new task
- **delete_task**: Delete a task
- **execute_chore**: Mark a chore as executed
- **get_batteries**: Get a list of all batteries
- **get_chores**: Get a list of all chores
- **get_product**: Get details for a specific product
- **get_recipe**: Get details for a specific recipe
- **get_recipes**: Get a list of all recipes
- **get_shopping_list**: Get all items on the shopping list
- **get_stock**: Get all products currently in stock
- **get_tasks**: Get a list of all tasks
- **inventory_product_stock**: Set the stock amount of a product to a specific value
- **remove_purchased_shopping_list**: Remove all items marked as purchased from the shopping list
- **transfer_product_stock**: Transfer a product between locations
- **update_task**: Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grocy (Home ERP)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What products do I currently have in stock?"

**🤖 AI Agent:**
> I've checked your Grocy inventory. You currently have 12 items in stock, including Milk (2L), Eggs (12 units), and Flour (1kg). Would you like the full list?

---

**👤 You:**
> "Add 2 units of Coffee to my shopping list."

**🤖 AI Agent:**
> Success! I've added 2 units of Coffee (Product ID: 5) to your shopping list. Is there anything else you need to buy?

---

**👤 You:**
> "Show me my pending chores and mark 'Vacuuming' as done."

**🤖 AI Agent:**
> You have 3 pending chores: Vacuuming, Watering Plants, and Dusting. I have successfully executed 'Vacuuming' (ID: 2) for you.


## Installation & Usage

To install and use the **Grocy (Home ERP)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grocy-home-erp](https://vinkius.com/mcp/grocy-home-erp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
