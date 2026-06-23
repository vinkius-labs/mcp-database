# Open Library MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-library-extended)
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


## Available Tools (17)
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


## ❓ FAQ

**Q: Can I look up a book if I only have its ISBN?**
Yes! Use the `get_books_by_bibkeys` tool and provide the ISBN (e.g., 'ISBN:0451526538'). The agent will return the book metadata associated with that specific identifier.

**Q: How do I see all the different versions or publications of a specific book?**
You can use the `get_work_editions` tool with a Work ID (like 'OL27258W'). This will list the various physical editions and formats linked to that core literary work.

**Q: Can I search for authors by their name instead of an ID?**
Absolutely. Use the `search_authors` tool with a name query. Once you find the correct author, you can use their ID with `get_author` or `get_author_works` for more details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-library-extended](https://vinkius.com/mcp/open-library-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open Library** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `open-library-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open Library** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-library-extended": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
