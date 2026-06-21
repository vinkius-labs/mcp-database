# Roblox Avatar & Catalog Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roblox-avatar-catalog-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/roblox-avatar-catalog-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/roblox-avatar-catalog-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Universal Roblox marketplace intelligence — audit item prices, bundles, and user inventories via AI.

## Description
Equip your AI agent with deep intelligence for the **Roblox Avatar Shop** and virtual economy. This advanced MCP server provides direct access to the official Roblox Catalog, allowing your agent to instantly search for thousands of assets, audit item prices in Robux, retrieve detailed bundle metadata, and analyze user inventories. Whether you are a trader tracking rare Limited items or a creator auditing the marketplace, your agent acts as a professional virtual asset broker through natural conversation.

### What you can do

- **Marketplace Auditing** — Search the entire Avatar Shop for clothing, accessories, and gear matching specific keywords.
- **Asset Intelligence** — Retrieve granular technical metadata for items and bundles including price, stock, and creator info.
- **Rarity Tracking** — List Limited and Limited U items to monitor the most exclusive assets in the Roblox ecosystem.
- **Inventory Analysis** — Fetch public inventory data for any user to identify owned assets and total collection value.

### How it works

1. Subscribe to this server
2. No API key required for public catalog discovery
3. Start managing your Roblox assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Virtual Asset Traders** — instantly audit item prices and rarity to identify optimal trading opportunities.
- **Roblox Creators** — monitor marketplace trends and competitor assets directly from your workflow.
- **Analytical Gamers** — track your inventory progress and collection value with precision.


## Available Tools
- **get_asset_thumbnails**: Get high-resolution thumbnails for one or more assets
- **get_avatar_bundle_details**: Get details for a specific avatar bundle
- **get_bundle_recommendations**: Get recommended bundles similar to a given one
- **get_catalog_item_details**: Get full metadata for an asset by ID
- **get_limited_resale_data**: Get resale price history for a Limited item
- **get_limited_resellers**: List current resellers for a Limited item
- **get_user_catalog_inventory**: Asset types: Hat, Gear, Face, Package, HairAccessory, etc.

Browse the public inventory of a Roblox user
- **search_avatar_catalog**: Supports category and sort filters.

Search for items in the Roblox Avatar Shop


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roblox Avatar & Catalog Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Valkyrie' hats in the catalog and show the cheapest active listing."

**🤖 AI Agent:**
> Running the catalog query for 'Valkyrie'... I found 3 matching items. The 'Valkyrie Helm' is currently a Limited item. I've identified the cheapest active listing at 55,000 Robux. Would you like to see the other variations?

---

**👤 You:**
> "What items are included in the 'Korblox Deathspeaker' bundle?"

**🤖 AI Agent:**
> Inspecting bundle ID '192'... The 'Korblox Deathspeaker' bundle includes 7 items, most notably the legendary 'Korblox Deathspeaker Right Leg'. The current price is 17,000 Robux. Shall I provide the IDs for each component?

---

**👤 You:**
> "Audit the inventory of user ID '7654321' and list their 5 most expensive items."

**🤖 AI Agent:**
> Retrieving user assets... User '7654321' has 150 public items. Their top 5 most expensive assets include 'Dominus Empyreus' and 'Clockwork's Headphones'. The total estimated value of these 5 items is 1.2M Robux. Would you like the full breakdown?


## Installation & Usage

To install and use the **Roblox Avatar & Catalog Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roblox-avatar-catalog-intelligence](https://vinkius.com/mcp/roblox-avatar-catalog-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
