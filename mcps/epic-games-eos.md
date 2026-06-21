# Epic Games EOS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epic-games-eos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/epic-games-eos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/epic-games-eos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect to Epic Online Services — lookup accounts, friends, and explore the Epic Games ecosystem.

## Description
Integrate your AI agent with **Epic Online Services (EOS)**, the high-performance backend powering some of the world's biggest games. This server allows you to interact with the Epic Games ecosystem through natural language.

### What you can do

- **Account Lookup** — Get public metadata and display names for Epic Account IDs
- **Social Integration** — Retrieve friend lists and manage social connections within the EOS framework
- **Ecosystem Search** — Explore products and services available across Epic's sandboxes and deployments
- **Cross-Platform Identity** — Verify external authentication links (Steam, Xbox, PlayStation) associated with Epic accounts

### How it works

1. Subscribe to this server
2. Enter your **Epic Client ID** and **Client Secret** (obtained from the [Epic Games Dev Portal](https://dev.epicgames.com/))
3. Start querying account and game services via chat

### Who is this for?

- **Game Developers** — quickly verify account info and social states during development
- **Community Managers** — lookup player profiles and external links
- **Gaming Enthusiasts** — interact with their Epic social graph using AI


## Available Tools
- **get_account_info**: Retrieve public account information for one or more Epic Account IDs
- **get_friends_list**: Retrieve the friends list for a specific Epic account
- **search_store_catalog**: Search the Epic Games Store catalog (Note: Requires valid Sandbox/Deployment IDs)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Epic Games EOS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get account info for Epic ID '0123456789abcdef'."

**🤖 AI Agent:**
> Retrieving data for ID '0123456789abcdef'... Display name: 'EpicExplorer'. This account is linked to Steam and PlayStation Network.


## Installation & Usage

To install and use the **Epic Games EOS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epic-games-eos](https://vinkius.com/mcp/epic-games-eos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
