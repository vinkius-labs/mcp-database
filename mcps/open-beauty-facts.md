# Open Beauty Facts MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-beauty-facts)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/open-beauty-facts-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/open-beauty-facts-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Universal cosmetics intelligence — search ingredients, allergens, and brands via AI.

## Description
Equip your AI agent with the definitive open database for cosmetic products through the **Open Beauty Facts** MCP server. This integration provides real-time access to a collaborative database of beauty products from around the world. Your agent can search for cosmetics by name or barcode, retrieve detailed lists of ingredients (INCI), and identify potential allergens or restricted substances. Whether you are auditing your skincare routine, researching cosmetic formulations, or verifying product claims, your agent acts as a dedicated personal care specialist through natural conversation.

### What you can do

- **Product Lookup** — Find cosmetic products by name, brand, or EAN/UPC barcode.
- **Ingredient Analysis** — Retrieve the complete INCI list for thousands of beauty and hygiene products.
- **Allergen Detection** — Identify potential allergens and irritants in specific formulations.
- **Brand Auditing** — Explore the product portfolios of global cosmetic brands.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying cosmetic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Conscious Consumers** — audit the ingredients of their personal care products.
- **Dermatologists & Professionals** — quickly verify formulations and potential irritants for patients.
- **Cosmetic Researchers** — analyze industry trends and ingredient usage across brands.
- **Health Tech Developers** — integrate open cosmetic data into their wellness applications.


## Available Tools
- **get_beauty_product**: Get cosmetic product details by barcode
- **search_beauty_products**: Search for beauty products by category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Beauty Facts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for cosmetic products from the brand 'Nivea'."

**🤖 AI Agent:**
> Searching the Open Beauty Facts database... I've found a wide range of products from Nivea, including face creams, body lotions, and sunscreens. Would you like to see the ingredients for a specific product?

---

**👤 You:**
> "What are the ingredients in the product with barcode '4005900130778'?"

**🤖 AI Agent:**
> Retrieving product details... This barcode belongs to a Nivea Creme. The main ingredients include Water, Paraffinum Liquidum, Cera Microcristallina, Glycerin, and Lanolin Alcohol. It also contains several fragrance components.

---

**👤 You:**
> "Identify potential allergens in 'La Roche-Posay Anthelios'."

**🤖 AI Agent:**
> Analyzing the product data... For the Anthelios sunscreen line, I've identified that most formulations are designed for sensitive skin, but some versions may contain Alcohol Denat or specific preservatives. I can provide the full list for a specific variant.


## Installation & Usage

To install and use the **Open Beauty Facts** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-beauty-facts](https://vinkius.com/mcp/open-beauty-facts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
