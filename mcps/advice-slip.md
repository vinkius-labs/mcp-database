# Advice Slip MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/advice-slip)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/advice-slip-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/advice-slip-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Universal advice engine — get random advice or search by keyword via AI.

## Description
Equip your AI agent with a source of wisdom through the **Advice Slip** MCP server. This integration provides access to a massive database of over 10 million advice slips. Your agent can retrieve random pearls of wisdom, fetch specific advice by ID, or search for advice related to any topic. Whether you're looking for inspiration, life tips, or a bit of humor, your agent acts as a digital sage through natural conversation.

### What you can do

- **Random Advice** — Get a random piece of advice instantly.
- **Keyword Search** — Find advice related to specific topics (e.g., life, work, love).
- **Reference by ID** — Retrieve specific advice slips using their numerical identifiers.
- **Wisdom Auditing** — Summarize multiple advice slips to identify themes and insights.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start getting advice from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **General Users** — looking for daily inspiration or interesting tips.
- **Content Creators** — seeking quotes or advice snippets for their work.
- **Developers** — wanting to add a bit of personality and wisdom to their AI interactions.
- **Educators** — source snippets of practical wisdom for students and presentations.


## Available Tools
- **get_advice_by_id**: Get advice by its ID
- **get_random_advice**: Get a random piece of advice
- **search_advice**: Search for advice by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Advice Slip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a random piece of advice."

**🤖 AI Agent:**
> Here is a pearl of wisdom for you: 'Always drink a glass of water before you eat.' Would you like another one?

---

**👤 You:**
> "Search for advice related to 'success'."

**🤖 AI Agent:**
> I've searched the database for 'success'. Here is one for you: 'Success is a journey, not a destination.' I found several other slips; would you like me to list them all?

---

**👤 You:**
> "What is the advice with ID 42?"

**🤖 AI Agent:**
> Retrieving advice slip #42... It says: 'Make choices and don't look back.' A very practical piece of wisdom. Do you have another specific ID in mind?


## Installation & Usage

To install and use the **Advice Slip** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/advice-slip](https://vinkius.com/mcp/advice-slip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
