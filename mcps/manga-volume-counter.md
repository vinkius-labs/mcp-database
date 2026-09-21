# Manga Volume Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/manga-volume-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and manage volume counts for your manga collections.

## Description
This MCP server provides tools to manage and analyze manga collections. You can use `get_collection_summary` to see the total volume count and series count for a specific collection, or `list_series_in_collection` to see every series within it. For deep dives, `get_series_details` provides the exact volume count and completion status of a single series. You can also use `calculate_collection_gap` to determine how many more volumes are needed to reach a specific target for your collection.


## Available Tools (4)
- **calculate_collection_gap**: Determines how many more volumes are needed to reach a target count for a collection
- **get_collection_summary**: Provides a high-level overview of a specific collection's size
- **get_series_details**: Retrieves exhaustive information about a single manga series
- **list_series_in_collection**: Answers which specific manga series are part of a given collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Manga Volume Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total volume count for collection 'my-manga-shelf'?"

**🤖 AI Agent:**
> The collection 'my-manga-shelf' contains a total of 142 volumes across 12 series.

---

**👤 You:**
> "List all the series in the 'summer-reading' collection."

**🤖 AI Agent:**
> The 'summer-reading' collection includes: One Piece (105 volumes), Naruto (72 volumes), and Bleach (74 volumes).

---

**👤 You:**
> "How many more volumes do I need to reach 200 volumes in my 'collector-set'?"

**🤖 AI Agent:**
> You currently have 185 volumes in 'collector-set', so you need 15 more volumes to reach your target of 200.


## ❓ FAQ

**Q: How do I see the total number of volumes in my collection?**
You can use the `get_collection_summary` tool to get the total volume count and the number of series in a specific collection.

**Q: Can I check if a specific manga series is finished?**
Yes, the `get_series_details` tool returns the completion status for any given series.

**Q: How many more volumes do I need to reach my goal?**
Use the `calculate_collection_gap` tool by providing the collection ID and your target volume count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/manga-volume-counter](https://vinkius.com/en/ai-agent-connect/manga-volume-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Manga Volume Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `manga-volume-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Manga Volume Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "manga-volume-counter": {
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
