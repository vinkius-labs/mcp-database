# CheapShark MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cheapshark)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cheapshark-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cheapshark-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Find the best PC game deals across multiple stores. Search for games, compare prices, and set price alerts directly from your AI agent.

## Description
Connect to **CheapShark** and never miss a PC game deal again. This MCP server allows your AI agent to query the massive CheapShark database to find the lowest prices across major digital storefronts like Steam, Epic Games Store, GOG, and more.

### What you can do

- **Browse Deals** — Get a list of current top deals with filters for price, ratings, and specific stores.
- **Game Search** — Find specific titles or search by Steam App ID to get unique game identifiers.
- **Price Comparison** — Retrieve detailed information for a specific game, including its cheapest price ever and current offers across all tracked stores.
- **Store Directory** — List all stores tracked by CheapShark to map IDs to store names.
- **Price Alerts** — Set up email notifications to be alerted when a game drops below your target price.

### How it works

1. Subscribe to this server
2. No API key is required for public queries
3. Start hunting for deals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gamers** — find the absolute lowest price for that game on your wishlist without checking ten different sites
- **Deal Hunters** — automate the monitoring of price drops and historical lows
- **Content Creators** — quickly pull current pricing data for game recommendations or reviews


## Available Tools
- **get_deals**: Retrieve a list of current game deals
- **get_game**: Get specific game details by ID
- **manage_alert**: Manage email alerts for game price drops
- **search_games**: Search for games by title or Steam App ID
- **get_stores**: Good for mapping storeIDs from deals.

Get a list of all stores tracked by CheapShark


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CheapShark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the game 'Elden Ring' to get its ID."

**🤖 AI Agent:**
> I found 'Elden Ring' with Game ID: 237788. It's currently available on several stores. Would you like to see the best current deals for it?

---

**👤 You:**
> "Show me the best deals for games under $20 with a Metacritic score over 80."

**🤖 AI Agent:**
> I've filtered the current deals for you. Top picks include 'The Witcher 3: Wild Hunt' at $12.49 (Metacritic: 93) and 'Hades' at $14.99 (Metacritic: 93).

---

**👤 You:**
> "Set a price alert for game ID 237788 to notify me at gamer@example.com if it drops below $30."

**🤖 AI Agent:**
> Success! I've set a price alert for 'Elden Ring' (ID: 237788). You will receive an email at gamer@example.com as soon as the price hits $30.00 or lower.


## Installation & Usage

To install and use the **CheapShark** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cheapshark](https://vinkius.com/mcp/cheapshark)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
