# HowLongToBeat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/howlongtobeat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Universal game completion data — get gameplay hours for any video game via AI.

## Description
Equip your AI agent with the ultimate gaming library intelligence via the **HowLongToBeat** MCP server. This integration provides instant access to the world's most trusted source for game completion times. Your agent can search for any video game and retrieve precise timing data for the 'Main Story', 'Main + Extra', and 'Completionist' runs. Whether you're planning your backlog, deciding on your next purchase, or auditing your play style, your agent acts as a dedicated gaming advisor through natural conversation.

### What you can do

- **Game Time Search** — Find how long it takes to beat any video game.
- **Playstyle Comparison** — Compare durations for different completion levels (story vs. 100%).
- **Release Intelligence** — Retrieve world release dates and exact game titles for thousands of entries.
- **Backlog Auditing** — Summarize expected playtimes for entire lists of games.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying game times from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gamers** — planning their playtime and managing their ever-growing backlogs.
- **Content Creators** — seeking duration data for reviews and game guides.
- **Data Analysts** — researching trends in game length and player engagement across different eras.
- **Game Journalists** — verify official versus community-reported gameplay durations.


## Available Tools
- **search_game_times**: Search for game completion times


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HowLongToBeat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long does it take to beat the main story of The Witcher 3?"

**🤖 AI Agent:**
> Searching for The Witcher 3: Wild Hunt... The main story takes approximately 52 hours to complete. If you decide to do the side quests as well, it goes up to about 103 hours.

---

**👤 You:**
> "Is 'Hades' a short game for a completionist?"

**🤖 AI Agent:**
> Analyzing Hades completion data... While the main story can be beaten in about 23 hours, a full 'Completionist' run typically takes around 98 hours. It's quite a deep experience if you're aiming for everything.

---

**👤 You:**
> "Compare the completion times for 'Skyrim' and 'Starfield'."

**🤖 AI Agent:**
> Comparing Bethesda titles... Skyrim's main story takes about 34 hours, while Starfield's is slightly shorter at 23 hours. However, for a full 100% run, Skyrim takes around 232 hours compared to Starfield's 154 hours.


## ❓ FAQ

**Q: Can I find out how long 'Elden Ring' takes to 100%?**
Yes! Use the `search_game_times` tool with the query 'Elden Ring'. It will return the average hours for different playstyles, including the 'Completionist' run which is usually over 130 hours.

**Q: Where does the data come from?**
The data is crowdsourced from thousands of gamers worldwide who submit their actual completion times to the HowLongToBeat community platform.

**Q: What is the difference between 'Main + Extra' and 'Completionist'?**
'Main + Extra' includes the story plus some side content, while 'Completionist' represents finishing everything the game has to offer (100% trophies/achievements).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/howlongtobeat](https://vinkius.com/mcp/howlongtobeat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HowLongToBeat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `howlongtobeat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HowLongToBeat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "howlongtobeat": {
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
