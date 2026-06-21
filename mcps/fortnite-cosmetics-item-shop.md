# Fortnite Cosmetics & Item Shop MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fortnite-cosmetics-item-shop)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fortnite-cosmetics-item-shop-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fortnite-cosmetics-item-shop-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

The definitive server for Fortnite cosmetics — track daily shop rotations, leaked skins, and rarity via AI.

## Description
Equip your AI agent with real-time intelligence for the world's most dynamic gaming marketplace via **Fortnite Cosmetics & Item Shop**. This server provides deep access to the official Fortnite-API.com database, allowing your agent to instantly retrieve the daily 'Featured' and 'Daily' shop items, monitor unreleased 'Leaked' skins found in game files, and audit technical metadata for thousands of cosmetics. From tracking the 'Last Seen' history of rare outfits to searching for specific item sets, your agent acts as a professional Fortnite consultant through natural conversation.

### What you can do

- **Shop Monitoring** — Instantly retrieve the current V-Bucks prices and bundles available in the real-time shop rotation
- **Leak Intelligence** — List unreleased items and newly added cosmetics to stay ahead of upcoming seasonal events
- **Rarity Auditing** — Search and filter the complete database by rarity (Legendary, Epic), item types, and official sets
- **Visual Retrieval** — Retrieve high-quality icon URLs and descriptions for skins, emotes, gliders, and pickaxes

### How it works

1. Subscribe to this server
2. Enter your Fortnite-API Key (obtainable via their official dashboard)
3. Start managing your Fortnite cosmetics strategy from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gaming Enthusiasts** — stay updated on the shop and never miss a rare skin return
- **Content Creators** — instantly retrieve high-quality icons and technical data for reporting and videos
- **Collectors & Traders** — perform deep audits of skin history and rarity distribution across the ecosystem


## Available Tools
- **get_cosmetic_details**: Get full details for a specific cosmetic by ID
- **get_new_cosmetics**: List newly added and leaked cosmetics
- **get_item_shop**: Updated at 00:00 UTC.

Get the current daily and featured item shop
- **get_combined_shop**: Get the full combined item shop data
- **list_banners**: List all profile banner icons
- **search_cosmetics_by_rarity**: Rarities: common, uncommon, rare, epic, legendary, marvel, dc, icon, gaminglegends.

Find cosmetics filtered by rarity tier
- **search_cosmetics_by_type**: Types: outfit, backpack, pickaxe, glider, emote, wrap, loadingscreen, spray, emoji, music.

Find cosmetics filtered by item type
- **search_cosmetics**: Returns images, rarity, set info, and introduction date.

Search for cosmetics by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fortnite Cosmetics & Item Shop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's featured items in the Fortnite shop and their prices."

**🤖 AI Agent:**
> Retrieving today's shop rotation... I've identified 5 featured items including the 'Aura' skin (800 V-Bucks) and the 'Star Power' emote. I also found a new discounted bundle. Would you like the direct icon preview for these items?

---

**👤 You:**
> "Search for all items in the 'Frozen Series' and list their rarities."

**🤖 AI Agent:**
> Running the set query for 'Frozen Series'... I found 6 items including 'Frozen Love Ranger' and 'Frozen Raven'. Most items in this set are of 'Frozen' rarity. Shall I provide the detailed descriptions for each?

---

**👤 You:**
> "What are the latest leaked skins found in today's game update?"

**🤖 AI Agent:**
> Inspecting latest patch leaks... I've identified 3 new unreleased skins: 'Skin Name X', 'Skin Name Y', and an upcoming crossover emote. These are not yet in the shop but appear in the database files. Would you like the high-res icon URLs?


## Installation & Usage

To install and use the **Fortnite Cosmetics & Item Shop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fortnite-cosmetics-item-shop](https://vinkius.com/mcp/fortnite-cosmetics-item-shop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
