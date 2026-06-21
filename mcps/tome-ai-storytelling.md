# Tome (AI Storytelling) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tome-ai-storytelling)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tome-ai-storytelling-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tome-ai-storytelling-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate and manage AI-powered presentations via Tome — list workspaces, manage tomes, and add pages directly from any AI agent.

## Description
Connect your **Tome** account to any AI agent to streamline your AI-driven storytelling and presentation workflows through natural conversation.

### What you can do

- **Workspaces & Tomes** — List all accessible workspaces and fetch active tomes directly from the Tome cloud
- **Tome Management** — Create new tomes in specific workspaces and organize your storytelling projects
- **Page Operations** — Add new pages to existing tomes to expand your narrative dynamically
- **Deep Inspection** — Fetch complete metadata and page details for specific tomes to understand their structure

### How it works

1. Subscribe to this server
2. Enter your Tome API Key
3. Start generating presentations from Claude, Cursor, or any MCP-compatible client

No more manual slide creation. Your AI acts as a creative director, building out your vision page by page.

### Who is this for?

- **Content Creators** — instantly scaffold stories and presentations without leaving your AI chat
- **Marketing Teams** — manage workspace assets and create new campaign decks via automation
- **Product Managers** — document features and roadmaps by generating tomes directly from project specs


## Available Tools
- **add_page**: Add a new page to an existing tome
- **create_tome**: Create a new tome in a workspace
- **get_tome**: Get detailed information about a specific tome
- **list_tomes**: List tomes in a workspace
- **list_workspaces**: List Tome workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tome (AI Storytelling)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Tome workspaces."

**🤖 AI Agent:**
> I've retrieved your workspaces. You have access to: 'Personal Space' (ID: ws_987) and 'Design Team' (ID: ws_654). Which one would you like to explore?

---

**👤 You:**
> "Create a new tome titled 'Product Roadmap 2025' in workspace ws_987."

**🤖 AI Agent:**
> Successfully created! Your new tome 'Product Roadmap 2025' is now live in your Personal Space with ID: tome_abc123. Would you like to add the first page?

---

**👤 You:**
> "Add a page called 'Market Analysis' to tome tome_abc123."

**🤖 AI Agent:**
> Done. I've added the 'Market Analysis' page to your tome. You can now see it in the presentation structure.


## Installation & Usage

To install and use the **Tome (AI Storytelling)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tome-ai-storytelling](https://vinkius.com/mcp/tome-ai-storytelling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
