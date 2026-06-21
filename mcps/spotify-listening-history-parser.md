# Spotify Listening History Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spotify-listening-history-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Parse your Spotify data export and discover your top artists, tracks, and total listening hours. Turn your AI into your personal music analyst local.

## Description
Spotify lets you request your full listening history via Privacy settings. The result is a massive JSON file with every song you ever played. This MCP aggregates it locally into actionable insights: top 30 artists, top 30 tracks, total hours, and unique counts.

### The Superpowers

- **Smart Aggregation:** Millions of plays → clean top-30 rankings.
- **Total Hours Calculated:** Know exactly how many hours you spent listening.
- **100% Local.** Your music taste stays private.


## Available Tools (1)
- **parse_spotify_history**: The file is usually a JSON array of listening events.

Parse a Spotify listening history JSON export (from Spotify Privacy or Google Takeout) and aggregate top artists, tracks, and total listening hours


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spotify Listening History Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was my most listened artist in 2024?"

**🤖 AI Agent:**
> Your #1 artist was Radiohead with 342 plays, followed by Tame Impala (218) and Daft Punk (195).

---

**👤 You:**
> "How many total hours did I spend on Spotify?"

**🤖 AI Agent:**
> You spent exactly 1,245.3 hours listening to music across 28,400 tracks.

---

**👤 You:**
> "Show my top 5 most played songs of all time."

**🤖 AI Agent:**
> 1. Bohemian Rhapsody — Queen (89 plays)
2. Blinding Lights — The Weeknd (76)
3. Creep — Radiohead (71)


## ❓ FAQ

**Q: How do I get my Spotify data?**
Go to spotify.com/account/privacy. Request your data. Spotify emails you a download link within 30 days.

**Q: Does it work with Apple Music?**
This parser is optimized for Spotify's JSON format. Apple Music exports use a different structure.

**Q: Is my listening data sent to the cloud?**
No. All aggregation happens locally. Only the top-30 lists and totals are sent to the AI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spotify-listening-history-parser](https://vinkius.com/mcp/spotify-listening-history-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spotify Listening History Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spotify-listening-history-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spotify Listening History Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spotify-listening-history-parser": {
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
