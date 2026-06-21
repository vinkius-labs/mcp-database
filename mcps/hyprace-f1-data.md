# Hyprace F1 Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hyprace-f1-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hyprace-f1-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hyprace-f1-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query Formula 1 race results, driver standings, constructor rankings, and historical data since 1950 from any AI agent.

## Description
Connect your AI agent to the most trusted Formula 1 data source available. **Hyprace** delivers deep insights into every F1 season since 1950, with results published within minutes of the chequered flag during active race weekends.

### What you can do

- **Grands Prix & Schedules** — List upcoming events, browse the full season calendar, and retrieve metadata for any historical Grand Prix
- **Session Results** — Fetch qualifying classifications and race results including positions, gaps, fastest laps, and retirement reasons
- **Championship Standings** — Track Driver and Constructor rankings updated after every round throughout the season
- **Driver & Team Profiles** — Access career statistics, podium counts, pole positions, and detailed performance histories
- **Circuit Intelligence** — Inspect track details, locations, lap records, and historical race winners at each venue
- **Technical Archives** — Browse engine manufacturers, chassis builders, and the complete technical lineage of the sport

### How it works

1. Subscribe to this server
2. Enter your **RapidAPI Key** from the [Hyprace API page on RapidAPI](https://rapidapi.com/hyprace-hyprace-default/api/hyprace-api)
3. Start querying F1 data from Claude, Cursor, or any MCP-compatible client

Whether you are settling a debate about Senna vs. Schumacher or tracking the latest championship battle, Hyprace delivers the precision required for elite motorsport intelligence.

### Who is this for?

- **F1 Enthusiasts** — stay updated with live results and standings without leaving your conversation
- **Data Analysts & Researchers** — retrieve structured historical data for performance modeling and trend analysis
- **Content Creators & Journalists** — quickly pull verified stats and facts for race previews and reviews


## Available Tools
- **get_driver**: Get detailed information for a specific F1 driver
- **get_grand_prix**: Get detailed information for a specific Grand Prix event
- **get_qualifying_results**: Retrieve Formula 1 qualifying session results
- **get_race_results**: Retrieve Formula 1 race session results
- **get_standings**: Retrieve Formula 1 championship standings
- **get_team**: Get detailed information for a specific F1 team
- **list_circuits**: List all Formula 1 tracks and circuits
- **list_drivers**: List Formula 1 drivers
- **list_engine_manufacturers**: List all F1 engine builders and providers
- **list_grands_prix**: List Formula 1 Grands Prix events and schedules
- **list_seasons**: List all available Formula 1 seasons (1950–Present)
- **list_teams**: List Formula 1 teams (constructors)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hyprace F1 Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the race results for the 2024 Monaco Grand Prix."

**🤖 AI Agent:**
> Fetching the Monaco GP results... The winner was Charles Leclerc (Ferrari) with a dominant lights-to-flag victory, followed by Oscar Piastri (McLaren) in P2 and Carlos Sainz (Ferrari) in P3. Max Verstappen finished P6 after struggling with tyre degradation. Would you like to see the full classification or the qualifying grid?

---

**👤 You:**
> "What are the current driver standings for the 2025 season?"

**🤖 AI Agent:**
> Here are the 2025 Driver Standings after Round 5: 1. Max Verstappen (Red Bull) — 110 pts, 2. Lando Norris (McLaren) — 98 pts, 3. Charles Leclerc (Ferrari) — 87 pts, 4. Oscar Piastri (McLaren) — 76 pts. The gap at the top is 12 points. Would you like to see the Constructor standings as well?

---

**👤 You:**
> "Tell me about Ayrton Senna's career stats."

**🤖 AI Agent:**
> Retrieving driver profile... Ayrton Senna (Brazil, 1960–1994): 3× World Champion (1988, 1990, 1991), 161 race starts, 41 victories, 80 podiums, 65 pole positions, and 19 fastest laps. He raced for Toleman, Lotus, McLaren, and Williams across 11 seasons. Would you like to see his season-by-season results or compare him with another legendary driver?


## Installation & Usage

To install and use the **Hyprace F1 Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hyprace-f1-data](https://vinkius.com/mcp/hyprace-f1-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
