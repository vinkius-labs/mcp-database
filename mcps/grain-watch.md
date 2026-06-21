# Grain Watch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grain-watch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access silo temperature monitoring via Grain Watch — track grain temperature, humidity, hot spots, and spoilage risk from any AI agent.

## Description
Connect your **Grain Watch Silo Temperature Monitoring API** to any AI agent and take full control of real-time temperature tracking, humidity monitoring, hot spot detection, and AI-powered spoilage risk assessment through natural conversation.

### What you can do

- **Silo Management** — List and manage all temperature-monitored silos with grain types and sensor status
- **Real-Time Temperature** — Get current temperature readings from all sensors throughout the grain mass
- **Humidity Monitoring** — Track relative humidity levels for condensation risk assessment
- **Temperature History** — Analyze historical temperature trends to detect developing hot spots
- **Humidity History** — Monitor humidity patterns for moisture migration and condensation detection
- **Sensor Mapping** — View complete sensor layout with positions, depths, and zones
- **Hot Spot Alerts** — Receive automatic alerts when localized heating indicates potential spoilage
- **Spoilage Risk** — Get AI-powered risk assessments combining temperature, humidity, and grain type
- **Alert Management** — Monitor all active alerts for temperature, humidity, and sensor issues
- **Sensor Health** — Track sensor battery levels, communication status, and operational health
- **Facility Overview** — Get comprehensive facility-wide temperature summaries for executive reporting

### How it works

1. Subscribe to this server
2. Enter your Grain Watch API key and base URL (from your Grain Cloud dashboard)
3. Start monitoring silo conditions from Claude, Cursor, or any MCP-compatible client

No more manual temperature cable readings or climbing silos for inspections. Your AI acts as a dedicated grain storage analyst and condition monitoring assistant.

### Who is this for?

- **Grain Farmers** — monitor stored grain temperature conditions and detect hot spots early
- **Grain Elevator Operators** — manage temperature across hundreds of silos with automated alerts
- **Facility Managers** — oversee storage facilities with real-time sensor data and spoilage risk assessments
- **Agricultural Consultants** — provide data-driven storage management recommendations to clients


## Available Tools
- **get_alerts**: Returns alert type, severity (critical, warning, info), affected silo, timestamp, and recommended actions. Essential for comprehensive operational monitoring, issue detection, and management response. AI agents should use this when users ask "show me all active alerts", "what warnings have been triggered for silo 3", or need alert data for operational monitoring. Optional silo_id filters alerts for a specific silo.

Get all active alerts for temperature, humidity, and sensor issues
- **get_current_humidity**: Returns relative humidity (%) values from multiple sensor positions. High humidity combined with temperature indicates condensation risk and potential spoilage conditions. Essential for moisture migration detection, condensation risk assessment, and grain quality preservation. AI agents should reference this when users ask "what is the humidity level in silo 3", "show me humidity readings for silo 5", or need current humidity data for storage condition assessment.

Get current humidity readings from sensors in a grain silo
- **get_current_temperature**: Returns temperature values (Celsius) from multiple sensor positions throughout the grain mass including top, middle, bottom, and center zones. Essential for real-time grain condition monitoring, hot spot detection, and spoilage prevention. AI agents should use this when users ask "what is the current temperature in silo 2", "show me all temperature readings for silo 4", or need immediate grain temperature data for storage management decisions.

Get current temperature readings from all sensors in a grain silo
- **get_facility_overview**: Essential for executive reporting, facility-wide condition assessment, and strategic storage management. AI agents should use this when users ask "give me an overview of all my silos", "what is the overall temperature status across the facility", or need facility-level summaries for management reporting.

Get comprehensive overview of all monitored silos and their temperature status
- **get_hotspot_alerts**: Returns alert severity (critical, warning), affected silo, sensor zone location, temperature differential, detection timestamp, and recommended actions. Hot spots are early indicators of grain quality issues that require immediate attention. Essential for proactive grain management, spoilage prevention, and quality preservation. AI agents should use this when users ask "are there any hot spots detected", "show hotspot alerts for silo 3", or need early warning indicators of grain spoilage. Optional silo_id filters alerts for a specific silo.

Get active hot spot detection alerts for all silos or a specific silo
- **get_humidity_history**: Humidity patterns over time help identify moisture migration, condensation events, and drying effectiveness. Returns time-series humidity data (%) with timestamps from multiple sensor positions. Essential for moisture migration analysis, condensation detection, and storage safety monitoring. AI agents should reference this when users ask "show me humidity trends for silo 1", "has humidity been stable in silo 2", or need historical humidity data for storage management.

Get historical humidity readings to track moisture migration patterns
- **get_sensor_health**: Returns sensor IDs, positions, communication status, last reading time, battery levels (for wireless sensors), and operational status (active, offline, fault, needs calibration). Essential for sensor network maintenance, data continuity assurance, and monitoring system reliability. AI agents should reference this when users ask "are all sensors working in silo 5", "which sensors have gone offline", or need sensor health data for system administration.

Get health status of all temperature and humidity sensors in a silo
- **get_sensor_map**: Returns sensor IDs, physical locations (top/middle/bottom, center/perimeter), installation depths, and current operational status. Essential for understanding temperature distribution across the grain mass, identifying which sensor corresponds to which physical location, and troubleshooting sensor issues. AI agents should use this when users ask "show me the sensor layout for silo 4", "where are the sensors positioned in silo 6", or need sensor positioning data for temperature analysis interpretation.

