# An API of Ice And Fire MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/an-api-of-ice-and-fire)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/an-api-of-ice-and-fire-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/an-api-of-ice-and-fire-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Explore the world of A Song of Ice and Fire — query books, characters, and noble houses of Westeros directly from any AI agent.

## Description
Connect the definitive **A Song of Ice and Fire** database to your AI agent and explore the lore of George R.R. Martin's universe through natural conversation.

### What you can do

- **Literary Catalog** — List all books in the series and retrieve metadata like ISBN, page counts, and POV characters via `list_books` and `get_book`.
- **Character Biographies** — Search thousands of characters by name, gender, or culture. Get details on titles, aliases, and family ties using `list_characters` and `get_character`.
- **Great Houses** — Explore the noble houses of the Seven Kingdoms. Query regions, mottos (words), and ancestral seats with `list_houses` and `get_house`.
- **Lore Integration** — Perfect for writers, fans, and researchers looking to verify facts about Westeros and Essos without leaving their workspace.

### How it works

1. Subscribe to this server
2. No complex configuration needed for this public API
3. Start querying the Seven Kingdoms from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Writers & Creatives** — quickly verify character details or house words while drafting content
- **Fans & Researchers** — explore the complex genealogy and history of the series
- **Developers** — integrate high-quality fantasy metadata into applications or creative tools


## Available Tools
- **get_book**: Get details for a specific book
- **get_character**: Get details for a specific character
- **get_house**: Get details for a specific house
- **list_books**: List books in the A Song of Ice and Fire series
- **list_characters**: Can be filtered by name, gender, or culture.

List characters in the Ice and Fire universe
- **list_houses**: Can be filtered by name, region, or words.

List noble houses of Westeros and beyond


## 💬 Prompt Examples

Here are some examples of how you can interact with the **An API of Ice And Fire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the books in the A Song of Ice and Fire series."

**🤖 AI Agent:**
> I've retrieved the list of books. There are several entries including 'A Game of Thrones', 'A Clash of Kings', and 'A Storm of Swords'. Would you like the details for a specific one?

---

**👤 You:**
> "Find characters from the Valyrian culture."

**🤖 AI Agent:**
> Searching for Valyrian characters... I found several, including Aegon Targaryen and Daenerys Targaryen. Would you like me to fetch the full metadata for any of these characters using their ID?

---

**👤 You:**
> "Get the details for House Stark using its ID 362."

**🤖 AI Agent:**
> Inspecting House Stark (ID: 362)... Their region is 'The North', their seat is 'Winterfell', and their words are 'Winter is Coming'. They also possess the ancestral weapon 'Ice'.


## Installation & Usage

To install and use the **An API of Ice And Fire** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/an-api-of-ice-and-fire](https://vinkius.com/mcp/an-api-of-ice-and-fire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
