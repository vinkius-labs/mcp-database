# TheRundown MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/therundown)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time sports data, betting odds, and schedules for NFL, NBA, MLB, and more directly from your AI agent.

## Description
Connect **TheRundown** to any AI agent to retrieve the most accurate real-time sports information. Whether you are tracking live scores, analyzing betting markets, or checking upcoming schedules, this server provides professional-grade sports data through natural conversation.

### What you can do

- **Sport Discovery** — List all supported sports and their unique IDs (NFL, NBA, MLB, NHL, etc.) to target your queries.
- **Live Events & Scores** — Fetch real-time events by sport and date, including scores and period-by-period breakdowns.
- **Market Odds** — Retrieve the latest betting odds from multiple sportsbooks for any specific game or event.
- **Schedules** — Access upcoming game schedules for specific sports to stay ahead of the season.
- **Deep Event Inspection** — Get detailed metadata for a specific event using its unique identifier.

### How it works

1. Subscribe to this server
2. Enter your TheRundown API Key
3. Start querying sports data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Analysts** — Quickly pull historical and real-time data for performance modeling and reporting.
- **Betting Enthusiasts** — Compare odds across different sportsbooks and track line movements instantly.
- **Developers** — Integrate sports data into your workflow or build sports-aware AI assistants without leaving your IDE.


## Available Tools
- **get_event_odds**: Retrieve the latest odds for a specific event
- **get_event**: Retrieve detailed information for a specific event
- **list_events_by_sport**: You can optionally include scores or all_periods.

Retrieve events for a specific sport on a given date
- **get_sport_schedule**: Retrieve the schedule for a specific sport
- **list_sports**: g., NFL=2, NBA=4).

Retrieve a list of supported sports and their corresponding IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheRundown** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available sports and their IDs from TheRundown."

**🤖 AI Agent:**
> I've retrieved the supported sports. Some key IDs include: NFL (2), NBA (4), MLB (3), and NHL (6). Which league would you like to explore?

---

**👤 You:**
> "Show me the NFL games scheduled for 2024-11-10."

**🤖 AI Agent:**
> Searching for NFL events on that date... I found several matchups, including 'Philadelphia Eagles vs. Dallas Cowboys' and 'Detroit Lions vs. Houston Texans'. Would you like the betting odds for any of these?

---

**👤 You:**
> "Get the latest odds for event ID 492031."

**🤖 AI Agent:**
> Fetching odds for event 492031... For this matchup, the Spread is currently -3.5 for the home team at Pinnacle and -3.0 at DraftKings. The Total is set at 48.5 points.


## ❓ FAQ

**Q: How do I find the correct ID for a specific sport like NFL or NBA?**
Use the `list_sports` tool. It will return a complete list of all supported sports along with their corresponding IDs (e.g., NFL is 2, NBA is 4).

**Q: Can I see the betting odds from different sportsbooks for a single game?**
Yes! By using the `get_event_odds` tool with a specific event ID, the agent will fetch the latest lines and odds from various available sportsbooks.

**Q: How can I check the upcoming schedule for a specific league?**
You can use the `get_sport_schedule` tool. Just provide the sport ID, and it will return the upcoming games and events scheduled for that sport.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/therundown](https://vinkius.com/mcp/therundown)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TheRundown** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `therundown` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TheRundown** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "therundown": {
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
