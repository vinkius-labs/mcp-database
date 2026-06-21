# TheSportsDB Global Sports Database MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thesportsdb-global-sports-database)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/thesportsdb-global-sports-database-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/thesportsdb-global-sports-database-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

The definitive sports metadata server — search teams, players, leagues, and live results via AI.

## Description
Equip your AI agent with the most comprehensive sports intelligence available via **TheSportsDB**. This unified server merges all aspects of sporting data into a single, high-performance interface. Your agent can instantly find detailed profiles for professional teams and athletes, retrieve official league standings, monitor upcoming match schedules, and audit historical career achievements. Whether you are conducting deep biographical research or tracking live seasonal performance, your agent acts as a dedicated global sports scout and historian through natural conversation.

### What you can do

- **Discovery & Profiling** — Search for thousands of professional teams and players to retrieve histories, badges, and biographies
- **League Intelligence** — Query official standings, league tables, and member club lists for hundreds of global competitions
- **Real-time Monitoring** — Fetch upcoming match schedules and recent results with scores for specific teams or dates
- **Career Analysis** — Audit player trophy cabinets (honours), transfer histories, and professional milestones

### How it works

1. Subscribe to this server
2. Enter your TheSportsDB API Key (use '3' for testing)
3. Start managing your sports intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Analysts** — instantly retrieve team histories and player performance metrics for deep reporting
- **Fantasy League Managers** — check team rankings and player stats directly from your workflow
- **Content Creators** — automate the retrieval of high-quality team badges and player artwork for media production


## Available Tools
- **list_events_by_day**: List all sports events for a specific date
- **list_last_events_by_team**: List recent match results for a specific team
- **list_next_events_by_team**: List upcoming matches for a specific team
- **list_events_by_season**: List all events in a league for a specific season
- **list_all_leagues**: List all available leagues
- **get_league_details**: Get metadata for a specific league by ID
- **get_league_table**: Get current standings for a league and season
- **list_all_teams_in_league**: List all teams belonging to a specific league
- **list_player_contracts**: Get contract details for a player
- **list_player_honours**: List trophies and awards for a player
- **list_player_milestones**: List career milestones for a player
- **list_former_teams**: List previous clubs for a player
- **list_all_sports**: List all available sports
- **search_events**: Search for sports events by name
- **search_players**: Search for sports players by name
- **search_teams**: Search for sports teams by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheSportsDB Global Sports Database** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the professional profile of 'Lionel Messi'."

**🤖 AI Agent:**
> I've fetched Messi's profile. He is a forward for Inter Miami CF (ID: 34145937). I have his detailed bio, height, weight, and official social media links. Would you like to see his career honours cabinet?

---

**👤 You:**
> "Show me the current standings table for the NBA season 2023-2024."

**🤖 AI Agent:**
> Running the standings query... I've retrieved the full NBA table. Notable leaders include the Boston Celtics in the East and OKC Thunder in the West. Would you like the specific points and win/loss records for a particular team?

---

**👤 You:**
> "What are the next 5 matches scheduled for 'Arsenal'?"

**🤖 AI Agent:**
> Inspecting the calendar... Arsenal has 5 upcoming fixtures. The next match is against Everton at the Emirates Stadium. I also found matches against Brighton and Bournemouth. Would you like the precise start times?


## Installation & Usage

To install and use the **TheSportsDB Global Sports Database** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thesportsdb-global-sports-database](https://vinkius.com/mcp/thesportsdb-global-sports-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
