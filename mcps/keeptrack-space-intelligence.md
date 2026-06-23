# KeepTrack Space Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keeptrack-space-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal space intelligence — search satellites, orbital debris, and launches via AI.

## Description
Equip your AI agent with real-time orbital intelligence through the **KeepTrack** MCP server. This integration provides instant access to a massive database of satellites, space debris, and other objects orbiting the Earth. Your agent can search for satellites by name, retrieve detailed metadata (including NORAD IDs, country of origin, and launch dates), and monitor the most recent objects launched into space. Whether you are conducting aerospace research, tracking telecommunications assets, or exploring orbital mechanics, your agent acts as a dedicated space operations analyst through natural conversation.

### What you can do

- **Satellite Search** — Find satellites and orbital objects by name or keyword.
- **Metadata Retrieval** — Access exhaustive info including NORAD IDs, orbit types, and country data.
- **Launch Monitoring** — Retrieve a list of the most recent objects deployed into orbit.
- **Orbital Auditing** — Track specific satellite constellations like Starlink or GPS.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying orbital data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Aerospace Engineers & Researchers** — quickly verify satellite records and orbital status.
- **Astronomy Enthusiasts** — identify objects passing overhead and research space history.
- **Telecommunications Analysts** — track commercial and government satellite assets.
- **Data Scientists** — access a reliable source of structured orbital metadata.


## Available Tools (3)
- **get_recent_space_launches**: Get most recent space launches
- **get_satellite_details**: Get details for a specific satellite
- **search_satellites**: Search for satellites by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KeepTrack Space Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for satellites named 'Starlink'."

**🤖 AI Agent:**
> Searching the KeepTrack database... I've found a large list of Starlink satellites. Would you like to see the NORAD IDs for the most recent ones or specific orbital data for one of them?


## ❓ FAQ

**Q: Can I find the International Space Station (ISS)?**
Yes! Use the `search_satellites` tool with the query 'ISS'. The response will include its latest NORAD ID and orbital details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keeptrack-space-intelligence](https://vinkius.com/mcp/keeptrack-space-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KeepTrack Space Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keeptrack-space-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KeepTrack Space Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keeptrack-space-intelligence": {
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
