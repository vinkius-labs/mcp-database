# Podcast Episode Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/podcast-episode-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Count and categorize podcast episodes from datasets.

## Description
This MCP server provides tools to analyze podcast datasets. You can use `list_all_episodes` to find the total number of unique episodes, `count_episodes_by_series` to filter by a specific show, `count_episodes_by_status` to check release states, or `get_episode_summary_stats` for a full distribution overview.


## Available Tools (4)
- **count_episodes_by_status**: g., "released" or "upcoming").

Answers how many episodes are currently released versus those that are upcoming
- **get_episode_summary_stats**: Answers the high-level distribution of episodes across the dataset
- **list_all_episodes**: Answers how many total episodes are available in the provided dataset
- **count_episodes_by_series**: Answers how many episodes belong to a specific podcast series


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Podcast Episode Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many total episodes are in this list?"

**🤖 AI Agent:**
> There are 42 unique episodes in the provided dataset.

---

**👤 You:**
> "How many episodes belong to the 'Daily News' series?"

**🤖 AI Agent:**
> The 'Daily News' series has 12 episodes.

---

**👤 You:**
> "Give me a summary of the episode distribution."

**🤖 AI Agent:**
> The dataset contains 50 episodes total, distributed across 5 series, with 40 released and 10 upcoming.


## ❓ FAQ

**Q: How does the tool handle duplicate episodes?**
The tools use unique identifiers to ensure each episode is only counted once, even if it appears multiple times in the input list.

**Q: Can I filter episodes by their release status?**
Yes, you can use `count_episodes_by_status` to count episodes that are marked as released or upcoming.

**Q: What kind of data does the summary tool provide?**
The `get_episode_summary_stats` tool provides the total unique count, a distribution of episodes by series, and a distribution by status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/podcast-episode-counter](https://vinkius.com/en/ai-agent-connect/podcast-episode-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Podcast Episode Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `podcast-episode-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Podcast Episode Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "podcast-episode-counter": {
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
