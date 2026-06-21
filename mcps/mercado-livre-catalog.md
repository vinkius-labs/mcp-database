# Mercado Livre Catalog MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mercado-livre-catalog)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mercado-livre-catalog-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mercado-livre-catalog-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Create, update, and manage product listings, stock, and prices on Mercado Livre.

## Description
Connect **Mercado Livre Catalog** to any AI agent and streamline your e-commerce operations — manage listings, adjust stock levels, update prices, and discover categories through natural conversation.

### What you can do
- **Create Listings** — Publish new products with full details and attributes
- **Stock Management** — Update inventory levels instantly across all listings
- **Price Updates** — Change prices dynamically to stay competitive
- **Search & Discovery** — Find your active listings and browse categories
- **Attribute Management** — Get mandatory attributes for specific categories (e.g., voltage, size)
- **Deactivation** — Close listings that are no longer available

### How it works
1. Subscribe to this server
2. Enter your Mercado Livre OAuth2 Access Token
3. Start managing your catalog from Claude, Cursor, or any MCP-compatible client

Mercado Livre is the largest e-commerce ecosystem in Latin America.

### Who is this for?
- **E-commerce Sellers** — Keep stock and prices up-to-date without logging into the Seller Panel
- **Inventory Managers** — Automate stock replenishment alerts and updates via AI
- **Digital Marketers** — Quickly publish new campaigns and listings directly from chat


## Available Tools
- **get_domain_attributes**: Get required attributes for a category/domain
- **get_categories**: List top-level categories of Mercado Livre Brasil
- **create_item**: Create a new listing
- **delete_item**: Deactivate a listing (close it)
- **get_item**: Get details of a specific listing
- **update_price**: Update the price of an item
- **search_items**: Note: Full search parameters are available via query string in documentation.

Search for listings belonging to the authenticated user
- **update_stock**: Update available quantity for an item
- **update_item**: Update a listing (title, description, attributes)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mercado Livre Catalog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Update the price of item MLB123456 to R$99.90."

**🤖 AI Agent:**
> Price updated successfully! Item is now active at R$99.90.

---

**👤 You:**
> "Create a new listing for a 'Wireless Mouse' in category 'Accessories'."

**🤖 AI Agent:**
> Listing created successfully! ID: MLB789012345. It is now live in the site.

---

**👤 You:**
> "What are the mandatory attributes for the Cellphones category?"

**🤖 AI Agent:**
> Required attributes: Brand, Model, Storage Capacity, Color, Screen Size, RAM.


## Installation & Usage

To install and use the **Mercado Livre Catalog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mercado-livre-catalog](https://vinkius.com/mcp/mercado-livre-catalog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
