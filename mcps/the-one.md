# The One MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/the-one)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the complete lore of Middle-earth — browse books, movies, characters, and iconic quotes from The Lord of the Rings universe.

## Description
Connect to **The One API** and bring the vast world of J.R.R. Tolkien to your AI assistant. This server provides comprehensive access to data from The Lord of the Rings and The Hobbit series.

### What you can do

- **Books & Chapters** — List all books and drill down into specific chapters using `list_books` and `list_book_chapters` to explore the narrative structure.
- **Cinematic Data** — Access details for all movies, including runtimes, budget, and award nominations via `list_movies` and `get_movie`.
- **Character Database** — Retrieve metadata for thousands of characters, including race, gender, and birth/death dates using `list_characters` and `get_character`.
- **Iconic Quotes** — Fetch thousands of quotes from the movies, searchable by character or film using `list_movie_quotes` and `list_character_quotes`.
- **Advanced Filtering** — Use pagination, sorting, and limits to manage large datasets of Middle-earth lore efficiently.

### How it works

1. Subscribe to this server
2. Enter your The One API Key (Access Token)
3. Start querying Middle-earth data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Tolkien Enthusiasts** — instantly retrieve facts, quotes, and character details without searching through wikis
- **Developers & Creatives** — integrate Middle-earth data into applications or creative writing workflows
- **Data Analysts** — explore movie statistics, character distributions, and quote frequencies


## Available Tools
- **get_book**: Get a specific book by ID
- **get_chapter**: Requires authentication.

Get a specific chapter by ID
- **get_character**: Requires authentication.

Get a specific character by ID
- **get_movie**: Get a specific movie by ID
- **get_quote**: Requires authentication.

Get a specific quote by ID
- **list_book_chapters**: Get all chapters of a specific book
- **list_books**: List all The Lord of the Rings books
- **list_chapters**: Requires authentication.

List all book chapters
- **list_character_quotes**: Requires authentication.

Get all quotes by a specific character
- **list_characters**: Requires authentication.

List all characters
- **list_movie_quotes**: Requires authentication.

Get all quotes from a specific movie
- **list_movies**: List all movies (LOTR and The Hobbit)
- **list_quotes**: Requires authentication.

List all movie quotes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **The One** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the books in The Lord of the Rings series."

**🤖 AI Agent:**
> I've retrieved the books from the database. The series includes 'The Fellowship of the Ring', 'The Two Towers', and 'The Return of the King'. Would you like to see the chapters for any of these?

---

**👤 You:**
> "Show me some quotes from the movie 'The Return of the King'."

**🤖 AI Agent:**
> Fetching quotes from 'The Return of the King' (ID: 5cd95395de30eff6ebccde5d)... Here are a few: 'I am glad you are here with me. Here at the end of all things, Sam.' and 'My friends, you bow to no one.'

---

**👤 You:**
> "Get details for the character Frodo Baggins."

**🤖 AI Agent:**
> Inspecting character data... Frodo Baggins is a Hobbit of the Shire. He was born on September 22, TA 2968. His wiki link is available for more deep lore if you're interested.


## ❓ FAQ

**Q: Can I get all quotes spoken by a specific character like Gandalf?**
Yes! Use the `list_character_quotes` tool with the character's unique ID. The agent will return a list of all recorded movie quotes for that specific character.

**Q: Does this server include data from The Hobbit movies?**
Yes, the `list_movies` tool retrieves data for both The Lord of the Rings trilogy and The Hobbit trilogy, including metadata like runtime and academy award wins.

**Q: How do I browse the chapters of a specific book?**
First, use `list_books` to find the book's ID, then use the `list_book_chapters` tool with that ID to see all chapters contained within that volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-one](https://vinkius.com/mcp/the-one)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **The One** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `the-one` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **The One** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "the-one": {
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
