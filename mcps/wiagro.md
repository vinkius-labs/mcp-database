# Wiagro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wiagro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access smart silobag monitoring via Wiagro — track temperature, humidity, CO2, rupture detection, and grain quality from any AI agent.

## Description
Connect your **Wiagro Smart Silobag API** to any AI agent and take full control of IoT-based grain condition monitoring, rupture detection, satellite environmental monitoring, and silobag quality management through natural conversation.

### What you can do

- **Silobag Management** — List and manage all silobags and conventional silos with grain types, fill levels, and monitoring status
- **Real-Time Readings** — Get current temperature, intergranular humidity, and CO2 readings from IoT sensors throughout the grain mass
- **Temperature History** — Track historical temperature trends to detect hot spots and spoilage heating
- **Humidity History** — Monitor intergranular humidity patterns for moisture migration and condensation detection
- **CO2 Tracking** — Follow CO2 trends as the earliest indicator of biological activity and grain spoilage
- **Rupture Detection** — Receive satellite-based alerts for silobag tears, holes, and structural damage
- **Alert Management** — Monitor active alerts for high temperature, humidity, and CO2 threshold breaches
- **Sensor Health** — Track IoT sensor battery levels, signal strength, and operational status
- **Satellite Monitoring** — Access satellite-based environmental data affecting silobag conditions
- **Quality Assessment** — Get AI-powered grain quality scores with storage life predictions
- **Facility Overview** — Get comprehensive facility-wide summaries for executive reporting

### How it works

1. Subscribe to this server
2. Enter your Wiagro API key and base URL (from your platform dashboard)
3. Start monitoring silobag conditions from Claude, Cursor, or any MCP-compatible client

No more manual silobag inspections or delayed quality testing. Your AI acts as a dedicated silobag monitoring analyst and grain preservation assistant.

### Who is this for?

- **Grain Farmers** — monitor stored grain conditions in silobags and detect spoilage early
- **Grain Traders** — assess grain quality across multiple storage locations for marketing decisions
- **Facility Managers** — oversee silobag facilities with real-time IoT sensor data and satellite monitoring
- **Agricultural Consultants** — provide data-driven storage management recommendations to clients


## Available Tools (12)
- **get_rupture_alerts**: Rupture alerts indicate tears, holes, or structural damage to silobags that could expose grain to weather, pests, and spoilage. Returns alert severity, location of rupture, detection timestamp, and recommended actions. Essential for silobag integrity monitoring, grain protection, and preventing quality loss. AI agents should use this when users ask "are there any silobag ruptures detected", "show rupture alerts for silobag 3", or need structural integrity alerts for silobag management. Optional silobag_id filters alerts for a specific silobag.

Get silobag rupture detection alerts for all silobags or a specific one
- **get_alerts**: Returns alert severity (critical, warning, info), alert type, affected silobag, timestamp, and recommended actions. Essential for proactive grain management, quality issue detection, and operational response. AI agents should use this when users ask "show me all active alerts", "what warnings have been triggered for silobag 3", or need alert data for operational monitoring. Optional silobag_id filters alerts for a specific silobag.

Get active temperature, humidity, and CO2 alerts for silobags
- **get_co2_history**: CO2 is the earliest indicator of biological activity (mold, insects, grain respiration) that leads to spoilage. Returns time-series CO2 data in ppm with timestamps. Essential for spoilage trend analysis, early warning detection, and validating storage condition stability. AI agents should reference this when users ask "show me CO2 trends for silobag 3 over the past 30 days", "has CO2 been rising in silobag 5", or need historical CO2 data for grain quality assessment.

Get historical CO2 readings to track biological activity and spoilage trends
- **get_current_readings**: Returns temperature (Celsius), intergranular humidity (%), and CO2 levels (ppm) from multiple sensor positions throughout the grain mass. Essential for real-time grain quality monitoring, early spoilage detection, and storage condition assessment. AI agents should use this when users ask "what are the current conditions in silobag 2", "show me all sensor readings for silobag 4", or need immediate grain quality data for storage management decisions.

Get current temperature, humidity, and CO2 readings from sensors in a silobag
- **get_facility_overview**: Essential for executive reporting, facility-wide quality assessment, and strategic storage management. AI agents should use this when users ask "give me an overview of my entire facility", "what is the overall grain quality status", or need facility-level summaries for management reporting.

Get comprehensive overview of all monitored silobags and storage units
- **get_humidity_history**: Humidity migration and condensation are key drivers of spoilage and quality loss. Returns time-series humidity data (%) with timestamps from multiple sensor positions. Essential for moisture migration analysis, condensation detection, and storage safety monitoring. AI agents should use this when users ask "show me humidity trends for silobag 1", "has humidity been stable in silobag 2", or need historical humidity data for storage management.

Get historical intergranular humidity readings for moisture migration analysis
- **get_quality_assessment**: Returns quality score, risk level, estimated remaining storage life, and recommended actions. Essential for grain quality monitoring, marketing timing decisions, and storage duration optimization. AI agents should reference this when users ask "what is the grain quality in silobag 3", "assess storage conditions for silobag 5", or need quality assessment data for storage management and marketing decisions.

