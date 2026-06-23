# NASA Earth — Full-Disk Imagery & Natural Events MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-earth-full-disk-imagery-natural-events)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

View Earth from 1.5 million km away through DSCOVR's EPIC camera (full-disk images in natural and enhanced color) and track active natural events worldwide through EONET: wildfires, volcanic eruptions, severe storms, icebergs, and more.

## Description
Two complementary Earth observation systems.

### EPIC (DSCOVR)
- Full-disk images of the sunlit side of Earth
- Natural and enhanced color composites
- Browse by date

### EONET (Earth Observatory)
- Active natural events worldwide
- Categories: wildfires, volcanoes, storms, floods, etc.
- Coordinates and source links


## Available Tools (5)
- **get_epic_images**: 5 million km from Earth. Available in natural color or enhanced color.

Get the latest full-disk images of Earth from the DSCOVR satellite
- **get_epic_by_date**: Each entry includes coordinates, sun position, and image identifier for constructing the full image URL.

Get EPIC Earth images for a specific date
- **get_epic_dates**: Useful for finding specific dates of interest before requesting images.

List all dates with available EPIC Earth images
- **get_natural_events**: Categories include wildfires, volcanic eruptions, severe storms, sea ice, dust/haze, floods, and earthquakes. Includes coordinates and source links.

Get active natural events worldwide: wildfires, volcanoes, storms, icebergs
- **get_event_categories**: List all EONET natural event categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA Earth — Full-Disk Imagery & Natural Events** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any active wildfires right now?"

**🤖 AI Agent:**
> 🔥 **Active Wildfires (EONET)**

| Location | Coordinates | Source |
|----------|-------------|--------|
| Northern California | 41.2°N, 122.3°W | InciWeb |
| Siberia | 62.1°N, 114.8°E | MODIS |
| Australian Outback | 25.4°S, 133.2°E | FIRMS |

48 wildfires currently tracked by EONET.

---

**👤 You:**
> "Are there any strong storms currently being tracked?"

**🤖 AI Agent:**
> EONET is currently tracking Tropical Cyclone Freddy off the coast of Madagascar and a severe winter storm system moving across the US Midwest. There are also 5 smaller convective storms active.

---

**👤 You:**
> "Show me what Earth looked like on January 1, 2020."

**🤖 AI Agent:**
> I found 13 full-disk images of Earth taken by the EPIC camera on Jan 1, 2020. The first image taken at 00:15 UT shows the Pacific Ocean, Australia, and parts of Asia fully illuminated.


## ❓ FAQ

**Q: What is the DSCOVR satellite?**
DSCOVR orbits at the L1 Lagrange point, 1.5 million km from Earth. Its EPIC camera takes full-disk images of Earth every 1-2 hours, always showing the sunlit face.

**Q: What is EONET?**
EONET (Earth Observatory Natural Event Tracker) provides real-time data on active natural events. It tracks wildfires, severe storms, volcanoes, and more, updated daily from satellite sources.

**Q: Can I get historical data using the EPIC camera?**
Yes, you can browse images by specific dates since the DSCOVR satellite began taking regular photos in 2015, allowing you to see Earth on a specific past day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-earth-full-disk-imagery-natural-events](https://vinkius.com/mcp/nasa-earth-full-disk-imagery-natural-events)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NASA Earth — Full-Disk Imagery & Natural Events** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nasa-earth-full-disk-imagery-natural-events` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NASA Earth — Full-Disk Imagery & Natural Events** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nasa-earth-full-disk-imagery-natural-events": {
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
