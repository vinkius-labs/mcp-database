# Gamma (AI Presentations) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gamma-ai-presentations)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gamma-ai-presentations-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gamma-ai-presentations-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate AI-powered presentations, documents, and webpages. List, update, and manage your Gamma workspace directly from any AI agent.

## Description
Connect **Gamma** to your AI agent to transform prompts into beautiful presentations, documents, or webpages instantly. Streamline your creative workflow by generating and managing content through natural language.

### What you can do

- **AI Creation** — Use `create_gamma` to generate presentations, documents, or webpages from a simple prompt or a detailed outline.
- **Content Management** — Retrieve specific details of any creation with `get_gamma` or list your entire library using `list_gammas`.
- **Dynamic Updates** — Modify titles and content of existing Gammas on the fly with `update_gamma` to keep your information current.
- **Workspace Cleanup** — Permanently remove outdated or unnecessary content using `delete_gamma`.

### How it works

1. Subscribe to this server
2. Enter your Gamma API Key
3. Start generating professional presentations and documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & Marketing** — Quickly generate pitch decks and landing pages from campaign briefs.
- **Educators & Trainers** — Turn lesson outlines into structured presentations in seconds.
- **Product Managers** — Create product documentation and internal wikis directly from project notes.


## Available Tools
- **update_gamma**: Update an existing Gamma
- **create_gamma**: Create a new Gamma (presentation, document, or webpage)
- **delete_gamma**: Delete a Gamma
- **get_gamma**: Get details of a specific Gamma
- **list_gammas**: List all Gammas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gamma (AI Presentations)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a presentation about the future of renewable energy with a professional theme."

**🤖 AI Agent:**
> I've started creating your presentation using `create_gamma`. The type is set to 'presentation' with your prompt. I'll provide the details once it's ready.

---

**👤 You:**
> "List my 5 most recent Gammas."

**🤖 AI Agent:**
> Fetching your library... I found your 5 most recent Gammas using `list_gammas`. Here they are: [List of Gammas with IDs and Titles].

---

**👤 You:**
> "Get the content and status for Gamma ID gam_12345."

**🤖 AI Agent:**
> Retrieving details for `gam_12345`... The status is 'completed' and the title is 'Q3 Strategy'. Would you like to see the full content outline?


## Installation & Usage

To install and use the **Gamma (AI Presentations)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gamma-ai-presentations](https://vinkius.com/mcp/gamma-ai-presentations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
