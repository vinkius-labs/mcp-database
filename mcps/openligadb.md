# OpenLigaDB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openligadb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage football results — audit match data, standings, and leagues via AI.

## Description
Empower your AI agent to orchestrate your entire football intelligence workflow with **OpenLigaDB**, the community-driven platform for sports results. By connecting OpenLigaDB to your agent, you transform complex match tracking into a natural conversation. Your agent can instantly retrieve match results for dozens of leagues, audit current standing tables, and query upcoming fixtures without you ever touching a sports app. Whether you are building a sports blog or monitoring your favorite team, your agent acts as a real-time sports analyst, ensuring your football data is always current and detailed.

### What you can do

- **Match Auditing** — Query full match results for any supported league and season to maintain a clear view of historical performance.
- **Table Oversight** — Retrieve real-time standing tables to understand league positions and point distributions instantly.
- **Fixture Discovery** — Query upcoming and most recent matches for any league to maintain strict control over event schedules.
- **Match Intelligence** — Retrieve detailed metadata for specific match IDs, including scores and goal details.
- **League Discovery** — List all available leagues in the OpenLigaDB catalog to identify regional event markers.

### How it works

1. Subscribe to this server
2. No API Key required (OpenLigaDB is a public and free service)
3. Start managing your football intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Bloggers** — monitor match results and retrieve table metadata straight from your workflow.
- **Football Enthusiasts** — verify upcoming fixtures and audit recent scores through natural language.
- **Data Analysts** — perform rapid audits of team performance trends without manual database exports.
- **Operations Leads** — automate sports data querying to orchestrate cross-functional content teams smoothly.


## Available Tools (6)
- **get_last_league_match**: Get information about the most recent match in a league
- **get_league_matches**: Get all matches for a specific league and season
- **get_match_details**: Get full details for a specific match ID
- **get_next_league_match**: Get information about the next match in a league
- **get_league_table**: Get the current standing table for a league and season
- **list_available_leagues**: List all available leagues in the OpenLigaDB catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenLigaDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show results for Bundesliga 1 (bl1) season 2023 using OpenLigaDB."

**🤖 AI Agent:**
> I've retrieved the match results for Bundesliga 1. Notable scores include Bayern Munich vs Dortmund. Would you like the standing table for this season as well?

---

**👤 You:**
> "What is the next match in 'bl1'?"

**🤖 AI Agent:**
> The next match in Bundesliga 1 is identified. It features Leverkusen vs Stuttgart scheduled for this weekend. Would you like the venue details or past results for these teams?

---

**👤 You:**
> "List all available leagues in OpenLigaDB."

**🤖 AI Agent:**
> I've scanned the catalog. Available leagues include Bundesliga 1 (bl1), Bundesliga 2 (bl2), and various international cups. I can provide the shortcuts for any of these to retrieve more data.


## ❓ FAQ

**Q: Is an API Key required for OpenLigaDB?**
No. OpenLigaDB is a public and community-driven service. This server works out of the box without any static credentials required.

**Q: What leagues are supported?**
OpenLigaDB primarily covers German football (Bundesliga), but also supports many other international leagues. Use the `list_available_leagues` tool to see the full list.

**Q: Can the agent show the next match for a team?**
Yes. Use the `get_next_league_match` tool providing the league shortcut. Your agent will identify the next upcoming event in that league instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openligadb](https://vinkius.com/mcp/openligadb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenLigaDB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openligadb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenLigaDB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openligadb": {
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
