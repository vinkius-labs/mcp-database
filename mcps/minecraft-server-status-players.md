# Minecraft Server Status & Players MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/minecraft-server-status-players)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming-entertainment](../categories/gaming-entertainment.md)

Minecraft live infrastructure as an MCP: Java + Bedrock server status (player counts, MOTD, versions), player profile/UUID lookup, skin renders and the official 910-version Mojang manifest — keyless.

## Description
**Minecraft's live multiplayer infrastructure** as a single MCP server — the world's best-selling game, monitored through its public status services.

### What you can do
- **Server status (Java + Bedrock)** — ping any server: online flag, players online/max, clean MOTD, protocol version, SRV resolution, even Forge mod lists when exposed (2b2t: 1226 players, CubeCraft: 1600+)
- **Player profiles** — resolve username ⇄ UUID via Mojang, check premium status, get skin render URLs (avatar, helm, 3D head, body)
- **Version intelligence** — the full official Mojang manifest: 910 versions (releases, snapshots, old_beta/alpha) with types and release dates — mod/plugin compatibility answers
- **Server comparisons** — ping up to 8 servers at once, auto-detecting Java vs Bedrock, ranked by population

### Why it matters
Server status is the heartbeat of Minecraft culture: "is 2b2t up?", "how many people are on Hypixel right now?", "does this server support 1.21?" — answered with live data, not stale screenshots.

### Who is this for?
Server admins, Discord bot builders, YouTubers, community moderators, hosting providers and AI agents that monitor or report on Minecraft multiplayer.


## Available Tools (7)
- **get_java_server_status**: io: online flag, players online/max, clean MOTD text, protocol version, SRV record resolution, Forge/Modded mod list when exposed. Works with hostnames (play.cubecraft.net, 2b2t.org) or IPs. For "is this server up and how many players are on?".

Check a Minecraft JAVA server live status: online state, player count, version, MOTD
- **get_player_skins**: Combine with lookup_player for display cards. No fetch needed — the URLs are embeddable images.

Get skin/head render URLs for a Minecraft player (avatar, helm, body, isometric)
- **list_game_versions**: Essential for mod/plugin compatibility checks ("does X support 1.21.4?").

List Minecraft game versions from the official Mojang manifest (910+ releases and snapshots)
- **lookup_player**: Returns the canonical profile id and name. Useful before rendering skins or checking if a premium username exists.

Resolve a Minecraft player profile by username OR UUID (id, name, textures availability)
- **compare_servers**: For "which server has more players right now?" and uptime spot-checks.

Compare multiple Minecraft servers side by side (player counts, versions, online state)
- **get_bedrock_server_status**: io): online flag, players online/max, gamemode (Survival/Creative), version name and protocol. The Hive, Lifeboat, CubeCraft-Bedrock and Realms-alternatives use Bedrock. Note the platform: many big servers run both Java AND Bedrock.

Check a Minecraft BEDROCK server live status: players, version, gamemode
- **get_version_details**: Get full details of one Minecraft version: type, release date and JSON manifest URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Minecraft Server Status & Players** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is 2b2t online right now? How many players?"

**🤖 AI Agent:**
> ⛏️ **2b2t.org — Java status**

🟢 ONLINE — **1226 players** online
Version: Velocity 1.7.2-26.2
MOTD: the oldest anarchy server, as always

Queue is probably long at this hour. Want me to compare player counts with other anarchy servers?

---

**👤 You:**
> "Compare Hypixel, CubeCraft and The Hive player counts"

**🤖 AI Agent:**
> 📊 **Server population ranking (live)**

1. 🟢 The Hive (Bedrock) — 23,204 players
2. 🟢 CubeCraft (Java) — 1,616 players
3. ⚫ Hypixel — offline from here / rate-limited

Bedrock servers dominate raw player counts — The Hive alone outnumbers most Java networks. Want a status check on the Java runners-up?

---

**👤 You:**
> "What's the latest Minecraft snapshot and when did 1.21.4 release?"

**🤖 AI Agent:**
> 🗂️ **Mojang version manifest**

Latest release: 26.2 · Latest snapshot: 26.3-pre-2 (2026-09-04)
1.21.4: released as a full release — exact date pulled from the manifest.

910 versions tracked since old_alpha. Need the JSON manifest URL for your launcher?


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. mcstatus.io, the Mojang profile API and the piston-meta version manifest are all public — no authentication anywhere in this MCP.

**Q: Why does a server show offline when I know it's up?**
Some servers block status pings (enable-status=false in server.properties), hide behind proxies, or are Bedrock-only (a Java ping fails). The compare_servers tool auto-probes Bedrock too — try it there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/minecraft-server-status-players](https://vinkius.com/en/ai-agent-connect/minecraft-server-status-players)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Minecraft Server Status & Players** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `minecraft-server-status-players` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Minecraft Server Status & Players** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "minecraft-server-status-players": {
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
