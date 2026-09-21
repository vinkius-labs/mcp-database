# Card Collection Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/card-collection-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Track and analyze your collectible card game collections.

## Description
This MCP server provides tools to manage and analyze collectible card game (CCG) collections. You can use `get_total_card_count` to find the absolute sum of all cards owned, `get_unique_card_count` to see how many distinct card identities are in a collection, and `get_collection_composition` to view breakdowns by rarity or set name. Additionally, `get_set_coverage_percentage` helps you track progress toward completing specific sets.

### Available Tools

`getTotalCardCountTool`, `getUniqueCardCountTool`, `getCollectionCompositionTool`, `getSetCoveragePercentageTool`, `getTotalCardCount`, `getUniqueCardCount`, `getCollectionComposition`, `getSetCoveragePercentage`


## Available Tools (4)
- **getUniqueCardCount**: Get the number of unique card identities in a collection
- **getCollectionComposition**: Get the breakdown of cards by rarity or set name
- **getSetCoveragePercentage**: Get the percentage of a specific set owned
- **getTotalCardCount**: Get the total number of cards in a collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Card Collection Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many total cards are in my collection 'user_123'?"

**🤖 AI Agent:**
> You have a total of 452 cards in your collection.

---

**👤 You:**
> "How many unique cards do I own in collection 'user_123'?"

**🤖 AI Agent:**
> You own 124 unique card identities in your collection.

---

**👤 You:**
> "What is my coverage for the 'base_set_01' set in collection 'user_123'?"

**🤖 AI Agent:**
> You have 75% coverage for the 'base_set_01' set.


## ❓ FAQ

**Q: How do I check my total card count?**
You can use the `get_total_card_count` tool by providing your specific collection ID. Tools available: `getTotalCardCountTool`, `getUniqueCardCountTool`, `getCollectionCompositionTool`.

**Q: Can I see how many rare cards I have?**
Yes, use `get_collection_composition` with the grouping type set to 'rarity' to see your breakdown.

**Q: How do I know if I am close to finishing a set?**
Use the `get_set_coverage_percentage` tool with your collection ID and the target set ID to see your completion percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/card-collection-counter](https://vinkius.com/en/ai-agent-connect/card-collection-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Card Collection Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `card-collection-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Card Collection Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "card-collection-counter": {
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
