# Earth Imagery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/earth-imagery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Images of Earth from NASA's EPIC camera aboard DSCOVR — the freshest frames, the archive by date, and the scans centred nearest a place, keyless.

## Description
Connect any AI agent to **NASA's EPIC camera** aboard NOAA's DSCOVR spacecraft, parked at the Earth–Sun L1 Lagrange point a million miles away — the view that sees the whole sunlit Earth at once. No key required.

### What you can do

- **See the newest image of Earth** — the latest frame published, with capture time and a permanent archive URL
- **Browse the archive** — every date EPIC captured imagery, paged with offset and amount
- **Get every scan on a date** — roughly one frame per hour across the dayside, enough to watch a full rotation
- **Fetch one frame by identifier** — with the sub-spacecraft point and the J2000 positions of DSCOVR, the Moon and the Sun
- **Find the frames facing a place** — pass a latitude and longitude, get the scans whose view was centred nearest it, with distance and bearing

### Why it matters

EPIC is the only camera that continuously watches the whole sunlit disc, which is why it is the reference for daylight cloud cover, dust plumes and volcanic ash. The natural collection is the calibrated true-colour version; the enhanced collection boosts colour and contrast for detail, and trails it by days to weeks.


## Available Tools (6)
- **get_earth_images_by_date**: Accepts ISO dates only (YYYY-MM-DD). Throws when the collection has no frames that day and names dates that do.

Get every image of Earth NASA EPIC captured on one date — capture time, sub-spacecraft point and archive URL for each scan
- **get_latest_earth_images**: The natural collection publishes the same day; the enhanced collection lags it, so ask for natural when freshness matters. Returns the newest frame first. The URL points into the permanent archive and never changes.

Get the freshest images of Earth NASA EPIC has published — capture time, the point on Earth under the spacecraft, and a stable archive URL for each frame
- **list_epic_collections**: The two collections are the same frames treated differently: natural is the calibrated true-colour version and publishes same-day; enhanced has colour and contrast boosted for cloud detail and trails it by days to weeks. Both are keyless.

List the NASA EPIC imagery collections — natural colour and enhanced colour — with how many dates each one covers and which date is newest, from the DSCOVR spacecraft at the Earth–Sun L1 point
- **list_epic_dates**: This tool lists the dates that actually have frames. Pass offset to page backwards in time; amounts over 100 are rejected because the index is long. Hand one of the dates to get_earth_images_by_date.

Page through every date NASA EPIC captured imagery, newest first — the archive index for planning a lookup by date
- **find_earth_images_near**: Distances are great-circle kilometres from the place to the scan centre; a small distance means the place was near the middle of the frame. Widen max_distance_km or raise max_dates when nothing matches.

Find the NASA EPIC scans whose view was centred closest to a latitude and longitude — the frames where a given place was facing the camera
- **get_earth_image**: Get identifiers from get_latest_earth_images, get_earth_images_by_date or find_earth_images_near.

Get one NASA EPIC frame by its identifier — the full record with archive URL, capture time, sub-spacecraft point and the J2000 positions of DSCOVR, the Moon and the Sun


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Earth Imagery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the most recent photo of Earth."

**🤖 AI Agent:**
> EPIC's natural collection, captured 2026-09-17 00:03:42 UTC with scan centre 6.5N, 178.4E: https://epic.gsfc.nasa.gov/archive/natural/2026/09/17/png/epic_1b_20260917000831.png — the newest frame NASA has published.

---

**👤 You:**
> "Was New York facing the EPIC camera recently?"

**🤖 AI Agent:**
> The closest recent natural scan to 40.71N, 74.01W is epic_1b_20260916163014, 3859 km away on a bearing of 168° — the scan centre was well south of the city, so New York sat in the upper part of that frame: https://epic.gsfc.nasa.gov/archive/natural/2026/09/16/png/epic_1b_20260916163014.png

---

**👤 You:**
> "Show me EPIC's first portraits of the whole sunlit Earth, from July 2015."

**🤖 AI Agent:**
> On 2015-07-06 EPIC took five frames spaced hours apart — the set NASA released that month as its first images of the entire sunlit Earth. The first, epic_1b_20150706051132 at 05:01 UTC, was centred on 19.1N 112.7E (Asia); the sequence then walked west — 07:01 UTC at 82.7E, 11:01 UTC at 22.7E (Africa and the Indian Ocean) — and by 18:01 UTC the centre had reached 18.9N 82.3W, with the Americas sunlit: https://epic.gsfc.nasa.gov/archive/natural/2015/07/06/jpg/epic_1b_20150706051132.jpg. Ask for 2015-07-06 to get all five.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads NASA's public EPIC archive, which requires no key or account.

**Q: What is the difference between the natural and enhanced collections?**
They are the same frames. Natural is the calibrated true-colour composite and publishes the same day; enhanced has colour and contrast boosted to show cloud and surface detail, and its pipeline trails natural by days to weeks. Ask for natural when freshness matters.

**Q: Why is there no imagery on the date I asked for?**
DSCOVR does not image every day. The tool reports the dates that do have frames — call list_epic_dates first when you are unsure, and switch collections if one has nothing for that day.

**Q: What does the distance in find_earth_images_near mean?**
Great-circle kilometres from the place you gave to the scan centre — the point on Earth directly under the spacecraft. A small distance means the place was near the middle of the frame and facing the camera; EPIC sees each longitude roughly once per day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/earth-imagery](https://vinkius.com/en/ai-agent-connect/earth-imagery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Earth Imagery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `earth-imagery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Earth Imagery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "earth-imagery": {
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
