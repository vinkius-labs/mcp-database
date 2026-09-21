# Solar Imagery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/solar-imagery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Live images of the Sun from NASA's SDO and SOHO — every AIA wavelength, the HMI magnetogram, and the LASCO coronagraphs that watch for coronal mass ejections, keyless.

## Description
Connect any AI agent to **NASA's solar telescopes** — the live frames that space-weather forecasters actually look at. No key required.

### What you can do

- **See the Sun in ten wavelengths** — each AIA channel photographs the solar atmosphere at a different temperature, from the 6,000-degree surface to the 10-million-degree flare plasma
- **Read the magnetic field** — the HMI magnetogram shows sunspot groups as black-and-white polarity pairs, and the intensitygram shows sunspots as the eye would
- **Watch for coronal mass ejections** — the 193 Å running-difference frame highlights anything that erupted between scans, and the LASCO C2/C3 coronagraphs photograph the CME itself out to 30 solar radii
- **Match a phenomenon to the right product** — say "sunspots" or "coronal hole" and get the product that shows it, with the reason
- **Know whether a frame is live** — capture time and file size come from the file itself, and a frame older than a day is flagged stale

### Why it matters

Space weather starts on the Sun. A flare in 94 Å and a CME in LASCO C3 are the two observations that precede a geomagnetic storm — and a C3 frame filling with a bright expanding cloud is the signature of a storm Earth-directed.


## Available Tools (4)
- **get_solar_image**: A frame older than a day is flagged stale — SDO pauses for manoeuvres and lunar transits, so try another wavelength or the coronagraphs.

Get a live image of the Sun — a stable NASA archive URL plus capture time, file size and whether the frame is fresh, for any AIA wavelength, HMI product, composite or LASCO coronagraph
- **list_solar_image_products**: Optionally narrow to one instrument: AIA, HMI or LASCO.

List the solar image products one imager publishes — every AIA wavelength, the HMI continuum and magnetogram, the composites, and the LASCO coronagraphs — with what each one reveals
- **list_solar_instruments**: AIA photographs the solar atmosphere in ten extreme-ultraviolet wavelengths that each show a different temperature; HMI maps the visible surface and magnetic field; LASCO occults the disc to photograph coronal mass ejections. All keyless, all live.

List the solar imagers this API serves — SDO's AIA and HMI, and SOHO's LASCO coronagraphs — with what each one observes and how many products it publishes
- **find_solar_product_for**: Returns the best product plus alternates that show the same thing; pass the id to get_solar_image for the frame. For an Earth-directed CME the answer is the LASCO C3 coronagraph.

Pick the solar image product that shows a phenomenon — sunspots, a flare, a coronal mass ejection, a coronal hole, a filament, the magnetic field — with the reason it fits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solar Imagery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me what the Sun looks like right now."

**🤖 AI Agent:**
> The SDO HMI intensitygram, captured about 10 minutes ago — the solar disc in white light with sunspot groups visible as dark patches: https://sdo.gsfc.nasa.gov/assets/img/latest/latest_1024_HMII.jpg. For the corona and any eruptions, the AIA 171 Å frame shows coronal loops and the LASCO C3 coronagraph watches for Earth-directed CMEs.

---

**👤 You:**
> "Is there a coronal mass ejection heading our way?"

**🤖 AI Agent:**
> The product to check is the LASCO C3 coronagraph, which occults the solar disc and photographs the outer corona out to 30 solar radii: https://soho.nascom.nasa.gov/data/realtime/c3/1024/latest.jpg. A bright expanding cloud filling that frame is the signature of an Earth-directed CME — pair it with the AIA 193 Å running-difference frame, which highlights material that left the disc between scans.

---

**👤 You:**
> "Where do I look for sunspots?"

**🤖 AI Agent:**
> The HMI intensitygram — the only product here that photographs the Sun in visible light, so sunspots appear as dark patches on the disc: https://sdo.gsfc.nasa.gov/assets/img/latest/latest_1024_HMII.jpg, a 1024 px frame refreshed about every 15 minutes. To see the magnetism behind them, the HMI magnetogram (latest_1024_HMIB.jpg) shows the same groups as black-and-white polarity pairs — that is how active regions are numbered and tracked.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads NASA's public SDO and SOHO image archives, which require no key or account.

**Q: What do the AIA wavelength numbers mean?**
They are angstroms of extreme-ultraviolet light. Each one is emitted by plasma at a characteristic temperature: 304 Å shows the 50,000-degree chromosphere, 171 Å the million-degree coronal loops, and 94 Å and 131 Å the multi-million-degree plasma of solar flares.

**Q: Which product shows a coronal mass ejection?**
Two of them. The AIA 193 Å running-difference frame (aia193-difference) shows the eruption leaving the disc, and the LASCO C3 coronagraph (lasco-c3) photographs it out to 30 solar radii — a bright expanding cloud filling that frame is an Earth-directed CME. Call find_solar_product_for with "cme" to get both.

**Q: Why is an image marked stale?**
Its capture time is more than a day old. SDO pauses imagery during spacecraft manoeuvres, lunar transits and instrument calibration; SOHO pauses during Spacecraft rolls. Try another wavelength or the coronagraphs, and retry later.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/solar-imagery](https://vinkius.com/en/ai-agent-connect/solar-imagery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Solar Imagery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `solar-imagery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Solar Imagery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solar-imagery": {
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
