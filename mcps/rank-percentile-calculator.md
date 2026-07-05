# Rank Percentile Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rank-percentile-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Discover exactly what percentage of players you've surpassed in games like Valorant, League of Legends, and CS2.

## Description
The Rank Percentile Calculator connects AI agents to precise player distribution data for major competitive titles. Using tools like `get_rank_percentile`, you can determine your exact standing in the player base, or use `calculate_next_rank_gap` to see how much of the population you need to overtake to reach your next tier. It provides accurate, patch-specific metrics for games including Valorant, League of Legends, CS2, Apex Legends, and Dota 2.


## Available Tools (4)
- **calculate_next_rank_gap**: How much more progress do I need to reach the next rank?
- **get_game_metadata**: How current is this ranking data?
- **get_rank_percentile**: What percentage of players are at my rank or higher?
- **list_supported_ranks**: What ranks and games can I query?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rank Percentile Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What percentage of players are in the Radiant rank in Valorant?"

**🤖 AI Agent:**
> Players in the Radiant rank represent the top 0.01% of the total player population.

---

**👤 You:**
> "How much more progress do I need to reach Gold from Silver in League of Legends?"

**🤖 AI Agent:**
> To reach Gold, you need to surpass approximately 15% more of the player base.

---

**👤 You:**
> "Check if my ranking data for CS2 is up to date."

**🤖 AI Agent:**
> The current distribution data for CS2 is based on patch v7.34, last updated on October 12, 2023.


## ❓ FAQ

**Q: How accurate is the percentile data?**
The data is based on official distribution tables for each game. However, since player populations shift with every patch, always check `get_game_metadata` to ensure you are looking at the correct version.

**Q: Can I see which games are supported?**
Yes, you can use the `list_supported_ranks` tool to get a complete list of all currently supported games and their respective rank hierarchies.

**Q: How do I know how much progress I need for the next rank?**
Use the `calculate_next_rank_gap` tool. It will tell you exactly what percentage of the player base you need to surpass to reach your target tier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rank-percentile-calculator](https://vinkius.com/mcp/rank-percentile-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rank Percentile Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rank-percentile-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rank Percentile Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rank-percentile-calculator": {
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
