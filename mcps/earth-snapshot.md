# Earth Snapshot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/earth-snapshot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Render satellite imagery of any place on any day — NASA Worldview layers for true colour, active fires, aerosols and land surface, keyless.

## Description
Connect any AI agent to **on-demand satellite imagery of Earth** — NASA's Worldview snapshot service renders any published layer, over any region, on any day, as a JPEG URL that never expires. No key required.

### What you can do

- **Browse the imagery themes** — true and false colour, fires and thermal anomalies, aerosols and air, land surface
- **Find the right layer** — VIIRS, MODIS, Landsat, GOES and Aqua layer ids with their instruments and date ranges, resolved from a search phrase as well as an exact id
- **Render a snapshot** — any layer over a region given as lat/lon plus span, or as a bounding box, at up to 2000 px
- **Stack two layers** — fires or aerosol detections drawn over a true-colour underlay, the classic way to see what is burning against what it looks like
- **Find active fires** — VIIRS 375 m thermal anomaly points over a region, without needing a fire-specific API key

### Why it matters

This is the tool for "what did it look like then". Wildfire extent, smoke plumes crossing continents, snow cover, vegetation green-up and burn scars are all visible in layers that go back to 2000. Every request is checked against the layer's published date range — an out-of-range day renders a blank image rather than an error, so the tool refuses it instead.


## Available Tools (5)
- **find_active_fires**: A detection frame with no coloured points means no hot pixels that day — not a failed render. Fires are best seen on the day they burn; the burn scar shows for weeks afterwards in true colour.

Render the active fire detections over a region on a date — VIIRS 375 m thermal anomaly points, alone and overlaid on true-colour satellite imagery, keyless
- **get_layer_details**: Accepts a layer id or a search phrase like "aerosol" or "night lights"; returns the best match.

Get the details of one NASA Worldview layer — title, instrument, date range and projections — plus a small sample snapshot URL
- **get_earth_snapshot**: The image renders on request from the URL, which never expires. An overlay layer can be stacked on top — the classic pairing is true colour underneath with fires or aerosol on top. Out-of-range dates are rejected rather than rendered blank.

Render a satellite image of a place on a date — a NASA Worldview snapshot URL for any layer, any region, any day the layer was published
- **list_imagery_categories**: The categories cover the physical questions people ask of imagery: what it looks like, what is burning, what is in the air, and what is on the ground.

List the themes of satellite imagery available — true colour, fires and thermal anomalies, aerosols and air, land surface — with what each one shows
- **list_imagery_layers**: The date range matters: some layers are recent, and a few are discontinued — an id whose end date has passed cannot render after it.

List the satellite imagery layers in one theme — NASA Worldview layer ids with their titles, instruments and the dates each one covers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Earth Snapshot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a satellite view of the New York area on September 1st, 2026."

**🤖 AI Agent:**
> MODIS Terra's Corrected Reflectance (True Color) — the natural look of the day, published continuously since February 2000. Over 8 degrees centred on 40.7N, 74W, that is a box from 36.7N to 44.7N and 78W to 70W, rendered at 800x800 px: https://wvs.earthdata.nasa.gov/api/v1/snapshot?REQUEST=GetSnapshot&LAYERS=MODIS_Terra_CorrectedReflectance_TrueColor&CRS=EPSG%3A4326&TIME=2026-09-01&BBOX=36.70%2C-78.00%2C44.70%2C-70.00&FORMAT=image%2Fjpeg&WIDTH=800&HEIGHT=800 — a 116 KB JPEG. For a sharper daily frame, the same view exists from VIIRS on Suomi NPP.

---

**👤 You:**
> "Were there fires burning in the Amazon on September 15th, 2026?"

**🤖 AI Agent:**
> Yes — the VIIRS 375 m thermal anomalies layer, Fires and Thermal Anomalies (Day and Night, 375m), published since January 2012, shows active fire pixels across the box from 13S to 3S and 65W to 55W: https://wvs.earthdata.nasa.gov/api/v1/snapshot?REQUEST=GetSnapshot&LAYERS=VIIRS_SNPP_Thermal_Anomalies_375m_All&CRS=EPSG%3A4326&TIME=2026-09-15&BBOX=-13.00%2C-65.00%2C-3.00%2C-55.00&FORMAT=image%2Fjpeg&WIDTH=800&HEIGHT=800 — coloured points over black. The composite draws those detections on top of true-colour imagery so the fires can be seen against the forest. A frame with no coloured points would mean no hot pixels that day, not a failed render.

---

**👤 You:**
> "How green is the Midwest farm belt right now?"

**🤖 AI Agent:**
> The MODIS Terra NDVI rolling 8-day layer, Normalized Difference Vegetation Index (NDVI) (rolling 8-day), published since February 2025. Over 12 degrees centred on 41N, 95W — from 35N to 47N and 101W to 89W — it renders at 800x800 px: https://wvs.earthdata.nasa.gov/api/v1/snapshot?REQUEST=GetSnapshot&LAYERS=MODIS_Terra_NDVI_8Day&CRS=EPSG%3A4326&TIME=2026-09-01&BBOX=35.00%2C-101.00%2C47.00%2C-89.00&FORMAT=image%2Fjpeg&WIDTH=800&HEIGHT=800. Dense canopy reads bright green; harvested fields and bare ground read brown. Comparing that frame with one from a month earlier shows green-up and senescence directly.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads NASA's public Worldview services — the layer catalog and the snapshot renderer — which require no key or account.

**Q: Does the tool return the image itself?**
It returns a URL that renders the image on request. The URL is stable and never expires — open it in a browser, embed it, or fetch it. Worldview composes the JPEG from the layer and region at request time, so it works for any date the layer covers and any size up to 2000 px.

**Q: Why was my date rejected?**
Layers have published lifetimes, and a date outside that range renders a blank image instead of returning an error — so the tool checks and refuses. Night lights only covers 2012 and 2016, snow extent ended in 2024, and nothing can be rendered for a future date. Call get_layer_details to see a layer's range, or list_imagery_layers for alternatives in the same theme.

**Q: What does it mean when a fire detection frame looks empty?**
The VIIRS 375 m layer colours hot pixels over a black background, so a frame with no coloured points means no thermal anomalies were recorded in that region that day — that is the answer, not a failed render. Compare it with the composite, which draws the same detections on true-colour imagery, or widen the region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/earth-snapshot](https://vinkius.com/en/ai-agent-connect/earth-snapshot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Earth Snapshot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `earth-snapshot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Earth Snapshot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "earth-snapshot": {
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
