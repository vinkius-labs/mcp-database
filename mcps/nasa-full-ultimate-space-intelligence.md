# NASA Full — Ultimate Space Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-full-ultimate-space-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

The definitive NASA Mega-Server: 32+ tools spanning astronomy pictures, near-Earth asteroids, Mars rover photos, solar flares and CMEs, Earth imagery and natural disasters, 5,700+ exoplanets, NASA's media library, and technology patents — all from 10 official NASA data sources.

## Description
The **ultimate NASA Mega-Server** — 32+ tools across 7 domains from 10 data sources.

### 32+ Tools
- 🌌 APOD (3) — Today, date range, random
- ☄️ Asteroids (5) — NEOs, close approaches, fireballs
- 🔴 Mars (4) — Photos by sol/date, manifests, latest
- ☀️ Space Weather (7) — CME, flares, storms, shocks, particles
- 🌍 Earth (5) — EPIC imagery, EONET events
- 🪐 Exoplanets (4) — Confirmed, habitable zone, stats
- 📸 Media (4) — Images, videos, patents

### One API Key for Everything


## Available Tools
- **get_apod**: Includes title, explanation, image URL, copyright, and media type (image or video). Running since June 16, 1995 — one of the most popular websites across all federal agencies.

Get the Astronomy Picture of the Day — NASA's most popular API
- **get_apod_range**: Great for exploring a week or month of astronomical imagery. Maximum range is about 30 days per request.

Get APOD images for a date range
- **get_random_apod**: Perfect for discovering amazing space imagery you might have missed. Default: 5 random images.

Get random Astronomy Pictures of the Day from the 30-year archive
- **get_neo_feed**: Includes estimated diameter, velocity, miss distance, and whether potentially hazardous. Source: NASA NeoWs.

Get near-Earth asteroids approaching within a date range
- **get_neo_lookup**: Use SPK-IDs from the feed endpoint.

Get detailed information about a specific asteroid by its NASA SPK-ID
- **get_neo_browse**: Returns 20 asteroids per page. Use for exploring the complete known catalog of near-Earth objects.

Browse the complete catalog of known near-Earth asteroids
- **get_close_approaches**: Filter by distance threshold, date range, and minimum size. Critical for planetary defense monitoring.

Get future close approaches of asteroids to Earth from JPL CNEOS
- **get_fireballs**: Includes location, velocity, energy (kilotons of TNT equivalent), and altitude. Covers events worldwide.

Get atmospheric fireball (bolide) events detected by US government sensors
- **get_epic_images**: 5 million km from Earth. Available in natural color or enhanced color.

Get the latest full-disk images of Earth from the DSCOVR satellite
- **get_epic_by_date**: Each entry includes coordinates, sun position, and image identifier for constructing the full image URL.

Get EPIC Earth images for a specific date
- **get_epic_dates**: Useful for finding specific dates of interest before requesting images.

List all dates with available EPIC Earth images
- **get_natural_events**: Categories include wildfires, volcanic eruptions, severe storms, sea ice, dust/haze, floods, and earthquakes. Includes coordinates and source links.

Get active natural events worldwide: wildfires, volcanoes, storms, icebergs
- **get_event_categories**: List all EONET natural event categories
- **query_confirmed_planets**: Filter by planet name, discovery method (Transit, Radial Velocity, Imaging, Microlensing), discovery facility (Kepler, TESS, Keck), or year. Returns orbital period, radius, mass, equilibrium temperature.

Search confirmed exoplanets by name, discovery method, facility, or year
- **get_transit_planets**: Transit is the most productive method (>75% of all discoveries). Kepler and TESS are the primary transit missions.

Get exoplanets discovered via the transit method (Kepler/TESS)
- **get_habitable_zone**: These are the most promising candidates for life.

Get exoplanets in the habitable zone — where liquid water could exist
- **get_planet_stats**: Shows how exoplanet science has exploded since Kepler's launch in 2009.

Get global exoplanet discovery statistics: totals, methods, yearly trends
- **get_mars_photos**: Filter by camera: FHAZ (front hazard), RHAZ (rear hazard), MAST (mast), CHEMCAM, MAHLI, MARDI, NAVCAM. Curiosity has 800K+ photos.

Get Mars rover photos by sol number and camera
- **get_mars_photos_by_date**: Easier than using sol numbers. Works with all three rovers.

Get Mars rover photos by Earth date
- **get_mars_manifest**: Essential for understanding what data is available.

