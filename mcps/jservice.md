# Jservice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jservice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the Jeopardy! clue database — fetch clues by category, value, or date, and get random trivia for your AI agent.

## Description
Connect to the **Jservice** API and bring the world of Jeopardy! trivia to your AI agent. This server allows you to query thousands of historical clues, explore categories, and generate random trivia challenges directly through natural conversation.

### What you can do

- **Clue Retrieval** — Fetch specific clues filtered by dollar value, category ID, or date ranges using the `get_clues` tool.
- **Random Trivia** — Generate random clues to create quizzes or test general knowledge with `get_random_clues`.
- **Category Exploration** — Browse through the extensive list of Jeopardy! categories and their associated IDs using `get_categories`.
- **Deep Category Inspection** — Retrieve all clues belonging to a specific category for focused study or gaming via `get_category`.

### How it works

1. Subscribe to this server
2. No API key is required as Jservice is a public trivia database
3. Start querying trivia data directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — building trivia apps or testing LLM knowledge retrieval with real-world data
- **Educators** — creating engaging quizzes based on historical Jeopardy! clues
- **Trivia Enthusiasts** — exploring the vast history of the game show through natural conversation


## Available Tools (4)
- **get_categories**: Limited to 100 at a time.

Get a list of categories
- **get_category**: Get a specific category and its associated clues
- **get_clues**: Can be filtered by value, category, date, and offset.

Get a list of clues based on filter criteria
- **get_random_clues**: Limited to 100 at a time.

Get a random set of clues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jservice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me 3 random Jeopardy clues."

**🤖 AI Agent:**
> I've retrieved 3 random clues for you. One is from the 'Science' category: 'This element has the symbol Au'. Would you like the answers as well?

---

**👤 You:**
> "List 10 trivia categories and their IDs."

**🤖 AI Agent:**
> Here are 10 categories from the database: 1. Publications (ID: 12), 2. Sports (ID: 42), 3. Potent Potables (ID: 67)... Which one would you like to explore?

---

**👤 You:**
> "Find clues worth $1000 in category 42."

**🤖 AI Agent:**
> Searching for high-value clues in category 42 (Sports)... I found 2 clues worth $1000. One is about a famous 1920s baseball player. Should I reveal the clue text?


## ❓ FAQ

**Q: Can I get multiple random clues at once?**
Yes! Use the `get_random_clues` tool and specify the `count` parameter (up to 100) to receive a batch of random trivia questions.

**Q: How do I find clues from a specific category ID?**
You can use `get_category` with the specific ID to get all clues in that category, or use `get_clues` and filter by the `category` parameter.

**Q: Is it possible to filter clues by their difficulty or dollar value?**
Yes, the `get_clues` tool accepts a `value` parameter (e.g., 200, 400, 800) to help you find clues corresponding to specific Jeopardy! board positions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jservice](https://vinkius.com/mcp/jservice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jservice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jservice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jservice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jservice": {
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
