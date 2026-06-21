# Project Gutenberg MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/project-gutenberg)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/project-gutenberg-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/project-gutenberg-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Universal public domain library — search and retrieve thousands of free books via AI.

## Description
Equip your AI agent with the largest library of free public domain books through the **Project Gutenberg** MCP server. This integration provides access to over 60,000 eBooks, allowing your agent to search for classic literature, retrieve detailed metadata for specific titles, and explore works by your favorite authors. Whether you're conducting literary research, looking for historical texts, or simply seeking a new read, your agent acts as a dedicated digital librarian through natural conversation.

### What you can do

- **Book Search** — Find classic books by title, keyword, or subject across a massive collection.
- **Author Exploration** — List all available works by a specific author registered in the database.
- **Metadata Retrieval** — Fetch IDs, languages, and detailed info for any book in the collection.
- **Literary Auditing** — Summarize multiple classic works to compare themes and historical contexts.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start searching for books from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Students & Academics** — access primary sources and classic literature for studies.
- **Literature Lovers** — discover new gems in the public domain.
- **Researchers** — identify historical texts and various editions of classic works.
- **Digital Humanists** — retrieve structured metadata for large-scale literary analysis.


## Available Tools
- **search_author**: Search for books by author
- **get_book_details**: Get details for a specific Gutenberg book
- **search_gutenberg_books**: Search for books on Project Gutenberg


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Project Gutenberg** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the book 'Pride and Prejudice' on Project Gutenberg."

**🤖 AI Agent:**
> Searching... I found 'Pride and Prejudice' by Jane Austen. Its Project Gutenberg ID is 1342. Would you like me to retrieve more details about this edition?

---

**👤 You:**
> "List all available works by 'Mark Twain'."

**🤖 AI Agent:**
> Retrieving Mark Twain's bibliography... I've found classics like 'The Adventures of Tom Sawyer' and 'Adventures of Huckleberry Finn'. Shall I provide the IDs for these and other available titles?

---

**👤 You:**
> "Search for books about 'Philosophy'."

**🤖 AI Agent:**
> Scanning the collection for philosophy... I found several works including titles by Plato, Nietzsche, and Spinoza. I can list the most downloaded ones if you'd like to narrow down your search.


## Installation & Usage

To install and use the **Project Gutenberg** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/project-gutenberg](https://vinkius.com/mcp/project-gutenberg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
