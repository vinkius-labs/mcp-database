# Start.gg MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/startgg)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Manage esports tournaments via Start.gg — fetch event IDs, track standings, and report match results directly from any AI agent.

## Description
Connect your **Start.gg** developer account to any AI agent and take full control of your esports tournament workflows through natural conversation.

### What you can do

- **Event Discovery** — Retrieve unique Event IDs using slugs from tournament URLs to target specific competitions.
- **Standings & Placements** — Fetch real-time standings and top placements for any active or completed event.
- **Match Tracking** — Query sets (matches) for specific events to monitor bracket progress and results.
- **Geographic Search** — Filter and find tournaments based on country codes to discover local or regional scenes.
- **Tournament Administration** — Report set winners and update phase seeding directly (requires admin permissions).

### How it works

1. Subscribe to this server
2. Enter your Start.gg Personal Access Token
3. Start managing brackets and checking standings from Claude, Cursor, or any MCP-compatible client

No more manual searching through tournament pages to find specific match IDs or standings. Your AI acts as a dedicated tournament coordinator.

### Who is this for?

- **Tournament Organizers** — quickly report match results and update seeding without navigating the full admin dashboard.
- **Esports Analysts** — fetch standings and match data instantly for reporting or data analysis.
- **Competitive Players** — check upcoming sets and current standings directly from their workspace.


## Available Tools
- **get_event_sets**: Get Sets in Event
- **get_event_standings**: Get Event Standings
- **get_event_id**: Get Event ID by Slug
- **report_set**: Requires admin permissions.

Report Set
- **get_tournaments_by_country**: Get Tournaments by Location
- **update_phase_seeding**: Update Phase Seeding


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Start.gg** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the event ID for the slug 'tournament/genesis-9-1/event/ultimate-singles'."

**🤖 AI Agent:**
> I've found the event ID. For the Genesis 9 Ultimate Singles event, the ID is 783210. You can use this ID to fetch standings or match sets.

---

**👤 You:**
> "Show me the top standings for event ID 783210."

**🤖 AI Agent:**
> Fetching standings... Here are the top placements: 1st: MkLeo, 2nd: Sparg0, 3rd: Tweek. Would you like to see more results or specific match details?

---

**👤 You:**
> "List the latest tournaments happening in the US."

**🤖 AI Agent:**
> I've found several active tournaments in the US, including 'Super Smash Con' and 'The Big House'. Which one would you like to explore further?


## ❓ FAQ

**Q: How do I find the Event ID for a specific tournament?**
Use the `get_event_id` tool by providing the slug from the tournament URL (e.g., 'tournament/genesis-9-1/event/ultimate-singles'). The agent will return the unique numeric ID needed for other tools.

**Q: Can I report match results if I am a tournament administrator?**
Yes! If your token has admin permissions, you can use the `report_set` tool with the Set ID and Winner ID to update the bracket results directly.

**Q: How can I see which tournaments are happening in my country?**
Use the `get_tournaments_by_country` tool with your country code (e.g., 'US' or 'BR'). You can also specify how many results you want to see per page.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/startgg](https://vinkius.com/mcp/startgg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Start.gg** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `startgg` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Start.gg** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startgg": {
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
