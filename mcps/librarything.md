# LibraryThing MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/librarything)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/librarything-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/librarything-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Look up books by ISBN, explore works, and check library coverage — a bibliographic intelligence tool for AI agents.

## Description
Connect **LibraryThing** to your AI agent for instant book lookups, bibliographic data, and library coverage analysis.

### What you can do

- **ISBN Lookup** — Retrieve book details by ISBN including title, author, publication info, and ratings
- **Work Discovery** — Explore works and their editions, translations, and related metadata
- **Book Coverage** — Check which libraries hold a specific title for interlibrary research

### How it works

1. Subscribe to this server
2. Register for a [LibraryThing Developer Key](https://www.librarything.com/services/keys.php)
3. Start querying books from Claude, Cursor, or any MCP client


## Available Tools
- **get_book_coverage**: The coverage score (0-1) indicates how completely the book is cataloged on LibraryThing. Free, no API key required.

Get catalog coverage score for a book
- **get_work**: Returns title, author, coverage score (how well the work is cataloged), member count, review count and more. Free, no API key required. Use what_work to find the work ID first.

Get detailed info for a LibraryThing work
- **thing_isbn**: Useful for finding paperback, hardcover, audio, and international editions of a book. Free, no API key required.

Find all ISBNs for different editions of the same book
- **what_work**: The work ID is needed for other LibraryThing API calls. Free, no API key required.

Find the LibraryThing work ID for a book


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LibraryThing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Look up the book with ISBN 978-0-13-468599-1."

**🤖 AI Agent:**
> Found it! 'The Pragmatic Programmer' by David Thomas and Andrew Hunt. Publisher: Addison-Wesley (2019, 2nd edition). Community rating: 4.2/5 with 1,847 members. Tagged: programming, software-engineering, best-practices.


## Installation & Usage

To install and use the **LibraryThing** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/librarything](https://vinkius.com/mcp/librarything)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
