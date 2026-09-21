# Podcast Season Duration MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/podcast-season-duration)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total playback time and listening estimates for podcast seasons.

## Description
This MCP server provides tools to analyze podcast season durations. Use `get_season_total_duration` to find the total raw playback time, `estimate_listening_time` to calculate how long a season takes at different playback speeds, `get_season_episode_stats` for episode length distributions, and `get_season_metadata` to retrieve season details like release year and episode count.


## Available Tools (4)
- **get_season_episode_stats**: Provides a breakdown of the episode distribution and length within a season
- **get_season_metadata**: Retrieves basic identifying information about a specific season
- **estimate_listening_time**: Calculates how long it will take to finish a season based on a user's preferred playback speed
- **get_season_total_duration**: Calculates the total raw playback time for a specific podcast season


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Podcast Season Duration** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long is the total duration of season 'S1-2023'?"

**🤖 AI Agent:**
> The total duration for season 'S1-2023' is 02:15:30.

---

**👤 You:**
> "If I listen at 1.25x speed, how long will it take to finish season 'pod-99'?"

**🤖 AI Agent:**
> At 1.25x speed, it will take approximately 01:48:00 to finish season 'pod-99'.

---

**👤 You:**
> "Give me the stats for season 'season-abc'."

**🤖 AI Agent:**
> Season 'season-abc' has 10 episodes, with an average duration of 30 minutes, a longest episode of 45 minutes, and a shortest episode of 15 minutes.


## ❓ FAQ

**Q: How do I calculate how long a podcast season will take to listen to?**
You can use the `estimate_listening_time` tool by providing the `seasonId` and your preferred `playbackSpeed` (e.g., 1.5 for 1.5x speed).

**Q: Can I see the length of individual episodes within a season?**
Yes, use `get_season_episode_stats` to get the average, longest, and shortest episode durations for a specific season.

**Q: What information is included in the season metadata?**
The `get_season_metadata` tool returns the season name, the release year, and the total number of episodes in that season.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/podcast-season-duration](https://vinkius.com/en/ai-agent-connect/podcast-season-duration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Podcast Season Duration** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `podcast-season-duration` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Podcast Season Duration** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "podcast-season-duration": {
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
