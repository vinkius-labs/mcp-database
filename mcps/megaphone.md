# Megaphone MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/megaphone)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/megaphone-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/megaphone-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Podcast publishing and ad management via Megaphone — manage networks, podcasts, and campaigns.

## Description
Connect your **Megaphone** account to any AI agent and take full control of your podcast publishing and advertisement workflows through natural conversation.

### What you can do

- **Network Management** — List all podcast networks and fetch detailed metadata for specific organizations
- **Podcast Orchestration** — Enumerate podcasts within a network and retrieve detailed show configurations
- **Episode Operations** — List and inspect episodes, search across your library, and verify publish statuses
- **Ad Campaign Management** — Manage ad campaigns, ad locations, and track advertisement orders natively

### How it works

1. Subscribe to this server
2. Enter your Megaphone API Token
3. Start managing your podcast library from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_episode**: Get episode details
- **get_network_details**: Get network details
- **get_podcast**: Get podcast details
- **list_ad_locations**: List ad locations for an episode
- **list_campaigns**: List ad campaigns in a network
- **list_episodes**: List episodes for a podcast
- **list_networks**: List all podcast networks
- **list_orders**: List ad orders in a network
- **list_podcasts**: List podcasts in a network
- **search_episodes**: Search episodes across a network


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Megaphone** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all podcasts in my network."

**🤖 AI Agent:**
> Retrieving podcasts... I found several active shows including 'Daily Tech News' and 'Marketing Insights'.

---

**👤 You:**
> "Search for episodes about 'Artificial Intelligence'."

**🤖 AI Agent:**
> Searching... I identified 3 episodes covering AI topics across your network.

---

**👤 You:**
> "Show active ad campaigns for network ID 123."

**🤖 AI Agent:**
> Querying campaigns... Network 123 has 5 active ad campaigns including 'Spring Sale' and 'New Product Launch'.


## Installation & Usage

To install and use the **Megaphone** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/megaphone](https://vinkius.com/mcp/megaphone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
