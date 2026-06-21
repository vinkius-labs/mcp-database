# Centaur Analytics MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/centaur-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/centaur-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/centaur-analytics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access AI-powered grain monitoring via Centaur — track CO2, moisture, temperature, predict spoilage, and forecast grain quality from any AI agent.

## Description
Connect your **Centaur Analytics Internet-of-Crops API** to any AI agent and take full control of AI-powered grain quality monitoring, predictive spoilage detection, wireless sensor management, and enterprise grain storage intelligence through natural conversation.

### What you can do

- **Bin Management** — List and manage all grain storage bins with fill levels, grain types, and monitoring status
- **Real-Time Readings** — Get current CO2, moisture, and temperature readings from wireless sensors throughout the grain mass
- **CO2 Tracking** — Monitor historical CO2 trends as the earliest indicator of biological activity and spoilage
- **Moisture Analysis** — Track moisture content and migration patterns to detect condensation and quality risks
- **Temperature Monitoring** — Detect hot spots and spoilage heating with distributed temperature sensor data
- **AI Spoilage Predictions** — Receive machine learning-powered spoilage risk assessments with days-to-spoilage estimates
- **Quality Forecasting** — Predict future grain quality metrics using computer simulation models
- **Alert Management** — Monitor active alerts for high CO2, rising temperature, moisture issues, and sensor failures
- **Sensor Health** — Track wireless sensor battery levels, signal strength, and operational status
- **Facility Overview** — Get comprehensive facility-wide summaries for executive reporting and strategic management
- **Quality Reports** — Generate AI-powered comprehensive quality reports with actionable recommendations

### How it works

1. Subscribe to this server
2. Enter your Centaur API key and base URL (from your platform dashboard)
3. Start monitoring grain quality from Claude, Cursor, or any MCP-compatible client

No more manual bin inspections or delayed quality testing. Your AI acts as a dedicated grain quality analyst and predictive storage management assistant.

### Who is this for?

- **Grain Farmers** — monitor stored grain conditions, predict spoilage, and optimize marketing timing
- **Grain Elevator Operators** — manage quality across hundreds of bins with AI-driven insights
- **Facility Managers** — oversee storage facilities with real-time sensor data and predictive alerts
- **Commodity Traders** — assess grain quality and forecast value changes for trading decisions


## Available Tools
- **get_facility_overview**: Essential for executive reporting, facility-wide quality assessment, and strategic storage management. AI agents should use this when users ask "give me an overview of my entire facility", "what is the overall grain quality status", or need facility-level summaries for management reporting.

Get comprehensive overview of the entire grain storage facility
- **get_alerts**: Alerts are triggered by threshold breaches (high CO2, rising temperature, moisture migration, sensor failures) and indicate conditions requiring immediate attention. Returns alert severity (critical, warning, info), alert type, affected bin, timestamp, and recommended actions. Essential for proactive grain management, quality issue detection, and operational response. AI agents should use this when users ask "show me all active alerts", "what warnings have been triggered for bin 3", or need alert data for operational monitoring. Optional bin_id filters alerts for a specific bin.

Get active alerts and warnings for grain bins or a specific bin
- **get_bin_details**: Essential for understanding bin context before analyzing sensor data, planning aeration strategies, or generating quality reports. AI agents should reference this when users ask "tell me about bin 5", "what grain is stored in silo 3", or need detailed bin metadata for informed analysis.

Get detailed information about a specific grain storage bin
- **get_bins**: Returns bin IDs, names, locations, grain types, fill levels, and current monitoring status. Essential for facility overview, bin inventory management, and selecting specific bins for detailed analysis. AI agents should use this when users ask "show me all my grain bins", "list monitored storage units", or need to identify available bins before querying sensor readings or AI predictions.

List all grain storage bins monitored by Centaur Analytics
- **get_co2_history**: CO2 is the earliest indicator of biological activity (mold, insects, grain respiration) that leads to spoilage. Returns time-series CO2 data in ppm with timestamps. Essential for spoilage trend analysis, early warning detection, and validating storage condition stability. AI agents should reference this when users ask "show me CO2 trends for bin 3 over the past 30 days", "has CO2 been rising in silo 5", or need historical CO2 data for grain quality assessment. Optional days parameter controls lookback period.

Get historical CO2 readings to track spoilage trends over time
- **get_current_readings**: Returns CO2 levels (ppm), moisture content (%), and temperature (C) from multiple sensor positions throughout the grain mass. Essential for real-time grain quality monitoring, early spoilage detection, and storage condition assessment. AI agents should use this when users ask "what are the current conditions in bin 2", "show me all sensor readings for silo 4", or need immediate grain quality data for storage management decisions.

