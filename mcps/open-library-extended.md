# Open Library MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-library-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/open-library-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/open-library-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the world's largest open book catalog — search books, authors, and works, and explore user-created lists directly from any AI agent.

## Description
Connect to the **Open Library** database and turn your AI into a master librarian. Access millions of records, from classic literature to modern scientific papers, using the Internet Archive's open catalog.

### What you can do

- **Comprehensive Book Search** — Find titles using keywords, specific authors, or advanced filters like language and publication date via `search_books`.
- **Author Deep-Dives** — Retrieve biographies, metadata, and the complete bibliography of any author using `get_author` and `get_author_works`.
- **Works vs. Editions** — Distinguish between abstract literary works and specific physical publications with `get_work` and `get_edition`.
- **Identifier Lookup** — Instantly fetch book data using standard industry codes like ISBN, OCLC, LCCN, or Open Library IDs via `get_books_by_bibkeys`.
- **Curated Lists & Subjects** — Explore public book lists created by the community or browse by specific subject categories using `search_lists` and `get_subject`.

### How it works

1. Subscribe to this server
2. Provide an optional User Agent string to identify your requests
3. Start exploring the global library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Students** — quickly compile bibliographies and verify publication details without leaving your research environment.
- **Developers** — integrate rich book metadata into applications or workflows using standard identifiers.
- **Bibliophiles** — discover new reads and explore the history of specific literary works through their various editions.


## Available Tools
- **get_author**: g., "OL23919A").

Get details for a specific Author
- **get_author_works**: Get works by a specific Author
- **get_books_by_bibkeys**: Format: "ISBN:xxxx", "OCLC:xxxx", etc.

Look up books by identifiers (ISBN, OCLC, LCCN, OLID)
- **get_edition**: g., "OL7353617M").

Get details for a specific Edition (Book)
- **get_list_editions**: Get editions in a specific user list
- **get_list_metadata**: Get metadata for a specific user list
- **get_list_seeds**: Get seeds (items) in a specific user list
- **get_recent_changes_by_date**: Access modifications to the Open Library database for a specific date
- **get_recent_changes**: Access a stream of modifications to the Open Library database
- **get_subject**: g., "love", "science_fiction").

Fetch books associated with a specific subject
- **get_user_books**: Retrieve a patron's public reading log
- **get_user_lists**: Get lists created by a user
- **get_work_editions**: Fetch editions of a specific Work
- **get_work**: g., "OL45804W").

Get details for a specific Work
- **search_authors**: Search for authors in Open Library
- **search_books**: Search for books in Open Library
- **search_lists**: Search for user-created book lists


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Library** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for books about 'Quantum Physics' published in English."

**🤖 AI Agent:**
> I've found several books on Quantum Physics. Top results include 'Quantum Physics for Beginners' and 'The Elegant Universe'. Would you like the details for any of these?

---

**👤 You:**
> "Get the biography and works of author Mark Twain."

**🤖 AI Agent:**
> Mark Twain (Samuel Langhorne Clemens) was an American writer. I've retrieved his profile (ID: OL18319A) and a list of his famous works like 'The Adventures of Tom Sawyer'. Shall I list more of his works?

---

**👤 You:**
> "Find all editions for the work with ID OL27258W."

**🤖 AI Agent:**
> I've found 12 editions for this work, ranging from the 1954 original hardcover to recent digital reprints. Would you like to see the specific ISBNs for these editions?


## Installation & Usage

To install and use the **Open Library** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-library-extended](https://vinkius.com/mcp/open-library-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
