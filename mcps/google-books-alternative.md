# Google Books MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-books-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-books-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-books-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search the world's most comprehensive index of full-text books, manage personal bookshelves, and retrieve detailed literary metadata.

## Description
Connect your **Google Books** library to any AI agent to explore millions of titles and organize your reading life through natural conversation.

### What you can do

- **Deep Search** — Perform full-text searches using advanced filters like title, author, publisher, subject, or ISBN.
- **Volume Metadata** — Fetch complete details for any book or magazine, including descriptions, page counts, categories, and preview links.
- **Bookshelf Management** — List and inspect public bookshelves from other users or manage your own private library.
- **Library Curation** — Add, remove, or move volumes within your personal bookshelves (requires OAuth).
- **Format Filtering** — Restrict searches to specific formats like EPUB or filter by availability (free vs. paid ebooks).

### How it works

1. Subscribe to this server
2. Enter your Google Books API Key (for searching) or OAuth Access Token (for library management)
3. Start exploring literature from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Students** — Quickly find relevant literature and extract bibliographic metadata for citations.
- **Avid Readers** — Organize your 'To Read' lists and manage your digital library without leaving your workspace.
- **Content Creators** — Verify book details, authors, and publication dates instantly during the writing process.


## Available Tools
- **add_volume_to_my_bookshelf**: 0 access token.

Add a volume to a bookshelf
- **clear_my_bookshelf**: 0 access token.

Remove all volumes from a bookshelf
- **get_my_bookshelf**: 0 access token.

Retrieve metadata for a specific bookshelf of the authenticated user
- **get_user_bookshelf**: Retrieve a specific public bookshelf for a user
- **get_volume**: Retrieve a volume by ID
- **list_my_bookshelf_volumes**: 0 access token.

Retrieve volumes on a specific bookshelf of the authenticated user
- **list_my_bookshelves**: 0 access token.

Retrieve the authenticated user's bookshelves
- **list_user_bookshelf_volumes**: Retrieve volumes on a user's public bookshelf
- **list_user_bookshelves**: Retrieve public bookshelves for a specific user
- **move_volume_in_my_bookshelf**: 0 access token.

Change the position of a volume on a bookshelf
- **remove_volume_from_my_bookshelf**: 0 access token.

Remove a volume from a bookshelf
- **search_volumes**: Use keywords like intitle:, inauthor:, inpublisher:, subject:, isbn:.

Search for books and magazines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Books** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for books about 'Artificial Intelligence' written by 'Stuart Russell'."

**🤖 AI Agent:**
> I found several volumes. The most prominent is 'Artificial Intelligence: A Modern Approach' (Volume ID: `zyTCAlS7f7cC`). Would you like to see the full description or check its availability?

---

**👤 You:**
> "List all the volumes currently in my 'To Read' bookshelf."

**🤖 AI Agent:**
> Accessing your library... You have 3 books in your 'To Read' shelf (ID: 2): 'Dune', 'Foundation', and 'Neuromancer'. Would you like the metadata for any of these?

---

**👤 You:**
> "Get the full details for the book with ID '7_f_DwAAQBAJ'."

**🤖 AI Agent:**
> Retrieving volume data... This is 'Project Hail Mary' by Andy Weir. It has 496 pages, published by Ballantine Books, and is categorized under Fiction / Science Fiction / Space Exploration.


## Installation & Usage

To install and use the **Google Books** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-books-alternative](https://vinkius.com/mcp/google-books-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
