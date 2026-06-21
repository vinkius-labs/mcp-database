# NASA Earth — Full-Disk Imagery & Natural Events MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-earth-full-disk-imagery-natural-events)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nasa-earth-full-disk-imagery-natural-events-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nasa-earth-full-disk-imagery-natural-events-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **NASA Earth — Full-Disk Imagery & Natural Events** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-earth-full-disk-imagery-natural-events](https://vinkius.com/mcp/nasa-earth-full-disk-imagery-natural-events)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
