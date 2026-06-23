# PoetryDB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/poetrydb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the world's largest database of public domain poetry — search by author, title, lines, or line count directly from your AI agent.

## Description
Connect the **PoetryDB** server to your AI agent to explore thousands of classic poems and literary works through natural conversation.

### What you can do

- **Author & Title Discovery** — List all available authors and poem titles in the database to explore the collection.
- **Targeted Search** — Find specific poems by searching for author names, titles, or exact line counts.
- **Content Analysis** — Search for poems containing specific phrases or keywords within their lines.
- **Random Inspiration** — Retrieve random poems to discover new authors or styles instantly.
- **Advanced Queries** — Combine multiple criteria like author, title, and line count for precise literary research.

### How it works

1. Subscribe to this server
2. Enter your access identifier (use 'PUBLIC' for standard access)
3. Start exploring literature from Claude, Cursor, or any MCP-compatible client

No more searching through fragmented archives. Your AI acts as a digital librarian and literary scholar.

### Who is this for?

- **Writers & Creatives** — find inspiration and reference classic styles directly in your workspace.
- **Students & Educators** — quickly locate specific poems or analyze works by certain authors.
- **Developers** — integrate literary data into applications or test NLP models with rich text.


## Available Tools (8)
- **advanced_search**: g., title, author, linecount, poemcount) to filter poems. The number of fields must match the number of terms.

Perform a complex search combining multiple fields
- **list_authors**: List all authors available in PoetryDB
- **get_random_poems**: Retrieve a set of random poems
- **search_by_author**: Can perform partial or exact matches.

Search for poems by author name
- **search_by_linecount**: Search for poems with a specific number of lines
- **search_by_lines**: Search for poems containing specific text in their lines
- **search_by_title**: Can perform partial or exact matches.

Search for poems by title
- **list_titles**: List all poem titles available in PoetryDB


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PoetryDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all authors available in the PoetryDB."

**🤖 AI Agent:**
> I've retrieved the list of authors. There are hundreds of poets available, including classics like William Shakespeare, Emily Dickinson, and Edgar Allan Poe. Would you like to see poems from a specific author?

---

**👤 You:**
> "Find 3 random poems for me."

**🤖 AI Agent:**
> Here are 3 random selections from the database: 'Ozymandias' by Percy Bysshe Shelley, 'The Raven' by Edgar Allan Poe, and 'A Bird, came down the Walk' by Emily Dickinson. Shall I provide the full text for any of these?

---

**👤 You:**
> "Search for poems by John Keats that have exactly 14 lines."

**🤖 AI Agent:**
> Searching for sonnets by John Keats... I found several matches, including 'On First Looking into Chapman's Homer' and 'When I have fears that I may cease to be'. Both are 14-line sonnets. Which one would you like to read?


## ❓ FAQ

**Q: Can I search for poems that contain specific words or phrases in their text?**
Yes! Use the `search_by_lines` tool. Provide a string, and the agent will return poems that include that specific text within their lines.

**Q: Is it possible to find a poem if I only know the author and the approximate length?**
Absolutely. You can use the `advanced_search` tool to combine fields like 'author' and 'linecount' to narrow down the results to exactly what you're looking for.

**Q: How can I discover new poets I haven't read before?**
You can use `list_authors` to see the full directory of available poets, or use `get_random_poems` to have the agent surprise you with a random selection from the database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/poetrydb](https://vinkius.com/mcp/poetrydb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PoetryDB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `poetrydb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PoetryDB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "poetrydb": {
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
