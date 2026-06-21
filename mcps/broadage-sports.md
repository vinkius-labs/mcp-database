# Broadage Sports MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/broadage-sports)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time sports data via Broadage — track scores, matches, and lineups directly from any AI agent.

## Description
Connect your **Broadage Sports** account to any AI agent and orchestrate your sports research, live score tracking, and match analysis workflows through natural conversation.

### What you can do

- **Live Score Monitoring** — List soccer matches currently in progress and retrieve real-time score updates.
- **Match Analysis** — Get detailed summaries, statistics (possession, shots), and event timelines (goals, cards) for any match.
- **Lineup Coordination** — Retrieve starting XI and substitute information for upcoming matches to analyze team strategy.
- **Schedule Oversight** — List matches by date to plan your coverage or monitor specific tournaments.
- **Tournament Discovery** — Access the directory of all supported sports, tournaments, and match statuses.
- **Player Intelligence** — List players for specific teams to retrieve roster details.

### How it works

1. Subscribe to this server
2. Enter your Broadage API Subscription Key and Language ID
3. Start tracking the world of sports from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Journalists & Content Creators** — quickly retrieve match stats and lineups for live reporting without manual data entry.
- **Betting Analysts** — monitor real-time scores and statistics straight from their workflow tools.
- **Die-hard Fans** — check live scores and player info using natural language.


## Available Tools
- **get_match_events**: Get timeline of match events (goals, cards)
- **get_match_lineup**: Get starting lineups and substitutes for a match
- **get_match_stats**: Get detailed match statistics (possession, shots)
- **get_match_summary**: Get summary and score for a specific match
- **list_live_matches**: List soccer matches currently in progress
- **list_matches_by_date**: List soccer matches for a specific date (YYYY-MM-DD)
- **list_team_players**: List players for a specific team
- **list_sports**: List all supported sports
- **list_match_statuses**: List possible match status definitions
- **list_tournaments**: List all available sports tournaments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Broadage Sports** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show the live soccer scores for today."

**🤖 AI Agent:**
> I've checked the live matches. Currently, Arsenal is leading 2-1 against Chelsea (75'), and Real Madrid is drawing 0-0 with Barcelona (20').

---

**👤 You:**
> "What's the starting lineup for the match with ID 12345?"

**🤖 AI Agent:**
> Retrieving lineup for match 12345... Team A is playing a 4-3-3 formation with Smith in goal. Team B is using a 4-4-2. Would you like the list of substitutes?

---

**👤 You:**
> "Show match statistics for match 12345."

**🤖 AI Agent:**
> Retrieving stats for match 12345... Possession is 55% for Team A, they have 12 shots total (5 on target), and 6 corners. Team B has 45% possession.


## ❓ FAQ

**Q: Can I check the live score of an ongoing match?**
Yes! Use the `list_live_matches` tool. Your agent will fetch all soccer matches currently in progress along with their real-time scores.

**Q: How early are match lineups available?**
Match lineups are typically available 45 to 60 minutes before kickoff. Use the `get_match_lineup` tool with the specific Match ID to retrieve them.

**Q: Does the integration support sports other than soccer?**
While the current toolset is optimized for soccer (football) match data, the Broadage API supports many sports. Use the `list_sports` tool to see all available sports in your subscription.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/broadage-sports](https://vinkius.com/mcp/broadage-sports)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Broadage Sports** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `broadage-sports` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Broadage Sports** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "broadage-sports": {
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
