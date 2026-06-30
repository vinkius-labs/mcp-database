# B5 Arena MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/b5-arena)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate Counter-Strike intelligence via B5 Arena — scan matchmaking leaderboards, track player ELO, and fetch competitive match logs natively from any AI agent.

## Description
Infuse the premier competitive matchmaking stats of **B5 Arena** into your AI toolkit. Run heavy analytical queries to monitor team rosters, verify individual player skill performance, and extract post-game data sets instantly through natural chat commands.

### What you can do

- **Player Profiles** — Download extensive KD statistics, accuracy percentages, and win/loss records mapping directly to player aliases seamlessly
- **Match Reports** — Unpack highly granular details around recent competitive series fetching individual scorings without opening heavy demo files
- **Rank Tracking** — Scan the ELO tiers aggregating thousands of user points into a simple leaderboard markdown table instantly

### How it works

1. Subscribe to the server
2. Create an API Key in the [B5 Developer Portal](https://b5csgo.com.cn/)
3. Inject the key here to bridge Claude or Cursor to the esports matrix

### Who is this for?

- **Esports Analysts** — compare team mechanics and extract precise K/D fluctuations ahead of official tournaments directly via script
- **Clan Managers** — monitor clan health actively tracking the recent match progression of internal members simultaneously
- **Community Organizers** — filter out potential smurf accounts querying historical data depth ensuring fair matchmaking globally


## Available Tools (10)
- **get_server_status**: Check B5 server node health and network
- **get_team_info**: Lookup an amateur or semi-pro 5-stack roster
- **get_user_data**: Get a players overall B5 Account summary
- **search_user**: Search the B5 player directory
- **get_ban_list**: Fetch the global recent anti-cheat ban feed
- **get_clutch_highlights**: Extract auto-generated highlight timestamps
- **get_event_list**: Retrieve active promotional events or drops
- **get_match_scoreboard**: Extract detailed match telemetry for a B5 pug
- **get_ranking_list**: Query the active B5 leaderboards/divisions
- **get_recent_matches**: Get a list of recent matches in the B5 hub


## 💬 Prompt Examples

Here are some examples of how you can interact with the **B5 Arena** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize user 'kennys_fan' combat performance spanning their last recorded session natively."

**🤖 AI Agent:**
> I've mapped out 'kennys_fan'. He pulled a solid 1.25 KD ratio across his last 15 maps predominantly locked onto AWP duties holding a 62% win percentage. Do you want the map-by-map extraction formatted clearly?

---

**👤 You:**
> "Chart the current regional top 5 hierarchy dominating the ladder."

**🤖 AI Agent:**
> Fetching regional nodes... Pinned the top 5 ELO holders! ID 'Wargod44' takes rank #1 sitting on 3020 points securely. 'Blade_Edge' trails at 2950 tightly. I can present the comprehensive markdown tabular breakdown showcasing win streaks alongside immediately?

---

**👤 You:**
> "Check match 992-abc logs to identify the lowest performing node pulling the team down natively."

**🤖 AI Agent:**
> Parsing logs for 992-abc... The weakest link resolves strictly pointing to 'User_Echo', pulling a meager 0.44 ratio closing down with only 5 secure frags across 24 intense rounds played globally there. Providing structural JSON export for extended penalty tracking.


## ❓ FAQ

**Q: Can my AI pull exhaustive match histories avoiding manual browser checks on specific dates?**
Yes! Utilize the `get_user_matches` tool providing the B5 Identity. Your engine will dynamically assemble their 20 latest scorelines fetching K/D performance strictly tabulated avoiding bloated HTML arrays altogether.

**Q: How do I fetch the active rank node indexing the top competitive ladder without lag?**
Direct your agent to use `get_b5_leaderboard`. The backend will isolate the primary ELO structure bypassing typical heavy website loading sequences and generate markdown ranks purely focused on point values quickly.

**Q: Are there vulnerabilities enabling irreversible edits like ranking manipulation from within this scope?**
No. The architecture provides rigid read-only isolation boundaries securing the data pool ensuring zero write permissions block any attempt at destructive data corruption natively securely all times seamlessly executing perfectly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/b5-arena](https://vinkius.com/mcp/b5-arena)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **B5 Arena** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `b5-arena` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **B5 Arena** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "b5-arena": {
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
