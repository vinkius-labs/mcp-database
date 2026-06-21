# TarotAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tarotapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tarotapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tarotapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Draw tarot cards, get readings, and explore card meanings via AI.

## Description
Connect **TarotAPI** to any AI agent and access the complete 78-card tarot deck with detailed meanings, keywords, fortune telling interpretations, and card imagery through natural language.

### What you can do

- **Daily Draw** — Pull a random card for daily guidance and reflection
- **Full Deck Browser** — Explore all 78 Major and Minor Arcana cards
- **Detailed Readings** — Get upright and reversed meanings, keywords, and fortune telling interpretations for any card
- **Multi-Card Spreads** — Draw multiple random cards for past/present/future or Celtic Cross readings
- **Meaning Search** — Find cards by their interpretive meanings or keywords
- **Card Details** — Access full card descriptions, imagery, and arcana classifications

### How it works

1. Subscribe to this server
2. No API key required — TarotAPI is free and open
3. Start reading tarot from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_api_info**: Get TarotAPI information
- **get_card**: Includes full meanings (upright and reversed), keywords, fortune telling interpretations, description, and card image. Use short names like "ar01" (The Magician), "swac" (Ace of Cups), "wa02" (Two of Wands), etc.

Get detailed information about a specific tarot card
- **get_random_card**: Perfect for daily draws, quick readings, or when you need guidance from the tarot without specifying a particular card.

Get a random tarot card for a daily reading
- **get_multiple_random_cards**: Useful for multi-card spreads like three-card past/present/future readings or Celtic Cross layouts. Returns up to 78 cards (full deck).

Get multiple random tarot cards for a spread
- **list_all_cards**: Returns card names, numbers, arcana types, suits, and short names. Use this to browse the full deck or find card identifiers for detailed lookups.

List all 78 tarot cards
- **search_cards**: Supports searching by upright meaning, reversed meaning, or general text query. Returns all cards that match the search criteria with full card details.

Search tarot cards by meaning or keywords


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TarotAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Pull a card for my daily reading."

**🤖 AI Agent:**
> Your card for today is **The Empress** (III) — Major Arcana. Keywords: fertility, femininity, beauty, nature, abundance. This card suggests nurturing energy and creative growth. Embrace beauty and abundance in your life today.

---

**👤 You:**
> "Give me a three-card past/present/future reading."

**🤖 AI Agent:**
> Your three-card spread:

**Past**: The Tower — Sudden change and upheaval. A structure in your life crumbled, making way for new growth.

**Present**: Four of Pentacles — Holding on tight to resources. You may be feeling protective of what you have.

**Future**: The Star — Hope, renewal, and inspiration. After the storm, peace and healing are coming.

---

**👤 You:**
> "What does The Fool card mean in tarot?"

**🤖 AI Agent:**
> **The Fool (0)** — Major Arcana. Keywords: innocence, beginnings, freedom, innocence, a free spirit. Upright meaning: new beginnings, optimism, trust, and the start of a journey. Reversed meaning: recklessness, risk-taking, naivety. Fortune telling: a new adventure is beginning; embrace the unknown with an open heart.


## Installation & Usage

To install and use the **TarotAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tarotapi](https://vinkius.com/mcp/tarotapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
