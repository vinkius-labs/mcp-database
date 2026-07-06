# The Odds API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/the-odds-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal sports betting intelligence — get real-time odds, scores, and sports data via AI.

## Description
Equip your AI agent with real-time sports market intelligence via **The Odds API** MCP server. This integration provides instant access to live odds from dozens of bookmakers across major sports leagues including NFL, NBA, MLB, EPL, and more. Your agent can list all supported sports, retrieve current market odds for specific regions, and check live or historical scores. Whether you are analyzing market trends, tracking your favorite teams, or building a betting advisor, your agent acts as a dedicated sports data analyst through natural conversation.

### What you can do

- **Live Odds Retrieval** — Get real-time odds for upcoming games from multiple bookmakers.
- **Sports Discovery** — List all available sports and leagues supported by the API.
- **Score Tracking** — Check live and recently completed game scores for various sports.
- **Market Comparison** — Compare prices across different bookmakers and regions (US, UK, EU, AU).
- **Historical Auditing** — Summarize and analyze past game results and market movements.

### How it works

1. Subscribe to this server
2. Enter your Odds API Key (get it at the-odds-api.com)
3. Start querying sports data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Enthusiasts** — stay updated with real-time odds and scores for their favorite leagues.
- **Data Analysts** — collect and analyze sports market data for research or modeling.
- **Betting Professionals** — quickly compare odds across multiple bookmakers.
- **App Developers** — integrate dynamic sports data into custom applications.


## Available Tools (3)
- **get_scores**: Get live and past scores
- **list_sports**: List all available sports
- **get_odds**: Get odds for a specific sport


## 💬 Prompt Examples

Here are some examples of how you can interact with the **The Odds API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current odds for the next NFL games."

**🤖 AI Agent:**
> Retrieving NFL odds... I've found several upcoming games. For example, the Chiefs vs Raiders match has odds ranging from 1.45 to 1.55 for a home win across different bookmakers. Would you like to see more markets like spreads or totals?

---

**👤 You:**
> "Check the live scores for the English Premier League."

**🤖 AI Agent:**
> Fetching live scores for soccer_epl... Liverpool is currently leading 2-1 against Chelsea at the 75th minute. Arsenal vs Man City is still 0-0. Would you like to see the stats or current live odds for these matches?

---

**👤 You:**
> "List all sports available on The Odds API."

**🤖 AI Agent:**
> Retrieving the sports list... I've identified over 100 sports and leagues, including American Football (NFL, NCAA), Basketball (NBA, WNBA), Soccer (EPL, La Liga, Serie A), and even eSports. Which one would you like to focus on?


## ❓ FAQ

**Q: Can I get odds for the Premier League?**
Yes! Use the `get_odds` tool with the sport key `soccer_epl`. It will return the latest odds from various bookmakers.

**Q: How do I see results for recently finished games?**
Use the `get_scores` tool and provide the sport key. It will return the scores for live games and those that have recently ended.

**Q: What bookmaker regions are supported?**
The Odds API supports 'us' (United States), 'uk' (United Kingdom), 'eu' (Europe), and 'au' (Australia). Use the `regions` parameter to filter odds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-odds-api](https://vinkius.com/mcp/the-odds-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **The Odds API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `the-odds-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **The Odds API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "the-odds-api": {
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
