# Akeneo PIM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/akeneo-pim)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/akeneo-pim-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/akeneo-pim-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Product Information Management orchestration — manage products, attributes, and categories via AI.

## Description
Connect your **Akeneo PIM** instance to your AI agent to unlock professional product data orchestration. From auditing product technical metadata and localized descriptions to managing attribute groups and category trees, your agent handles your e-commerce catalog through natural conversation.

### What you can do

- **Product Orchestration** — List and retrieve details for products using identifiers or UUIDs, and update attributes seamlessly
- **Taxonomy Management** — List and audit category trees to ensure your product classification is always consistent
- **Attribute Oversight** — List available attributes and families to understand your PIM's data structure
- **Channel & Locale Auditing** — Retrieve configured channels and locales to manage multi-market product data
- **Catalog Insights** — Quickly identify incomplete product records or audit attribute values directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Akeneo Base URL, Client ID, Secret, Username, and Password
3. Start managing your product data and monitoring catalog health through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — automate product status updates and monitor catalog consistency across channels
- **PIM Stewards** — audit attribute values and manage category assignments effortlessly
- **Product Owners** — research product technical specs and localized content using simple commands
- **Data Engineers** — verify API integration and inspect product JSON responses on the fly


## Available Tools
- **list_products**: Supports cursor-based pagination.

List PIM products
- **get_product_details**: Get product metadata
- **update_product**: Update product attributes
- **list_categories**: List category trees
- **get_category_details**: Get category metadata
- **list_attributes**: List product attributes
- **get_attribute_details**: Get attribute metadata
- **list_families**: List product families
- **list_channels**: g. Mobile, Web) configured in the PIM.

List sales channels
- **list_locales**: List enabled languages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Akeneo PIM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 products updated in my Akeneo PIM."

**🤖 AI Agent:**
> I've retrieved the latest 5 products. They include 'Wireless Headset v2', 'Ergonomic Desk', and 3 others. Would you like to see the completeness status for any of them?

---

**👤 You:**
> "Show details for product identifier 'SKU-98765'."

**🤖 AI Agent:**
> I've retrieved the details for SKU-98765. It belongs to the 'Electronics' family and has active attributes for 'Weight', 'Color', and 'Battery Life'. It is currently enabled in 2 channels: 'E-commerce' and 'Mobile App'.

---

**👤 You:**
> "List all attributes in the 'Marketing' group."

**🤖 AI Agent:**
> I've retrieved the attributes for the Marketing group. It contains 12 attributes including 'Description_EN', 'SEO_Keywords', and 'Promotional_Text'. Would you like to see the validation rules for any of these?


## Installation & Usage

To install and use the **Akeneo PIM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/akeneo-pim](https://vinkius.com/mcp/akeneo-pim)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
