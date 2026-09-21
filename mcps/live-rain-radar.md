# Live Rain Radar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/live-rain-radar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Live global precipitation radar from RainViewer — list the latest radar sweeps, get tile URLs for any location, and build playable rain animations.

## Description
Connect any AI agent to **live weather radar** — real precipitation data from the global radar network, served through RainViewer's public API. No key required.

### What you can do

- **See what's falling right now** — list the radar frames currently available, typically the last ~2 hours of sweeps at 10-minute intervals plus a short nowcast
- **Get a radar tile for any point** — give it a latitude and longitude, get back a PNG tile URL showing precipitation over that spot at your chosen zoom and colour scheme
- **Build a rain animation** — get an ordered sequence of tile URLs, one per frame, that a UI can play to watch the rain move

### How it works

1. Subscribe to this server — no account, no key
2. Ask your agent: "Is it raining in Lisbon right now?", "Show me the last two hours of rain over Berlin", "Give me a radar tile for Tokyo at zoom 10"
3. The agent returns ready-built image URLs — fetch them or hand them straight to a UI

Radar sweeps refresh roughly every 10 minutes, and each frame's URL is ephemeral: a tile built more than a few minutes ago may stop resolving, so rebuild from a fresh frame list if that happens.

### Who is this for

- **Weather-aware apps** — add live radar without negotiating a paid weather API
- **Event and logistics planners** — check precipitation along a route or at a venue
- **Developers** — prototype radar features with agent-driven tile retrieval
- **Anyone with a chat window** — "is it raining where I am?" answered from real sweeps, not a forecast icon


## Available Tools (3)
- **list_radar_frames**: Each frame has a Unix time and an ISO timestamp. Nothing here is an image yet — use the frame times with get_radar_tile or build_radar_animation to get tile URLs. The infrared satellite layer is listed separately and is often empty at night; that is expected, not an outage.

List the precipitation radar frames currently available from RainViewer — past sweeps plus nowcast
- **build_radar_animation**: Play them in order at ~10-minute intervals to animate the radar. Each URL is a raster tile addressed by lat/lon and zoom — this server builds the URLs, it does not return image bytes. Frame hashes expire within minutes, so build the animation close to when you need it.

Build a sequence of radar tile URLs for a location — one per frame — so a UI can play the rain moving over time
- **get_radar_tile**: Omit frame_time for the latest observed sweep, or pass a Unix time from list_radar_frames to pick the closest frame. Frame hashes are ephemeral: a tile URL built more than a few minutes ago may 404 — rebuild from a fresh index if so. Zoom 0-20 (8 is a good city-scale default); size 256 or 512; color 0-8 controls the palette (2 is the classic RainViewer blue-green-red).

Get the URL of the live precipitation radar tile covering a latitude/longitude, for the latest or a specific radar frame


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Live Rain Radar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it raining in Lisbon right now? Show me the radar."

**🤖 AI Agent:**
> Here's the latest radar tile over Lisbon — the returned URL is the current sweep, so open it to see precipitation intensity at that moment. If it looks clear, nothing is falling; if you see green or yellow over the city, rain is moving through.

---

**👤 You:**
> "Give me an animation of the last two hours of rain over Berlin."

**🤖 AI Agent:**
> Here are twelve tile URLs in chronological order, one per 10-minute sweep. Play them in sequence at about 10-minute cadence to watch the rain bands move across the city.

---

**👤 You:**
> "How fresh is the radar data right now? And is there any forecast for the next half hour?"

**🤖 AI Agent:**
> The archive holds 13 past sweeps at 10-minute cadence — the newest frame is from 06:10 UTC on 20 Sep 2026 and the oldest from 04:10 UTC, so the whole window reaches back about two hours. There are no forecast frames right now: RainViewer only publishes nowcast frames when precipitation is actually within about 30 minutes of a covered area, so an empty forecast means the immediate outlook is dry, not that the data is missing.


## ❓ FAQ

**Q: Does this need an API key?**
No. RainViewer's public radar index and tile cache are open. Subscribe and ask away.

**Q: Why do I get image URLs instead of the picture itself?**
Radar tiles are raster images — megabytes of PNG. An MCP tool passes text, so this server builds the exact URL for the frame, location, zoom and colour scheme you asked for. Hand it to any browser, image tag or fetch call.

**Q: A tile URL I got earlier now returns 404. What happened?**
Each radar frame is addressed by a short-lived hash that ages out minutes after the frame leaves the index. Call list_radar_frames again and rebuild — a fresh frame resolves immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/live-rain-radar](https://vinkius.com/en/ai-agent-connect/live-rain-radar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Live Rain Radar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `live-rain-radar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Live Rain Radar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "live-rain-radar": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
