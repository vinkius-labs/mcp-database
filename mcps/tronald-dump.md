# Tronald Dump MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tronald-dump)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming-entertainment](../categories/gaming-entertainment.md)

Access the world's smartest database of Donald Trump quotes. Search by tag, keyword, or get random insights directly in your AI agent.

## Description
Connect to the **Tronald Dump** API to retrieve, search, and categorize quotes from Donald Trump. This MCP server allows your AI agent to interact with a curated database of public statements.

### What you can do

- **Random Quotes** — Fetch a random quote instantly from the database
- **Search & Filter** — Search for specific keywords or filter quotes by tags to find relevant statements
- **Tag Discovery** — List all available categories and tags used in the system to organize the content
- **Specific Retrieval** — Access a specific quote using its unique identifier for precise referencing

### How it works

1. Subscribe to this server
2. No complex API keys are required for basic public access
3. Start querying quotes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Journalists** — quickly find and verify public statements and their context
- **Content Creators** — retrieve quotes for social media or editorial content without manual searching
- **Developers** — integrate a humorous or political quote engine into your AI workflows


## Available Tools (5)
- **get_quote**: Get a specific quote by ID
- **get_quotes_by_tag**: Get quotes associated with a specific tag
- **get_tags**: Get a list of all tags
- **get_random_quote**: Get a random Donald Trump quote
- **search_quotes**: Search for quotes containing specific text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tronald Dump** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a random Donald Trump quote."

**🤖 AI Agent:**
> I've fetched a random quote for you: 'I will build a great wall -- and nobody builds walls better than me, believe me --and I’ll build them very inexpensively.'

---

**👤 You:**
> "Search for quotes containing the word 'China'."

**🤖 AI Agent:**
> Searching the database... I found several quotes mentioning 'China'. One example is: 'We can't continue to allow China to rape our country and that's what they're doing.' Would you like to see more results?

---

**👤 You:**
> "Show me all available tags for these quotes."

**🤖 AI Agent:**
> I've retrieved the tags. You can filter quotes using categories like: 'Hillary Clinton', 'Barack Obama', 'Ted Cruz', 'Money', and 'The Wall'. Which tag would you like to explore?


## ❓ FAQ

**Q: How can I get a random quote from the system?**
Simply use the `get_random_quote` tool. It will fetch a single random entry from the Tronald Dump API and present it to you immediately.

**Q: Can I search for quotes about a specific topic like 'Hillary'?**
Yes! Use the `search_quotes` tool and provide your search term in the query parameter. The agent will return all matching quotes found in the database.

**Q: How do I see what categories or tags are available for filtering?**
You can use the `get_tags` tool to retrieve a complete list of all tags used to categorize quotes in the system. You can then use these with `get_quotes_by_tag`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tronald-dump](https://vinkius.com/mcp/tronald-dump)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tronald Dump** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tronald-dump` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tronald Dump** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tronald-dump": {
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
