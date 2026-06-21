# OpenF1 Live Data & Telemetry MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openf1-live-data-telemetry)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openf1-live-data-telemetry-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openf1-live-data-telemetry-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Real-time Formula 1 telemetry and race data — audit lap times, car performance, and team radio via AI.

## Description
Transform your AI agent into a professional Formula 1 data analyst with **OpenF1**. This high-performance server provides unprecedented access to granular race data and live car telemetry directly from the track. Your agent can monitor high-frequency technical metrics such as RPM, gear usage, and throttle application, while also tracking the narrative of the race through team radio links and official FIA race control messages. Whether you are analyzing tire strategies, auditing sector times, or following live overtakes, your agent provides deep technical intelligence through natural conversation.

### What you can do

- **Technical Analysis** — Retrieve live car telemetry including speed, engine RPM, and DRS usage for any driver directly from the session data
- **Race Narrative** — Follow team radio communications and official race control updates in real-time to understand race incidents
- **Strategy Auditing** — Track tire compounds, stint lengths, and pit stop durations across the entire field to map race strategy
- **Performance Benchmarking** — Compare sector times (S1, S2, S3) and lap-by-lap consistency to identify precise performance gaps

### How it works

1. Subscribe to this server
2. No API key required for public access
3. Start managing your F1 intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **F1 Strategy Enthusiasts** — perform deep audits of tire wear and sector performance to predict race outcomes
- **Data Journalists** — instantly retrieve high-frequency telemetry for technical reporting and race breakdowns
- **Professional Fans** — monitor team radio and race control messages straight from your workflow to never miss a steward decision


## Available Tools
- **list_drivers**: List F1 drivers for a session
- **get_starting_grid**: Get the initial race starting grid
- **get_driver_intervals**: Get intervals and gaps between drivers
- **get_lap_times**: Get lap and sector times
- **list_overtakes**: List all overtakes during a race
- **list_pit_stops**: List pit stop durations
- **get_race_control_messages**: Get FIA race control messages
- **get_team_radio**: Get team radio recording links
- **get_session_results**: Get final classification for a session
- **list_sessions**: List F1 sessions for a year
- **get_driver_standings**: Get current driver championship standings
- **get_team_standings**: Get current team championship standings
- **list_tyre_stints**: List tyre strategy and stints
- **get_car_telemetry**: Get technical telemetry for a car
- **get_weather_data**: Get track and air weather data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenF1 Live Data & Telemetry** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the technical telemetry for Max Verstappen in the latest session."

**🤖 AI Agent:**
> I've retrieved Verstappen's high-frequency telemetry. At the last sample, he was at 312 km/h in 7th gear at 11,200 RPM with DRS active. I also have his throttle and brake traces. Would you like to compare this to his previous lap?

---

**👤 You:**
> "Analyze the tire strategy for the top 5 drivers in the current session."

**🤖 AI Agent:**
> Running the stint query... I found that Verstappen and Norris are currently on Mediums (8 laps old), while Hamilton has just pitted for new Hards. I have the full stint history for the top 5. Would you like to see the projected life of their current sets?

---

**👤 You:**
> "Provide all race control messages involving 'Track Limits' from lap 10 onwards."

**🤖 AI Agent:**
> Inspecting FIA updates... I found 3 messages regarding Track Limits since lap 10. Drivers warned include Perez at Turn 4 and Leclerc at Turn 12. No penalties have been issued yet. Shall I continue monitoring for specific driver numbers?


## Installation & Usage

To install and use the **OpenF1 Live Data & Telemetry** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openf1-live-data-telemetry](https://vinkius.com/mcp/openf1-live-data-telemetry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