Get current CO2, moisture, and temperature readings from all sensors in a bin
- **get_moisture_history**: Moisture migration and condensation are key drivers of spoilage and quality loss. Returns time-series moisture data (%) with timestamps from multiple sensor positions. Essential for moisture migration analysis, condensation detection, drying effectiveness assessment, and storage safety monitoring. AI agents should use this when users ask "show me moisture trends for bin 1", "has moisture been stable in silo 2", or need historical moisture data for storage management.

Get historical moisture content readings for grain storage analysis
- **get_quality_forecast**: Uses computer simulation models combining current sensor data, weather forecasts, and grain characteristics. Essential for marketing timing, quality preservation planning, and storage duration optimization. AI agents should reference this when users ask "what will the grain quality be in bin 2 next month", "forecast quality changes for silo 4", or need predictive quality data for marketing and storage decisions.

Get AI-powered grain quality forecast for upcoming weeks
- **get_quality_report**: Combines current sensor readings, historical trends, spoilage predictions, quality forecasts, and actionable recommendations into a single report. Includes test weight estimates, moisture stability analysis, temperature uniformity assessment, and mycotoxin risk evaluation. Essential for quality documentation, marketing decisions, insurance claims, and comprehensive grain condition assessment. AI agents should reference this when users ask "generate a quality report for bin 2", "give me the complete grain condition assessment for silo 4", or need comprehensive quality documentation for a specific bin.

Get a comprehensive AI-generated quality report for a specific grain bin
- **get_sensor_health**: Returns sensor IDs, positions (depth/location), battery levels, signal strength, last communication time, and operational status (active, low battery, offline). Essential for sensor network maintenance, data continuity assurance, and monitoring system reliability. AI agents should reference this when users ask "are all sensors working in bin 5", "which sensors need battery replacement", or need sensor network health data for system administration.

Get health status and battery levels of wireless sensors in a grain bin
- **get_spoilage_predictions**: Returns spoilage risk level (low, moderate, high, critical), predicted days until spoilage onset, confidence scores, and recommended preventive actions. Essential for proactive grain management, early intervention planning, and quality preservation. AI agents should use this when users ask "what is the spoilage risk for bin 3", "when will grain quality degrade in silo 5", or need AI-driven risk assessments for storage management decisions.

Get AI-powered spoilage risk predictions for a specific grain bin
- **get_temperature_history**: Temperature increases often indicate active spoilage, insect activity, or mold growth. Returns time-series temperature data (Celsius) with timestamps from multiple sensor depths and positions. Essential for hot spot detection, spoilage heating identification, aeration effectiveness evaluation, and grain quality preservation. AI agents should reference this when users ask "show me temperature trends for bin 4", "are there any hot spots developing in silo 6", or need historical temperature data for spoilage analysis.

Get historical temperature readings to detect hot spots and spoilage heating


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Centaur Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current CO2, moisture, and temperature readings for bin 5."

**🤖 AI Agent:**
> Fetching current readings for bin 5 (Corn, 78% full)... CO2: 920 ppm (normal, no biological activity detected). Moisture: 14.1% (stable, within safe storage range). Temperature: Average 12.3C across all sensors, max 13.1C at center, min 11.8C at walls. All 24 wireless sensors reporting healthy. Assessment: Grain condition is EXCELLENT — no spoilage indicators detected. CO2 is well below the 1500 ppm warning threshold. Temperature is uniform with no hot spots. Continue routine monitoring. Next full assessment recommended in 7 days.

---

**👤 You:**
> "What is the AI spoilage prediction for my soybean bin?"

**🤖 AI Agent:**
> Analyzing AI spoilage predictions for soybean bin (bin ID: SB-2847)... Current risk level: LOW. Predicted days until spoilage: 45+ days. Confidence: 87%. Key indicators: CO2 at 780 ppm (stable trend), moisture at 12.8% (well below critical), temperature uniform at 10.5C. AI recommendation: Current storage conditions are optimal. Soybean quality is expected to remain stable through the next 6 weeks. No intervention required. Schedule next quality assessment in 14 days. Marketing recommendation: Current quality supports premium pricing — consider forward contracting if market conditions are favorable.

---

**👤 You:**
> "Give me a facility-wide overview of all grain bins and any active alerts."

**🤖 AI Agent:**
> Generating facility overview... Total bins: 18. Total inventory: 42,300 tonnes. Average CO2: 980 ppm (normal). Average moisture: 13.9% (stable). Active alerts: 2. Alert 1 (WARNING): Bin 7 — Moisture migration detected at top layer, 15.2%. Recommend targeted aeration. Alert 2 (INFO): Bin 12 — Sensor #8 battery at 15%, schedule replacement within 2 weeks. Overall facility risk: LOW. 16 of 18 bins in excellent condition. Facility quality score: 92/100. Priority actions: Address moisture in Bin 7, replace sensor battery in Bin 12. Would you like detailed recommendations for each alert?


## Installation & Usage

To install and use the **Centaur Analytics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/centaur-analytics](https://vinkius.com/mcp/centaur-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
