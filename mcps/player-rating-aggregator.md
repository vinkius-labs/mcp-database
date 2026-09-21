# Player Rating Aggregator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/player-rating-aggregator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Aggregate football player match ratings using arithmetic, weighted, or minutes-weighted averages.

## Description
This MCP server provides advanced statistical tools for analyzing football player performance. It allows for the calculation of detailed rating profiles using various mathematical methods. Use `get_player_rating_summary` to obtain statistical metrics like average, median, and standard deviation. Analyze performance shifts over time with `get_player_performance_trend`, or retrieve full chronological records using `get_player_match_history`. You can also view rating frequency distributions with `get_player_rating_distribution`.


## Available Tools (4)
- **get_player_match_history**: Retrieves a chronologically sorted list of all match ratings for a player
- **get_player_performance_trend**: Determines if a player's performance is improving, declining, or stable
- **get_player_rating_distribution**: g., how many 8-10s, 6-8s, etc.) for a player.

Provides a breakdown of how frequently specific rating ranges occur
- **get_player_rating_summary**: Calculates a statistical profile of a player's ratings for a specific period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Player Rating Aggregator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a statistical summary of player 'p123' from 2023-01-01 to 2023-12-31 using arithmetic average."

**🤖 AI Agent:**
> For player p123 in 2023, the average rating was 7.2, with a median of 7.0, a minimum of 5.5, a maximum of 8.5, and a standard deviation of 0.8 across 25 matches.

---

**👤 You:**
> "Is player 'p456' performing better or worse lately? Compare Jan 2024 to Dec 2023."

**🤖 AI Agent:**
> Player p456 is improving. The current period average is 7.8 compared to the previous period average of 7.2, showing an upward trend of 0.6.

---

**👤 You:**
> "Show me the match history for player 'p789' for the first half of 2024."

**🤖 AI Agent:**
> Player p789 played 12 matches between 2024-01-01 and 2024-06-30. The ratings ranged from 6.0 to 8.0, with the most recent match on 2024-06-15 resulting in a 7.5.


## ❓ FAQ

**Q: What aggregation methods are supported?**
The server supports arithmetic mean, weighted average (using a custom weight map), and minutes-weighted average which accounts for time played.

**Q: How can I see if a player's form is improving?**
You can use the `get_player_performance_trend` tool to compare the average rating of a current period against a previous one.

**Q: Can I handle matches where no rating was given?**
Yes, you can specify a missing rating policy (ignore or baseline) when calling `get_player_rating_summary`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/player-rating-aggregator](https://vinkius.com/en/ai-agent-connect/player-rating-aggregator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Player Rating Aggregator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `player-rating-aggregator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Player Rating Aggregator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "player-rating-aggregator": {
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
