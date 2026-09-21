# GOES Satellite Imagery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/goes-satellite-imagery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Live imagery URLs from NOAA's GOES satellites — full disk, continental US and mesoscale regions, with capture time, resolution and file size, keyless.

## Description
Connect any AI agent to **live satellite imagery of Earth** — the JPEGs NOAA's GOES-18 and GOES-19 publish every 5 to 10 minutes on the public STAR CDN. No key required.

### What you can do

- **See which satellites are live** — GOES East and GOES West, with the part of the globe each one covers
- **Discover sectors and regions** — full disk (FD), continental US (CONUS) and the named mesoscale boxes (MESO), each with its centre coordinates
- **List the composite products** — GEOCOLOR for a natural true-colour view, FireTemperature for active wildfires, Dust for dust and smoke, DayNightCloudMicroCombo for fog after sunset, and more
- **Get a live image URL** — always resolves to the newest scan, with capture time, pixel dimensions, file size and the other resolutions available
- **Find the region for a place** — pass a latitude and longitude, get the mesoscale box that covers or sits nearest it

### Why it matters

GOES imagery is how wildfires, dust storms, fog banks and hurricanes are tracked as they happen. FireTemperature shows hot ground before a fire is visible in smoke; GEOCOLOR shows a storm's full extent in one frame.


## Available Tools (5)
- **find_goes_region**: Region ids are the centre coordinates written as "33N-101W". Only GOES satellites publish mesoscale regions.

Find the GOES mesoscale region that covers or sits nearest a latitude and longitude — pass a place, get back the region id to use with get_latest_satellite_image
- **get_latest_satellite_image**: The capture time is read from the newest archived scan in the same directory, since the file itself carries no usable timestamp. Pass resolution "latest" for the full-resolution master (very large — tens of megabytes for full disk) or a WxH.jpg name from available_resolutions for something lighter. Mesoscale imagery needs a region id like "33N-101W"; find one with list_goes_sectors or find_goes_region. Unknown values are rejected with the nearest valid suggestion.

Get the URL of the latest GOES satellite image — full disk, continental US or a mesoscale region — with its capture time, pixel dimensions and file size
- **list_goes_products**: The list comes from the CDN directory itself, so it reflects what that satellite and sector actually publish — mesoscale regions offer a smaller set than full disk. ABI bands 01–16 are deliberately absent: they are zip-only on the CDN. Pass a region when sector is MESO.

List the composite imagery products published for one satellite and sector — GEOCOLOR, FireTemperature, Dust, DayNightCloudMicroCombo and the rest — each with a note on what it reveals
- **list_goes_satellites**: NOAA retires and reassigns satellites over time, so the set changes; the answer reflects what the CDN actually serves today, not a hardcoded list. GOES East watches the Atlantic, eastern North America and South America; GOES West watches the Pacific, western North America, Alaska and Hawaii.

List the GOES satellites that are publishing imagery right now on the NOAA STAR CDN, with each one's role — GOES East or GOES West — and the part of the globe it covers
- **list_goes_sectors**: Mesoscale imagery needs a region id that looks like "33N-101W" — the lat-lon of the box centre — and the full set of region ids is in this answer, so read it here rather than guessing.

List the imagery sectors a GOES satellite publishes — full disk (FD), continental US (CONUS) and mesoscale (MESO) — plus every named mesoscale region with its centre coordinates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GOES Satellite Imagery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest satellite image of the wildfires in Texas."

**🤖 AI Agent:**
> The FireTemperature composite from GOES-19, mesoscale region 33N-101W: https://cdn.star.nesdis.noaa.gov/GOES19/ABI/MESO/33N-101W/FireTemperature/latest.jpg — 2000×2000 px, captured 2026-09-11 05:59 UTC. Hot ground shows bright orange against black. That region's archive has stopped, so this image is not live; M1 is the actively scanned box right now.

---

**👤 You:**
> "What does the Earth look like right now?"

**🤖 AI Agent:**
> GOES-19's GEOCOLOR full disk, captured 2026-09-20 03:20 UTC: https://cdn.star.nesdis.noaa.gov/GOES19/ABI/FD/GEOCOLOR/1808x1808.jpg — a true-colour view of the Atlantic, eastern North America and South America, 1808×1800 px and about 1.7 MB. A 21696×21696 px master and four smaller sizes are published in the same directory.

---

**👤 You:**
> "Show me the Pacific side instead — what does GOES-West see right now?"

**🤖 AI Agent:**
> GOES-West is GOES-18, parked at 137.0°W, so its full disk covers the Pacific, the western US, Alaska and Hawaii rather than the Atlantic. Its GEOCOLOR full disk was captured 2026-09-20 06:03 UTC: https://cdn.star.nesdis.noaa.gov/GOES18/ABI/FD/GEOCOLOR/latest.jpg, about 9.6 MB. Two satellites means two hemispheres — ask for GOES-19 (East, 75.2°W) when the Atlantic or eastern US is what you need.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads NOAA's public STAR content delivery network, which requires no key or account.

**Q: Does the tool return the image itself?**
It returns a stable JPEG URL that always points at the most recent scan, along with the capture time, pixel dimensions and file size. The link refreshes itself — the image behind it changes every 5 to 10 minutes.

**Q: What is the difference between FD, CONUS and MESO?**
FD is the full hemisphere the satellite sees, scanned every 10 minutes. CONUS is the contiguous United States, every 5 minutes. MESO boxes are roughly 1000 × 1000 km at the finest resolution, and need a named region such as 33N-101W — or M1 and M2, the boxes that follow significant weather.

**Q: Why does a mesoscale image show a capture time days ago?**
A mesoscale region is only scanned while it is assigned. When its archive stops, latest.jpg is a frozen older image, and the reported capture time says so — switch to another region, or to M1 or M2, which follow active weather.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/goes-satellite-imagery](https://vinkius.com/en/ai-agent-connect/goes-satellite-imagery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GOES Satellite Imagery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `goes-satellite-imagery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GOES Satellite Imagery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "goes-satellite-imagery": {
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
