# Wiagro MCP Server

Access smart silobag monitoring via Wiagro — track temperature, humidity, CO2, rupture detection, and grain quality from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wiagro)

## Overview
**Category:** iot-hardware
**Tools Count:** 12

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


## Available Tools
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


## Installation & Usage

To install and use the **Wiagro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wiagro](https://vinkius.com/mcp/wiagro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
