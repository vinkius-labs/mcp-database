# Open Food Facts API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-food-facts-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/open-food-facts-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/open-food-facts-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Search food products — audit nutrition, barcode, and categories via AI.

## Description
Empower your AI agent to orchestrate your entire food research and nutritional auditing workflow with **Open Food Facts**, the collaborative source for global product data. By connecting the Open Food Facts API to your agent, you transform complex nutritional searches into a natural conversation. Your agent can instantly retrieve product details by barcode, audit Nutri-Scores, and query food categories without you ever touching a labeling app. Whether you are conducting dietary research or managing regional product constraints, your agent acts as a real-time nutritional consultant, ensuring your data is always verified and precise.

### What you can do

- **Product Auditing** — Retrieve high-resolution details for food products by barcode (EAN/UPC) and maintain a clear view of ingredients and brands.
- **Nutritional Oversight** — Audit the Nutri-Score and specific nutritional metadata for any product to understand the health scale instantly.
- **Category Discovery** — Browse all available food categories in the global catalog to identify relevant product markers.
- **Metadata Intelligence** — Retrieve unique product identifiers and quantity details to assist in deep-dive archival classification.
- **Operational Monitoring** — Check API status to ensure your food research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (Open Food Facts is a free and open service)
3. Start managing your food intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Nutritionists & Researchers** — monitor product quality and retrieve official metadata straight from your workflow.
- **Conscious Consumers** — verify Nutri-Scores and audit ingredient patterns without manual searching.
- **Health Apps** — perform rapid audits of food data and identify relevant stylistic markers through natural language.
- **Operations Leads** — automate food data querying to orchestrate cross-functional health teams smoothly.


## Available Tools
- **check_api_status**: Check if the Open Food Facts service is operational
- **get_food_product**: Get comprehensive details for a food product by barcode
- **list_food_categories**: List all available food categories in the database
- **search_food_products**: Search for food products by category or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Food Facts API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for product with barcode '3017620422003' (Nutella) using Open Food Facts."

**🤖 AI Agent:**
> I've retrieved the details for the Nutella! It has a Nutri-Score grade of 'E'. Notable ingredients include sugar and palm oil. Would you like the full nutritional breakdown or categories for this product?

---

**👤 You:**
> "Search for food products in the 'breakfast-cereals' category."

**🤖 AI Agent:**
> I've identified several breakfast cereals in the database! Notable entries include [Brand Name] and [Brand Name]. I can provide the Nutri-Score and quantity metadata for each of these items if you'd like.

---

**👤 You:**
> "List all food categories available in Open Food Facts."

**🤖 AI Agent:**
> I've scanned the category catalog! There are thousands of groups available, including 'beverages', 'dairies', and 'snacks'. I can help you search for specific products in any of these thematic clusters.


## Installation & Usage

To install and use the **Open Food Facts API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-food-facts-api](https://vinkius.com/mcp/open-food-facts-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
