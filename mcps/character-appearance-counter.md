# Character Appearance Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/character-appearance-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [text-processing](../categories/text-processing.md)

Track character presence across chapters with precise name variant counting.

## Description
This MCP server provides tools for literary analysis by counting how many times specific characters appear in text. It handles multiple name variants (e.g., 'Sherlock' and 'Holmes') as a single entity to ensure accuracy. Use `get_chapter_counts` to analyze specific chapters, `get_aggregate_totals` for book-wide sums, `get_chapter_summary` for a full breakdown, and `verify_name_integrity` to clean your character lists.


## Available Tools (4)
- **get_chapter_summary**: Provides a breakdown of character presence across chapters
- **get_aggregate_totals**: Calculates the total occurrences across all chapters
- **get_chapter_counts**: Counts character name occurrences in a specific chapter
- **verify_name_integrity**: Validates if the provided name variants are suitable for processing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Character Appearance Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many times does Sherlock Holmes appear in this chapter text: 'Sherlock walked into the room. Holmes looked around.'?"

**🤖 AI Agent:**
> Sherlock Holmes appears 2 times in this chapter.

---

**👤 You:**
> "Give me a summary of character presence for these chapter counts: [{'chapterId': '1', 'count': 5}, {'chapterId': '2', 'count': 3}]"

**🤖 AI Agent:**
> Chapter 1: 5 appearances, Chapter 2: 3 appearances. Total: 8 appearances.

---

**👤 You:**
> "What is the total count for these chapter counts: [10, 20, 15]?"

**🤖 AI Agent:**
> The total count is 45.


## ❓ FAQ

**Q: How does the tool handle different names for the same character?**
You can provide a list of name variants using `get_chapter_counts`. The tool will sum the occurrences of all provided variants to give you a single total for that character.

**Q: Can I get a summary of character presence across the whole book?**
Yes, use `get_chapter_summary` to receive a detailed breakdown of counts per chapter and the overall total.

**Q: What should I do if my character names have extra spaces?**
You can use `verify_name_integrity` to validate and sanitize your list of name variants before performing counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/character-appearance-counter](https://vinkius.com/en/ai-agent-connect/character-appearance-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Character Appearance Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `character-appearance-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Character Appearance Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "character-appearance-counter": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