Get the mission manifest for a Mars rover
- **get_mars_latest**: Curiosity is still active and sending new photos. Opportunity and Spirit missions have ended but their full archives are available.

Get the most recent photos from a Mars rover
- **search_media**: Covers every mission: Apollo, Space Shuttle, ISS, Hubble, Webb, Mars rovers, and more. Filter by media type and year range.

Search NASA's image and video library — 140,000+ assets
- **get_media_asset**: Use NASA IDs from search results.

Get download URLs for a NASA media asset by its NASA ID
- **get_media_metadata**: Get full metadata for a NASA media asset
- **search_patents**: NASA technologies have been adapted into thousands of commercial products — from memory foam to water purification systems.

Search NASA patents and technology spinoffs available for licensing
- **get_cme**: CMEs are massive bursts of solar wind and magnetic fields from the Sun. Earth-directed CMEs cause geomagnetic storms and aurora. Default: last 30 days.

Get Coronal Mass Ejection (CME) events from NASA DONKI
- **get_solar_flares**: Classes: C (common), M (moderate), X (extreme). X-class flares cause radio blackouts and satellite disruption. Includes begin/peak/end times, active region, and instruments that detected it.

Get solar flare events by class (C, M, X) from NASA DONKI
- **get_geomagnetic_storms**: Includes Kp index and linked CME/shock data. Storms above Kp=7 are severe, Kp=9 is extreme. Affects power grids, GPS, satellites, and enables aurora at low latitudes.

Get geomagnetic storm events from NASA DONKI
- **get_interplanetary_shocks**: Shocks often precede geomagnetic storms and are caused by CME-driven disturbances in the solar wind.

Get interplanetary shock wave events from NASA DONKI
- **get_solar_energetic_particles**: SEPs are dangerous to astronauts and can damage satellite electronics.

Get Solar Energetic Particle (SEP) events from NASA DONKI
- **get_radiation_belt**: The Van Allen radiation belts can be energized during geomagnetic storms, posing risks to satellites in medium Earth orbit.

Get radiation belt enhancement events from NASA DONKI
- **get_donki_notifications**: A unified feed of all space weather events: CMEs, flares, storms, shocks, and radiation events. Good for a quick overview of recent solar activity.

Get all recent DONKI space weather notifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA Full — Ultimate Space Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Full space briefing: APOD, asteroid threats, Mars photos, and solar activity"

**🤖 AI Agent:**
> 🚀 **NASA Full Briefing**

🌌 APOD: Veil Nebula — Hubble captures a supernova remnant
☄️ NEOs: 14 asteroids this week, 1 PHA (2023 BX5, 340m)
🔴 Mars: 12 new Curiosity photos (Sol 4150)
☀️ DONKI: X1.2 flare from AR 3842, 2 CMEs detected
🌍 EONET: 48 active wildfires worldwide
🪐 Exoplanets: 5,748 confirmed

6 NASA systems queried simultaneously.

---

**👤 You:**
> "Tell me about the latest discoveries in the habitable zone."

**🤖 AI Agent:**
> NASA's Exoplanet Archive recently added 3 new confirmed planets to the habitable zone list. The most notable is Kepler-1649c, an Earth-sized planet orbiting a red dwarf star 300 light-years away.

---

**👤 You:**
> "Find an astronomy picture showing the Andromeda galaxy."

**🤖 AI Agent:**
> I retrieved the APOD for November 22, 2023, titled 'M31: The Andromeda Galaxy'. It's a stunning high-resolution mosaic showing the entire galaxy, dust lanes, and its two small satellite galaxies.


## ❓ FAQ

**Q: Why Full instead of individual servers?**
The Full server has **all 32+ tools** from 10 NASA data sources. Query APOD AND asteroids AND Mars AND solar flares AND exoplanets in a single session. One API key covers everything.

**Q: How many exoplanets does the API track?**
The Exoplanet Archive API tracks over 5,700 confirmed exoplanets, including their detailed physical characteristics, orbital data, and habitable zone status.

**Q: Does this include the Astronomy Picture of the Day (APOD)?**
Yes, the Full server includes complete access to APOD, allowing you to get today's image, search by specific dates, or retrieve a random selection of breathtaking astronomy pictures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-full-ultimate-space-intelligence](https://vinkius.com/mcp/nasa-full-ultimate-space-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NASA Full — Ultimate Space Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nasa-full-ultimate-space-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NASA Full — Ultimate Space Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nasa-full-ultimate-space-intelligence": {
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
