# FatSecret Platform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fatsecret-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fatsecret-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fatsecret-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage your nutritional research — audit food records and recipes via AI.

## Description
Empower your AI agent to orchestrate your entire nutritional research workflow with **FatSecret Platform**, the leading API for food and nutrition data. By connecting FatSecret to your agent, you transform complex nutrient lookups into a natural conversation. Your agent can instantly search for food items, audit recipe metadata, and retrieve detailed composition reports without you ever touching a diet app. Whether you are building a nutrition tracker or conducting health research, your agent acts as a real-time dietitian, ensuring your data is always accurate and well-categorized.

### What you can do

- **Food Auditing** — Search for thousands of food items and retrieve detailed nutrient metadata, including calories, fats, and proteins.
- **Recipe Oversight** — Browse a comprehensive recipe database and retrieve detailed preparation metadata and nutritional breakdowns.
- **Barcode Discovery** — Query food IDs using barcodes (UPC/EAN) to maintain strict control over branded product data.
- **Dietary Intelligence** — Retrieve detailed nutrient information for specific food IDs to assist in analytical meal planning.
- **Category Monitoring** — List high-level food categories to understand the organizational hierarchy of nutritional data.

### How it works

1. Subscribe to this server
2. Enter your FatSecret Client ID and Client Secret
3. Start managing your nutritional intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Nutritionists & Coaches** — monitor client food choices and retrieve verified nutrient metadata straight from your workflow.
- **App Developers** — verify food data accuracy and audit recipe distributions for health-tech projects.
- **Health Enthusiasts** — perform rapid audits of food items and discover recipe desgloses through natural language.
- **Operations Leads** — automate nutritional data querying to orchestrate cross-functional wellness teams smoothly.


## Available Tools
- **get_food_by_barcode**: Get food details by barcode (UPC/EAN)
- **get_food_details**: Get detailed nutrient information for a specific food ID
- **get_recipe_details**: Get full details for a specific recipe ID
- **list_food_categories**: List high-level food categories
- **search_foods**: Search for food items in the FatSecret database
- **search_recipes**: Search for recipes by keywords


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FatSecret Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'avocado' in FatSecret and show me the nutrient details."

**🤖 AI Agent:**
> I've retrieved several entries for avocado. A standard serving contains about 160 calories and 15g of healthy fats. Would you like the full breakdown for a specific weight?

---

**👤 You:**
> "Find healthy recipes with 'salmon'."

**🤖 AI Agent:**
> I've found 5 healthy salmon recipes. Notable options include 'Grilled Salmon with Asparagus' and 'Lemon Baked Salmon'. Would you like the preparation steps or nutritional metadata?

---

**👤 You:**
> "What food corresponds to barcode 0748927020108?"

**🤖 AI Agent:**
> I've identified that barcode as 'Quest Bar - Chocolate Chip Cookie Dough'. I can retrieve the full nutritional profile for this product if you'd like.


## Installation & Usage

To install and use the **FatSecret Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fatsecret-platform](https://vinkius.com/mcp/fatsecret-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