Get the layout and positions of all temperature sensors in a silo
- **get_silo_details**: Essential for understanding silo context before analyzing temperature data, planning aeration strategies, or generating storage condition reports. AI agents should reference this when users ask "tell me about silo 3", "what grain is stored in silo 5 and how many sensors does it have", or need detailed silo metadata for informed analysis.

Get detailed information about a specific grain silo
- **get_silos**: Returns silo IDs, names, locations, grain types, current temperature status, and monitoring health. Essential for facility overview, silo inventory management, and selecting specific silos for detailed temperature analysis. AI agents should use this when users ask "show me all my monitored silos", "list temperature-monitored storage units", or need to identify available silos before querying temperature readings or alerts.

List all grain silos monitored by Grain Watch
- **get_spoilage_risk**: Returns risk level (low, moderate, high, critical), contributing factors, predicted days until spoilage if conditions persist, and recommended preventive actions. Essential for proactive grain management, early intervention planning, and quality preservation. AI agents should use this when users ask "what is the spoilage risk for silo 3", "is silo 5 at risk of spoilage", or need AI-driven risk assessments for storage management decisions.

Get AI-powered spoilage risk assessment for a specific silo
- **get_temperature_history**: Temperature trends over time are critical for identifying developing hot spots, spoilage heating, or effective cooling from aeration. Returns time-series temperature data (Celsius) with timestamps from multiple sensor zones. Essential for hot spot detection, spoilage heating identification, aeration effectiveness evaluation, and grain quality preservation. AI agents should use this when users ask "show me temperature trends for silo 3 over the past 30 days", "has silo 5 been heating up", or need historical temperature data for storage condition analysis. Optional days parameter controls lookback period.

Get historical temperature readings to detect trends and hot spot development


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grain Watch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current temperature readings for silo 3."

**🤖 AI Agent:**
> Fetching temperature readings for silo 3 (Wheat, 85% full)... Top zone: 18.2C (avg), Middle zone: 19.5C (avg), Bottom zone: 17.8C (avg), Center core: 20.1C. All 24 temperature lines reporting normal. Maximum temperature: 20.1C at center core. Temperature spread: 2.3C (within normal range). Assessment: Grain temperature is NORMAL — no hot spots detected. Temperature gradient is typical for stored wheat. Continue routine monitoring. Would you like to see the 30-day temperature trend?

---

**👤 You:**
> "Check for any hot spot alerts across my facility."

**🤖 AI Agent:**
> Checking facility hot spot alerts... 1 active hot spot detected. Silo 7 (Corn) — Zone: Center-mid depth, Temperature: 28.5C (7.2C above average). Detected 6 hours ago, trend: Rising. Recommended action: Activate aeration immediately and monitor temperature every 2 hours. All other silos are within normal temperature ranges. Facility average temperature: 19.3C. Would you like me to show the temperature history for silo 7 to see how quickly this hot spot developed?

---

**👤 You:**
> "Give me a facility-wide overview of all silo temperatures and any active alerts."

**🤖 AI Agent:**
> Generating facility overview... Total monitored silos: 12. Average temperature: 19.3C (normal range). Active hot spots: 1 (Silo 7, center-mid zone at 28.5C). Temperature alerts: 1 critical, 0 warnings. Sensor health: 96% online (1 sensor offline in Silo 4, scheduled maintenance). Overall spoilage risk: LOW for 10 silos, MODERATE for Silo 7, LOW for Silo 4. Priority action: Address hot spot in Silo 7 with immediate aeration. Schedule sensor replacement in Silo 4 within 1 week. Would you like detailed recommendations for each alert?


## ❓ FAQ

**Q: Can my AI detect hot spots developing in my grain silos before spoilage occurs?**
Yes! Use the `get_hotspot_alerts` tool to check for active hot spot detections across your silos. Hot spots are localized temperature increases that indicate early biological activity (mold, insects, or grain respiration) before visible spoilage. For trend analysis, use `get_temperature_history` to see how temperatures have been changing over the past days or weeks. Early hot spot detection gives you critical time to activate aeration and prevent grain loss.

**Q: How do I get the AI spoilage risk assessment for my silos?**
Use the `get_spoilage_risk` tool with your silo ID. Grain Watch AI analyzes temperature trends, humidity patterns, and grain type to provide a risk level (low, moderate, high, critical), contributing factors, predicted days until spoilage if conditions persist, and recommended preventive actions. This combines multiple data sources into a single actionable assessment. For a facility-wide view, use `get_facility_overview` to see overall risk across all silos.

**Q: Can I check the health of my temperature sensors to ensure reliable monitoring?**
Yes! Use the `get_sensor_health` tool with your silo ID to check the status of all temperature and humidity sensors. This shows which sensors are active, offline, or faulted, along with last communication times and battery levels for wireless sensors. You can also use `get_sensor_map` to see the physical layout of all sensors in a silo, helping you understand which zones each sensor monitors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grain-watch](https://vinkius.com/mcp/grain-watch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grain Watch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `grain-watch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grain Watch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grain-watch": {
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
