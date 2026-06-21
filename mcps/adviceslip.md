# Adviceslip MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adviceslip)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/adviceslip-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/adviceslip-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access over 10 million pieces of advice directly from your AI agent — get random wisdom, search by keyword, or retrieve specific slips by ID.

## Description
Connect to the **Adviceslip** API to empower your AI agent with a massive database of human wisdom. This server provides tools to fetch random advice, search for specific topics, or look up advice by its unique identifier.

### What you can do

- **Random Advice** — Use `get_random_advice` to receive a spontaneous piece of wisdom to inspire your day.
- **Keyword Search** — Use `search_advice` to find all advice slips containing a specific word or phrase (e.g., 'success', 'friendship', 'coding').
- **Direct Lookup** — Use `get_advice_by_id` to retrieve a specific slip when you know its unique numeric ID.

### How it works

1. Subscribe to this server
2. No authentication is required for this public API
3. Start asking for wisdom in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Integrating 'Advice of the Day' features into apps or terminal workflows.
- **Content Creators** — Looking for quick inspiration, unique prompts, or philosophical nuggets.
- **Daily Users** — Seeking a bit of perspective or a quick mental break during their workflow.


## Available Tools
- **adviceslip_get_by_id**: Get a specific advice slip by ID
- **adviceslip_get_random**: Get a random piece of advice
- **adviceslip_search**: Search for advice slips containing a specific term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adviceslip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a random piece of advice."

**🤖 AI Agent:**
> I've fetched a random advice slip for you: 'Remember that as far as anyone else is concerned, you're just another person in the street.' (ID: 142)

---

**👤 You:**
> "Search for advice about 'spiders'."

**🤖 AI Agent:**
> I found an advice slip about spiders: 'If you're ever attacked by a group of clowns, go for the juggler.' Wait, that's a joke! Let me find a real one... 'Never trust a spider.' (ID: 83)

---

**👤 You:**
> "What is the advice slip with ID 50?"

**🤖 AI Agent:**
> Advice slip #50 is: 'Don't always take advice from others.' A bit ironic, isn't it?


## Installation & Usage

To install and use the **Adviceslip** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adviceslip](https://vinkius.com/mcp/adviceslip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