Get AI-powered grain quality assessment for a specific silobag
- **get_satellite_data**: Essential for understanding external risk factors, weather impact assessment, and proactive silobag protection. AI agents should use this when users ask "what is the satellite data for silobag 2", "show external conditions affecting silobag 4", or need environmental context for silobag management decisions.

Get satellite-based monitoring data for external silobag conditions
- **get_sensor_health**: Returns sensor IDs, positions (depth/location), battery levels, signal strength, last communication time, and operational status (active, low battery, offline). Essential for sensor network maintenance, data continuity assurance, and monitoring system reliability. AI agents should reference this when users ask "are all sensors working in silobag 5", "which sensors need battery replacement", or need sensor network health data for system administration.

Get health status of IoT sensors deployed in a silobag
- **get_silobag_details**: Essential for understanding silobag context before analyzing sensor data, planning aeration strategies, or generating quality reports. AI agents should reference this when users ask "tell me about silobag 3", "what grain is stored in silobag 5", or need detailed silobag metadata for informed analysis.

Get detailed information about a specific silobag or conventional silo
- **get_silobags**: Returns silobag IDs, names, locations, grain types, fill levels, and current monitoring status. Essential for facility overview, silobag inventory management, and selecting specific silobags for detailed analysis. AI agents should use this when users ask "show me all my silobags", "list monitored storage units", or need to identify available silobags before querying sensor readings or alerts.

List all silobags and conventional silos monitored by Wiagro
- **get_temperature_history**: Temperature increases often indicate active spoilage, insect activity, or mold growth. Returns time-series temperature data (Celsius) with timestamps from multiple sensor depths and positions. Essential for hot spot detection, spoilage heating identification, and grain quality preservation. AI agents should reference this when users ask "show me temperature trends for silobag 4", "are there any hot spots developing in silobag 6", or need historical temperature data for spoilage analysis. Optional days parameter controls lookback period.

Get historical temperature readings to detect hot spots and spoilage heating in a silobag


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wiagro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current temperature, humidity, and CO2 readings for silobag 3."

**🤖 AI Agent:**
> Fetching current readings for silobag 3 (Corn, 85% full)... Temperature: 22.3°C average across all sensors (max 23.1°C at center, min 21.5°C at edges). Humidity: 14.8% intergranular humidity (stable, within safe range). CO2: 920 ppm (normal, no biological activity detected). All 12 IoT sensors reporting healthy. Assessment: Grain condition is GOOD — no spoilage indicators detected. Temperature is uniform with no hot spots. Continue routine monitoring. Would you like to see the 30-day temperature trend?

---

**👤 You:**
> "Check for any silobag rupture alerts or active warnings across my facility."

**🤖 AI Agent:**
> Checking facility alerts... No rupture alerts detected — all silobags are structurally intact according to satellite monitoring. Active warnings: 1 alert found. Silobag 7 — CO2 level approaching threshold (1450 ppm, warning level is 1500 ppm). Recommended action: Increase monitoring frequency and consider targeted aeration if CO2 continues rising. All other silobags are within normal parameters. Facility quality score: 94/100. Would you like detailed sensor readings for silobag 7?

---

**👤 You:**
> "Give me a quality assessment for all my monitored silobags."

**🤖 AI Agent:**
> Generating quality assessments... Silobag 1 (Soybeans): Quality score 91/100 — Excellent condition, stable temperature at 18°C, CO2 at 780 ppm. Estimated storage life: 4+ months. Silobag 2 (Wheat): Quality score 87/100 — Good condition, minor temperature variation (20-22°C), CO2 at 890 ppm. Storage life: 3+ months. Silobag 3 (Corn): Quality score 94/100 — Excellent condition, uniform temperature, CO2 at 920 ppm. Storage life: 4+ months. Silobag 7 (Sorghum): Quality score 72/100 — FAIR condition, elevated CO2 trend (1450 ppm), requires closer monitoring. Storage life: 1-2 months if conditions stabilize. Priority action: Investigate silobag 7 CO2 increase. Overall facility average: 86/100.


## ❓ FAQ

**Q: Can my AI detect if a silobag has been ruptured or damaged?**
Yes! Use the `get_rupture_alerts` tool to check for satellite-detected silobag ruptures, tears, or structural damage. Wiagro uses satellite imagery analysis to identify breaches in silobag integrity that could expose grain to weather and pests. For a complete picture, combine with `get_alerts` to see temperature, humidity, and CO2 alerts that may indicate secondary effects of a rupture.

**Q: How do I monitor CO2 levels to detect early grain spoilage in silobags?**
Use the `get_co2_history` tool with your silobag ID and a date range (e.g., 30 days) to see CO2 trends over time. Rising CO2 levels indicate biological activity from mold, insects, or grain respiration — often appearing before temperature changes. Combine with `get_current_readings` for real-time CO2 status and `get_alerts` to check for any active CO2 warnings.

**Q: Can I check the health status of sensors in my silobag monitoring system?**
Yes! Use the `get_sensor_health` tool with your silobag ID to check battery levels, signal strength, and operational status of all IoT sensors. This helps you identify sensors that need battery replacement or have gone offline, ensuring continuous monitoring coverage. For a facility-wide view, use `get_facility_overview` to see the overall health of your monitoring system.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wiagro](https://vinkius.com/mcp/wiagro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wiagro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wiagro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wiagro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wiagro": {
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
