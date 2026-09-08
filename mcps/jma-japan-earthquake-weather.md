# JMA Japan Earthquake & Weather MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/jma-japan-earthquake-weather)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Japan Meteorological Agency official live data: recent earthquakes with seismic intensity (0-7 scale), per-city intensity reports, active weather warnings for all prefectures, 3-day + weekly forecasts and the real-time disaster feed — keyless.

## Description
The **Japan Meteorological Agency (JMA)** — the world's most respected earthquake and weather authority — as a single MCP server, straight from the JSON endpoints that power jma.go.jp.

### What you can do
- **Recent earthquakes** — the latest JMA bulletins with epicentre region (Japanese + English), coordinates, magnitude and max seismic intensity on Japan's famous 0-7 scale, plus per-city intensity breakdowns
- **Full event reports** — detailed quake reports per prefecture/city, exactly as issued
- **Live weather warnings** — active warnings and advisories per prefecture office (Tokyo 130000, Osaka 270000, Sapporo 011000...) with status (issued/ongoing/released)
- **Official forecasts** — 3-day detailed forecasts (weather code, wind, waves) + weekly trends for every prefecture area
- **Real-time disaster feed** — the JMAXML high-frequency feed: earthquakes, volcanic bulletins and tsunami notices the moment they are published

### Why JMA and not USGS?
USGS gives global locations and magnitudes; JMA gives what actually matters in Japan: the Shindo seismic-intensity scale (0-7) measured at thousands of stations, per-city intensity reports, official Japanese warnings, volcanic bulletins and tsunami notices. When Japan says "intensity 6+", this is the source.

### Who is this for?
Travel safety briefings, earthquake-aware applications, news monitoring, researchers, expats and anyone building agents that need authoritative Japan disaster + weather data.


## Available Tools (6)
- **get_recent_earthquakes**: Some entries are tsunami-related bulletins. Filter client-side by region or magnitude as needed.

List recent Japan earthquakes with epicentre, magnitude and max seismic intensity (JMA official)
- **get_earthquake_detail**: Japanese original with structure intact.

Get full JMA report for one earthquake (cities with seismic intensity, epicentre details)
- **get_weather_warnings**: headlineText summarises current warnings in Japanese; status values like 継続 (ongoing), 発表 (issued), 解除 (released). Empty warnings array = all clear.

Get ACTIVE JMA weather warnings and advisories for a prefecture (weather + earthquake early warning areas)
- **get_weather_forecast**: Areas are sub-prefecture regions with codes (Tokyo 130000 → 東京地方 130010, 伊豆諸島 130020...). weatherCodes map to icons: 100=clear, 200=cloudy, 300=rain, 400=snow, 2xx/3xx variants — combine with warnings for safety briefings.

Get official JMA weather forecast (3 days + weekly) for a prefecture area
- **list_office_codes**: Japan has 47 prefectures but 46 offices (Hokkaido is split: 011000 Sapporo, 012000 Hakodate, 013000 Asahikawa, 014100 Kushiro/Obihiro; Okinawa = 471000).

Reference table of JMA prefecture office codes (46 offices incl. Hokkaido split and Okinawa)
- **get_disaster_feed**: g. 震源・震度に関する情報 = epicentre/intensity info, 火山の状況 = volcano status, 津波警報 = tsunami warning), update times and detail XML paths. Use to catch events that have no earthquake-list entry yet (volcanic activity, tsunami advisories).

Browse the JMA real-time disaster feed (earthquakes, volcano bulletins, tsunami) as a structured list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JMA Japan Earthquake & Weather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Any earthquakes in Japan today? Show me the strongest ones"

**🤖 AI Agent:**
> 🇯🇵 **Today's JMA earthquake bulletins**

Latest: **M3.8 — Kumamoto Region, Kumamoto Prefecture** at 23:21 JPT, max intensity 3 (Shindo scale)
Also reported: epicentre/intensity info for Izu Islands (M2.1, intensity 1)

All well below damaging levels. Want the per-city intensity breakdown of the Kumamoto quake?

---

**👤 You:**
> "Check the disaster feed for any volcano or tsunami bulletins right now"

**🤖 AI Agent:**
> 🌋 **JMA real-time disaster feed**

35 entries in the high-frequency feed. Recent:
- 震源・震度に関する情報 (epicentre & intensity) — 23:25 JPT
- 震度速報 (intensity flash) — 23:21 JPT
- No volcanic eruption notices (噴火警報) or tsunami warnings (津波警報) in the current window

All clear on the volcano/tsunami front. I can keep monitoring and pull details of any new entry.

---

**👤 You:**
> "I'm traveling to Osaka this week — weather and any active warnings?"

**🤖 AI Agent:**
> 大阪 **Osaka travel briefing (JMA)**

⚠️ Warnings: strong-wind advisory (強風注意報) ongoing for Osaka city — status 継続
🌤️ 3-day forecast: cloudy→sunny, highs 30°C, winds weakening tomorrow
📅 Weekly trend: sunny through the weekend, next rain window Thursday

Pack light — no dangerous warnings active. Typhoon season note: I can monitor the disaster feed for you.


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. This MCP reads the same JSON/XML endpoints the official jma.go.jp portal uses — fully public, no authentication.

**Q: Why is JMA better than USGS for Japan earthquakes?**
JMA measures the Shindo seismic-intensity scale (0-7) at thousands of stations across Japan — two quakes with the same magnitude can have very different intensity. It also issues the official Japanese warnings, volcanic bulletins and tsunami notices. USGS reports magnitudes globally; JMA reports what people actually feel.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/jma-japan-earthquake-weather](https://vinkius.com/ai-agent-connect/jma-japan-earthquake-weather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JMA Japan Earthquake & Weather** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jma-japan-earthquake-weather` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JMA Japan Earthquake & Weather** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jma-japan-earthquake-weather": {
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
